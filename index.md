---
title       : Predict the next word!
subtitle    : A Shiny app
author      : K. J.
job         : R Capstone
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : solarized_light      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides

--- .segue .quote .dark

<q> A new web-based app that predicts the next word in a sentence</q>

<style>
.dark q {
  color: white;
}
</style>

--- .class #id

## Overview

The Shiny app predicts the next word in a sentence.

It makes use of n-gram language models, specifically
- Markov Chains to store n-grams (up to 5-grams used)
- Katz's back-off model to estimate the probability against its history



--- .class #id 

## Dataset

This app makes use of english language blog, twitter and news text results, from a corpus called HC Corpora (www.corpora.heliohost.org)



--- .class #id 

## Instructions

Simple!

1. Type the phrase into the text box
2. Click submit

