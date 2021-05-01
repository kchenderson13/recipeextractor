---
title: "recipeextractor"
author: "Kylie Henderson"
date: "`r Sys.Date()`"
output: github_document
---
A package extending the capability of [reddit]
by enhancing the users experience in searching for recipes using only
specified ingredients.

##Install

Install from GitHub with the following code:
```{r install, eval = FALSE}
if (!requireNamespace("devtools", quietly = TRUE)) {
  install.packages("devtools")
}
devtools::install_github("kyliehenderson13/recipeextractor")
```

##Usage

The user will enter the following

```{setup instructions, eval = FALSE}
    recipe = function(ingredient, pages){
  df = RedditExtractorR::reddit_urls(search_terms = paste0(ingredient, ",",
  "recipe"), page_threshold = pages)
  assign("recipe_object", df, envir = GlobalEnv)
}
```

This must be done at the start of the session to establish the function.

## Load RedditExtractorR

## Now you can begin to customize your search

## Create an object and begin your search placing in you rpreferred ingredients 
## and page threshhold
example1 = RedditExtractoR::reddit_urls("broccoli, cheese, recipe", 
page_threshold = 3)

## After doing this, your object should exemplify the results you are searching

You can continue to search for different ingredients, and list as many as you 
would like. Be aware that the more specific you get with ingredients, the 
more narrow your search results will be
For best results, it is suggested to list no more than 5-7 ingredients or the
results will be too specific




