# README

This repository contains source and rendered output for *epicontacts: Handling, Visualisation and Analysis of Epidemiological Contacts*.

The manuscript is written in R Markdown, and can be found in `epicontacts-paper.Rmd` ... note that this is the only place you need to edit for narrative content. This file includes a mix of evaluated and unevaluated R code chunks, and uses the `f1000_article` R Markdown latex template from [**BiocWorkflowTools**](http://bioconductor.org/packages/release/bioc/html/BiocWorkflowTools.html). Figures were generated outside of the document and are included using standard [Markdown syntax](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#images).  If you are adding a new citation, add a [BibTex version](http://www.bioinformatics.org/texmed/) entry to `biblio.bib` and inline reference. 

To render the document, make sure you have the necessary packages installed ...

```
install.packages(c("rmarkdown", "epicontacts", "outbreaks"))

source("https://bioconductor.org/biocLite.R")
biocLite("BiocWorkflowTools")
```

... then from the root of the repository run `rmarkdown::render("epicontacts-paper.Rmd")`
