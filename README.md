# CV-as-a-Code

> Based on work of [mrzool](https://github.com/mrzool/cv-boilerplate) and [semirook](https://github.com/semirook/itcv).

Resume is compiled based on LaTeX template - `tamplate.tex` and content file `content.yml` in YAML format.
This nicely separates presentation layer from data layer.

To compile CV just run *(ensure that dependencies are installed)*:

```
make
```

This will produce PDF file `output.pdf` with a resume.


## Dependencies

### For macOS

Install required packages:

```
brew install pandoc
brew cask install basictex
```

Update `PATH` (if needed) with `/usr/local/texlive/2019basic/bin/x86_64-darwin`.


Update `tlmgr` utily
```
sudo tlmgr update --self
```

Get [texliveonfly](https://www.ctan.org/pkg/texliveonfly) to pn-the-fly download of missing TEX live packages:

```
sudo tlmgr install texliveonfly
```

Or get required packages manually:

```
sudo tlmgr install fontspec geometry multicol xunicode xltxtra marginnote sectsty ulem hyperref polyglossia
```


## Resources

1. [Installing (La)TeX on Mac, the Sane Way](https://ryan-holben.github.io/tex/latex/installation/macos/2016/08/21/installing-tex-on-mac/)
