To have a usable 'git diff' on ODP files
========================================

Install odt2txt
[https://github.com/dstosberg/odt2txt](https://github.com/dstosberg/odt2txt)

Add to ~/.gitconfig:

```
[core]
  attributesFile = ~/.gitattributes
[diff "odp"]
  textconv = odt2txt
```

And to ~/.gitattributes:

```
*.odp diff=odp
```


Now `git diff` should display textual changes from ODP files
