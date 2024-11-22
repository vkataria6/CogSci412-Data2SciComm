---
title: "Weekly Assignment 11"
author:
- name: Vidushi Kataria
  affiliation: '1'
  corresponding: yes
  email: vk412@scarletmail.rutgers.edu
  role:
  - Conceptualization
  - "Writing - Original Draft Preparation"
  - "Writing - Review & Editing"
affiliation:
- id: '1'
  institution: "Rutgers University--New Brunswick"
output:
  papaja::apa6_pdf:
    theme: cerulean
    toc: yes
    toc_float:
      collapsed: yes
  '': default
abstract: "One or two sentences providing a **basic introduction** to the field,  comprehensible
  to a scientist in any discipline.\nTwo to three sentences of **more detailed background**,
  comprehensible  to scientists in related disciplines.\nOne sentence clearly stating
  the **general problem** being addressed by  this particular study.\nOne sentence
  summarizing the main result (with the words \"**here we show**\" or their equivalent).\nTwo
  or three sentences explaining what the **main result** reveals in direct comparison
  to what was thought to be the case previously, or how the  main result adds to previous
  knowledge.\nOne or two sentences to put the results into a more **general context**.\nTwo
  or three sentences to provide a **broader perspective**, readily comprehensible
  to a scientist in any discipline.\n\n<!-- https://tinyurl.com/ybremelq -->\n"
keywords: keywords
wordcount: X
bibliography: "r-references.bib"
floatsintext: no
linenumbers: yes
draft: no
mask: no
figurelist: no
tablelist: no
footnotelist: no
classoption: man
authornote: |
  Add complete departmental affiliations for each author here. Each new line herein must be indented, like this line.
  Enter author note here.
---








```
## Warning: package 'ggplot2' was built under R version 4.3.1
```

```
## Warning: package 'tidyr' was built under R version 4.3.1
```

```
## Warning: package 'dplyr' was built under R version 4.3.1
```

```
## Warning: package 'lubridate' was built under R version 4.3.1
```

```
## Warning: package 'ggdist' was built under R version 4.3.1
```

# Introduction & Research Objectives

Comparing proportions is sometimes very hard! But, even infants seem to be able to do it a little bit. The purpose of this science project was to better understand how well people compare proportions when they are presented in different formats. Such insights contribute to the broader understanding of decision-making processes and the role of stimulus presentation in cognitive tasks.

This study aims to address the following research questions:
1. Does average performance vary across format type?
2. Does average performance vary across numerator congruency status?
3. Does numerator congruency vary across format type? (i.e., is there an interaction)


# Method


A total of 99 adults participated in the study. 


First, participants were introduced to a story about a magic ball and that the outcome (i.e., blue or orange) depended on the proportions. They were then asked to compare the proportions of different images.

In other words, participants were shown two images of the same kind at the same time and were asked to decide which had a higher proportion of the shape (or dots) colored in blue.

![ ](images_WA10/Probtask_Trial.png) 


There were four different conditions that changed what kinds of images the participants saw:

- divided blobs: blue and orange were entirely separate
- integrated blob: one blob, divided to be part blue and part orange
- separated dots: blue and orange dots were on opposite sides of the image
- integrated dots: blue and orange were intermixed 

![ ](images_WA10/Probtask_formats.png) 


# Results

1. Does average performance vary across format type, ignoring all other aspects of the stimuli?



![(\#fig:fig-1)This plot is measuring proportion correct responses with distributional information.](Kataria_WA11_files/figure-latex/fig-1-1.pdf) 
When considering only format type (blobs vs. dots), the (`fig-1`) plot reveals no clear systematic difference in average performance between the two formats, as both blob and dot conditions show similar ranges of accuracy (approx 62-69% correct responses) w/ substantial overlap in their distributions.


2. How are reaction time and accuracy related?




![(\#fig:fig-2)This plot is measuring reaction time and its impact on accuracy by condition.](Kataria_WA11_files/figure-latex/fig-2-1.pdf) 
According to (`fig-2`), reaction time tends to have an overall **positive** correlation. As reaction time *increases*, the proportion correct appears to *rise.* (However, there is some variability with *blob_stacked* and *dots_EqSizeSep*).


3. How does numerator congruency interact with format type?







![(\#fig:fig-3)This plot is measuring the interaction between format type and numerator congruency.](Kataria_WA11_files/figure-latex/fig-3-1.pdf) 
In (`fig-3`), it shows that across all four visualization conditions, participants consistently performed better when the numerator was congruent (TRUE) with the overall ratio compared to when it was incongruent (FALSE). 



## Data analysis
We used R [Version 4.3.0\; @R-base] and the R-packages *dplyr* [Version 1.1.4\; @R-dplyr], *forcats* [Version 1.0.0\; @R-forcats], *ggdist* [Version 3.3.2\; @R-ggdist], *ggplot2* [Version 3.5.1\; @R-ggplot2], *lubridate* [Version 1.9.3\; @R-lubridate], *papaja* [Version 0.1.3\; @R-papaja], *purrr* [Version 1.0.2\; @R-purrr], *readr* [Version 2.1.4\; @R-readr], *stringr* [Version 1.5.0\; @R-stringr], *tibble* [Version 3.2.1\; @R-tibble], *tidyr* [Version 1.3.1\; @R-tidyr], *tidyverse* [Version 2.0.0\; @R-tidyverse] and *tinylabels* [Version 0.2.4\; @R-tinylabels] for all our analyses.


# Discussion
The three key findings from these three objectives are **format effect** (blobs vs. dots), **speed-accuracy relationship**, and the **numerator congruency effect**. 
The choice between blob or dots format does not appear to meaningfully impact performance accuracy.
There appears to be a speed-accuracy tradeoff, where participants who took more time tended to achieve a higher accuracy. However, there was some variation in the blob_stacked and dots_EqSizeSep formats. 
There was also a consistent pattern that emerged across all visualization types where performance was superior when the numerator aligned with the overall ratio. 


1. Personally, the most annoying thing about this assignment (and making posters/presentations in R in general) is not knowing what is going to print before knitting. I think labeling code chunks can be a pain as well. But at least R tells you immediately after knitting what the issue is.

2. The most satisfying thing about this assignment is seeing everything you intend to print while knitting your poster. 


\newpage

# References

::: {#refs custom-style="Bibliography"}
:::
