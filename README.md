
<!-- README.md is generated from README.Rmd. Please edit that file -->

# nixtlar

The `nixtlar` package provides R users with a SDK for [Nixtla’s TimeGPT
API](https://docs.nixtla.io/).

<!-- logo -->

# nixtlar <a href="https://nixtla.github.io/nixtlar/"><img src="man/figures/logo.png" align="right" height="139" alt="nixtlar website" /></a>

<!-- badges: start -->

[![CRAN
status](https://www.r-pkg.org/badges/version/nixtlar)](https://CRAN.R-project.org/package=nixtlar)
[![R-CMD-check](https://github.com/MMenchero/nixtlar/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/MMenchero/nixtlar/actions/workflows/R-CMD-check.yaml)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue)](https://www.apache.org/licenses/LICENSE-2.0)
<!-- badges: end -->

## 🔄 nixtlar: Your Gateway to TimeGPT from R

With `nixtlar` you can easily interact with TimeGPT through simple API
calls, making the power of TimeGPT readily accessible in your projects.
Learn more about TimeGPT [here](https://arxiv.org/abs/2310.03589).

## 💻 Installation

You can install the development version of `nixtlar` from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
#devtools::install_github("MMenchero/nixtlar")
```

## 🎈Quick Start

To use TimeGPT, you first need to request a token from Nixtla. You can
do this at <https://dashboard.nixtla.io/>.

Once you have the token, you’ll need to set it up in your R session. The
`nixtlar` package provides a function to do this.

``` r
#library(nixtlar)

# Set up token 
#set_token("YOUR_TOKEN") 
```

You’ll need to set the token every time you re-start your R session.
`nixtlar` also includes a function to validate the token.

``` r
# Validate token
#validate_token("YOUR_TOKEN") 
```

You don’t need to validate the token every time you set it up, only when
you want to ensure its validity.

`nixtlar provides` an easy-to-use function to call the TimeGPT API. It
works with both [tsibbles](https://tsibble.tidyverts.org/) and base R
data frames.

``` r
# Call the TimeGPT API 
#df <- tssible::as_tsibble(AirPassengers) # df can also be a data frame  

#timegpt_forecast(df, h=8, freq=12, time_col="index", target_col="value")
```

## 🐍 Python SDK

Are you a Python user? If yes, then check out
[NixtlaTS](https://github.com/Nixtla/nixtla), a Python SDK for TimeGPT
and check out the [documentation](https://docs.nixtla.io/docs).
