
<!-- README.md is generated from README.Rmd. Please edit that file -->

[![Travis-CI Build
Status](http://badges.herokuapp.com/travis/Trackage/trip?branch=master&env=BUILD_NAME=trusty_release&label=linux)](https://travis-ci.org/Trackage/trip)
[![OSX Build
Status](http://badges.herokuapp.com/travis/Trackage/trip?branch=master&env=BUILD_NAME=osx_release&label=osx)](https://travis-ci.org/Trackage/trip)
[![AppVeyor build
status](https://ci.appveyor.com/api/projects/status/github/mdsumner/trip?branch=master&svg=true)](https://ci.appveyor.com/project/mdsumner/trip)[![Coverage\_Status](https://img.shields.io/codecov/c/github/Trackage/trip/master.svg)](https://codecov.io/github/Trackage/trip?branch=master)
[![CRAN\_Status\_Badge](http://www.r-pkg.org/badges/version/trip)](https://cran.r-project.org/package=trip)
[![CRAN\_Download\_Badge](http://cranlogs.r-pkg.org/badges/trip)](https://cran.r-project.org/package=trip)

# Tools for animal track data

The trip package provides functions for accessing and manipulating
spatial data for animal tracking. Filter for speed and create time spent
plots from animal track data.

# Development

There is some ongoing integration with the `sf` package, mostly to
provide outputs in its formats. Trip itself would be better implemented
on top of the ideas in <https://github.com/r-gris/rangl/>, rather than
shoe-horned into a weird twilight zone between MULTIPOINTs and
LINESTRINGs as it is now.

## Installing

The package is easily installed from CRAN in R.

``` r
install.packages("trip")
```

## Install dev version

To install the development package from Github, use `devtools`:

``` r
devtools::install_github("mdsumner/trip")
```

## TODO

  - **Probability image**. The SGAT (and tripEstimation) packages have
    functions for dealing with spatial track summaries that are atomized
    to the level of each time step. There are methods for combining
    summaries from multiple tracks and for casting arbitrary durations
    (by sum) to standard image structures. This would be a good feature
    to replace the existing tripGrid function by storing the individual
    grid summaries for each implicit line segment.

  - **Coercion to/from other classes** See
    [spbabel](https://github.com/mdsumner/spbabel).

  - **Validation** Must include a detailed report object of where the
    problems are, and how to filter/fix/flush them.

Please note that this project is released with a [Contributor Code of
Conduct](CONDUCT.md). By participating in this project you agree to
abide by its terms.
