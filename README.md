<!-- ---------------------------------------------------------------------- -->

<!-- badges: start -->
[![CRAN status](https://www.r-pkg.org/badges/version-last-release/hySpc.read.mat)](https://cran.r-project.org/package=hySpc.read.mat)
[![R-CMD-check](https://github.com/r-hyperspec/hySpc.read.mat/workflows/R-CMD-check/badge.svg)](https://github.com/r-hyperspec/hySpc.read.mat/actions)
![Website (pkgdown)](https://github.com/r-hyperspec/hySpc.read.mat/workflows/Website%20(pkgdown)/badge.svg)
[![Codecov](https://codecov.io/gh/r-hyperspec/hySpc.read.mat/branch/develop/graph/badge.svg)](https://codecov.io/gh/r-hyperspec/hySpc.read.mat?branch=develop)
[![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
<!--[![metacran downloads](https://cranlogs.r-pkg.org/badges/grand-total/hySpc.read.mat)](https://cran.r-project.org/package=hySpc.read.mat)-->
<!--[![metacran downloads](https://cranlogs.r-pkg.org/badges/hySpc.read.mat)](https://cran.r-project.org/package=hySpc.read.mat)-->
<!-- badges: end -->



# R Package **hySpc.read.mat**

[**R**](https://www.r-project.org/) package **hySpc.read.mat** is a member of the [**`r-hyperspec`**](https://r-hyperspec.github.io/) packages family, which import MATLAB files into hyperSpec.

<!-- ---------------------------------------------------------------------- -->

## Documentation

There are two versions of **hySpc.read.mat** online documentation:

a. for the [released version](https://r-hyperspec.github.io/hySpc.read.mat/) of package,  
b. for the [development version](https://r-hyperspec.github.io/hySpc.read.mat/dev/) of package.

The documentation of the other **`r-hyperspec`** family packages can be found at [r-hyperspec.github.io](https://r-hyperspec.github.io/).

<!-- ---------------------------------------------------------------------- -->

## Installation

### Install from CRAN

You can install the released version of **hySpc.read.mat** from [CRAN](https://cran.r-project.org/package=hySpc.read.mat) with:

```r
install.packages("hySpc.read.mat")
```


### Install from GitHub

You can install the development version of the package from [GitHub](https://github.com/r-hyperspec/hySpc.read.mat):

```r
if (!require(remotes)) {install.packages("remotes")}
remotes::install_github("r-hyperspec/hySpc.read.mat")
```

**NOTE 1:**
Usually, "Windows" users need to download, install and properly configure **Rtools** (see [these instructions](https://cran.r-project.org/bin/windows/Rtools/)) to make the code above work.

**NOTE 2:**
This method will **not** install package's documentation (help pages and vignettes) into your computer.
So you can either use the [online documentation](https://r-hyperspec.github.io/) or build the package from source (see the next section).


### Install from Source

1. From the **hySpc.read.mat**'s GitHub [repository](https://github.com/r-hyperspec/hySpc.read.mat):
    - If you use Git, `git clone` the branch of interest.
      You may need to fork it before cloning.
    - Or just chose the branch of interest (1 in Figure below), download a ZIP archive with the code (2, 3) and unzip it on your computer.  
![image](https://user-images.githubusercontent.com/12725868/89338263-ffa1dd00-d6a4-11ea-94c2-fa36ee026691.png)

2. Open the downloaded directory in RStudio (preferably, as an RStudio project).
    - The code below works correctly only if your current working directory coincides with the root of the repository, i.e., if it is in the directory that contains file `README.md`.
    - If you open RStudio project correctly (e.g., by clicking `project.Rproj` icon ![image](https://user-images.githubusercontent.com/12725868/89340903-26621280-d6a9-11ea-8299-0ec5e9cf7e3e.png) in the directory), then the working directory is set correctly by default.

3. In RStudio 'Console' window, run the code (provided below) to:
    a. Install packages **remotes** and **devtools**.
    b. Install **hySpc.read.mat**'s dependencies.
    c. Create **hySpc.read.mat**'s documentation.
    d. Install package **hySpc.read.mat**.

```r
# Do not abort installation even if some packages are not available
Sys.setenv(R_REMOTES_NO_ERRORS_FROM_WARNINGS = "true")

# Install packages remotes and devtools
install.packages(c("remotes", "devtools"))

# Install hySpc.read.mat's dependencies
remotes::install_deps(dependencies = TRUE)

# Create hySpc.read.mat's documentation
devtools::document()

# Install package hySpc.read.mat
devtools::install(build_vignettes = TRUE)
```

**NOTE 1:**
Usually, "Windows" users need to download, install and properly configure **Rtools** (see [these instructions](https://cran.r-project.org/bin/windows/Rtools/)) to make the code above work.