# Project management in R

[A Quick Guide to Organizing Computational Biology Projects](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1000424)
[A workflow for R](http://blog.revolutionanalytics.com/2010/10/a-workflow-for-r.html)

Similar projects:
[ProjectTemplate](http://projecttemplate.net/)

## Project structure

### Packages and functions
1. Required packages (maybe just stick with packrat)
2. Project-specific functions (should be documented via roxygen; maybe add support for tests).

### Data and data pre-processing
1. Should be as abstract as possible - from single files to databases.
2. Cache data after pre-processing (archivist?).
3. Allow more abstract storage than R memory or RData (ff package, archivist, RODBC?)
4. How to document data? External file with links to data?

### Analysis
1. Cache results (archivist)
2. Reporting (knitr, rmarkdown).

## Additional features

1. Sanity checks:
 - tests
 - concordance of results of analysis (for the same data chunks)
