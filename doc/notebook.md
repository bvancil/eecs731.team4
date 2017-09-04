# Notebook

## Reproducibility ideas

### [`checkpoint`](http://mran.revolutionanalytics.com/packages/info/?checkpoint)

```R
# Do once
install.packages("checkpoint")
# In a script named "checkpoint.R":
library("checkpoint")
checkpoint("2017-09-04")
# Use at the top of each script:
source("checkpoint.R")
```

### [`packrat`](http://rstudio.github.io/packrat/)

```R
# Do once per project
install.packages("packrat")
packrat::init(path_to_project)
# Do once per other developer
install.packages("packrat")
# When installing a new package
packrat::snapshot()
# When restoring new packages saved by others
# Just make sure that the files ".Rprofile" and "packrat/packrat.lock" are preserved
# Also:
packrat::restore()
# What's the status of the local library?
packrat::status()
# Look into options for version control:
packrat::set_opts(vcs.ignore.src = TRUE)
packrat::set_opts(vcs.ignore.lib = TRUE)
```

### [`gRAN`](https://github.com/gmbecker/gRAN)

Seems not to be as widely used

## Data analysis ideas

### Papers

### Methods

