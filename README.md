# README

This repository contains source and rendered output for *epicontacts: Handling, Visualisation and Analysis of Epidemiological Contacts*.

The narrative content is written in Markdown, and can be found in `epicontacts.Rmd`. This file includes a mix of evaluated and unevaluated R code chunks, and uses the `f1000_article` R Markdown latex template from [**BiocWorkflowTools**](http://bioconductor.org/packages/release/bioc/html/BiocWorkflowTools.html). Figures were generated outside of the document and are included using standard [Markdown syntax](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#images). Citations are defined in the `biblio.bib` file, and embedded inline.

To render the document, make sure you have the necessary packages:

```
install.packages(c("rmarkdown", "epicontacts", "outbreaks"))

source("https://bioconductor.org/biocLite.R")
biocLite("BiocWorkflowTools")
```

Then from the root of the repository run `rmarkdown::render("epicontacts-paper.Rmd")`
