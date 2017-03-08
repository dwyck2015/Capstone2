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

The Shiny app predicts the next word in a sentence using n-gram language models.


Simple Instructions!
<ol start="1">
<li> Go to app: https://johnsonkd.shinyapps.io/NextWordApp/ </li>
<li> Type the phrase into the text box </li>
<li> Click submit </li>
</ol>



--- .class #id 

## Dataset

This app makes use of english language blog, twitter and news text results, from a corpus called HC Corpora (www.corpora.heliohost.org)

60% of each of the following files were used for algorithm development (40% for testing)
- en_US.blogs.txt (899,288 lines & 37,546,246 words)
- en_US.news.txt (77,259 lines & 2,674,536)
- en_US.twitter.txt (2,360,148 lines & 30,093,410 words)



--- .class #id 

## Model development

It makes use of n-gram language models for a clean dataset:
- Curse words, stopwords, capitalization, punctuation are removed
- Markov Chains to store n-grams (1-grams to 5-grams used)
- Katz's back-off model to estimate the probability against its history (with penalty applied to probability score to get more matches)


THANK YOU!
Please send feedback to: dwyck_kdjohns@gmail.com
