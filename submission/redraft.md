<!--
title: 'Understanding data fabrication: Qualitative Comparative Analysis (QCA) of
fabrication strategies'
author: "CHJ Hartgerink"
date: '`r format(Sys.time(), "%d %B, %Y")`'
output:
  word_document: default
  pdf_document:
    toc: yes
  html_document:
    toc: yes
    toc_depth: 2
csl: ../bibliography/apa.csl
bibliography: ../bibliography/library.bib
-->


# Introduction 

Cases of data fabrication in research often peak the interest of people in research and beyond, where it speaks to the imagination to understand why, what, or how data were fabricated. 
For reasons why researchers fabricate data, some look at systemic origins (i.e., the bad barrel argument), such as the highly competitive research system [@10.1172/JCI36371;10.1038/521259a], whereas others look to personality traits that might be predictive of likelihood to commit misconduct [i.e., the bad-apple argument; @10.1038/534173a]. 
What was fabricated (i.e., which results) is often a question that drives scientific integrity committees established to investigate the case in order to correct the scientific record.

How data are fabricated remains puzzling because of incomplete knowledge of cases and lack of first-hand information on data fabrication. 
We have incomplete knowledge about data fabrication strategies because those that are effective at avoiding detection are not available for self-evident reasons (i.e., discovery bias). 
Vice versa, the cases we do know about can teach us what strategies are unsuccessful, but not the range of strategies that potentially are applied.
However, those cases that are discovered often do not result in confessions with explicit descriptions of how they fabricated the data. 
For example, Diederik Stapel confessed to fabricating data and wrote a book about his recollections and interpretations [@stapel2012ontsporing]. 
This is an exceptional case because of the confessive approach he takes. 
However, even in this exceptional case little specific information is available as to how he fabricated data to be of value for research on data fabrication strategies. 
The following excerpt includes a general description of how he fabricated data over the years [@stapel2012ontsporing;@apsstapel]:

>I preferred to do it at home, late in the evening, when everyone was asleep. I made myself some tea, put my computer on the table, took my notes from my bag, and used my fountain pen to write down a neat list of research projects and effects I had to produce ... Subsequently I began to enter my own data, row for row, column for column ... 3, 4, 6, 7, 8, 4, 5, 3, 5, 6, 7, 8, 5, 4, 3, 3, 2. When I was finished, I would do the first analyses. Often, these would not immediately produce the right results. Back to the matrix and alter data. 4, 6, 7, 5, 4, 7, 8, 2, 4, 4, 6, 5, 6, 7, 8, 5, 4. Just as long until all analyses worked out as planned. (p. 167)

Moreover, when scientific integrity committees investigate for data fabrication, rarely will they be able to conclusively state how data were fabricated. 
Some data fabrication strategies might be obvious if the raw data are available (e.g., copy-pasting responses), whereas others will be less obvious (e.g., multivariate modeling of the observed variables for the desired outcomes). 
Moreover, many fabricated results have underdetermined data fabrication strategies (i.e., multiplicity). 
That is, many different fabrication strategies can result in the observed data set, such that differentiating which one actually occurred based on the data is non-trivial [see also @10.12688/f1000research.12584.1].
Additionally, given that odds of data availability decrease each year after publication [@10.1016/j.cub.2013.11.014], methods to learn about how data were fabricated retrospectively by looking at the dataset are increasingly unfeasible even if underdetermination was not a problem. 
Data availability is especially problematic in cases where it takes longer to uncover problems in the first place, such that data are more likely to be unavailable for investigation in cases that go undetected longer.
Second-hand information about data fabrication offers relatively little indication on how data are actually fabricated by researchers due to this underdetermination and increasing lack of data availability.

Hence, first-hand knowledge from controlled settings about how researchers fabricate data is useful to further understand and maybe even improve detection of data fabrication in uncontrolled settings. 
There is unknown variability in how researchers fabricate data, which could result in foregone detection mechanisms if we focus on the limited and preselected knowledge that is available. 
However, we currently do not even know what methods are used and therefore only operate from hunches and inferences from psychology theory [e.g., @Haldane1948-nm] and how often they occur.
As far as we know, only one such study asked participants to fabricate data, but did not investigate how they did so [@10.1136/bmj.331.7511.267].
Qualitative information would provide a first-hand insight into how data are fabricated and could provide fruitful avenues for the development of new statistical tools to detect data fabrication. 

In this report, we qualitatively assess the data fabrication strategies that practicing researchers used to fabricate data in one of our controlled studies [@2015ori-1]. 
Based on the transcripts of the interviews about how participants fabricated data [@10.5281/zenodo.832490], we apply qualitative methods to learn more about characteristics of the observed data fabrication strategies. 
Moreover, we combine the observed data fabrication strategies with results from various statistical tools to detect data fabrication [see also @], in order to assess whether certain data fabrication characteristics cause better or worse detection.

# Methods

We used transcripts of 28 interviews with researchers who we previously asked to fabricate data in a controlled setting [available at @10.5281/zenodo.832490]. 
In these interviews, we asked participating researchers to answer questions separated into five sections. 
Section 1 pertained to general information about the researcher (e.g., frequent programs used). 
Section 2 inquired about the time and days spent on fabricating data (e.g., how many hours spent). 
Section 3 asked the researcher about their general framework with which they fabricated the data (e.g., what makes data look weird according to them).
Section 4 focused on the specific steps taken to fabricate data (e.g., did they use a (pseudo-)random number generator).
Section 5 was about the motivations of the researcher to participate in this study and their general assessment of their performance.

To recapitulate, we previously asked these 28 researchers to fabricate raw data for a Stroop experiment [see Figure 1; @stroop1935]. 
In short, a Stroop experiment is typically a within-subjects experiment with two conditions measuring response times: (1) congruent (e.g., the word 'red' is presented in red) and (2) incongruent (e.g., the word 'red' is presented in green). 
We asked the participating researchers to fabricate response times for 25 participants, such that there was a statistically significant effect between conditions (i.e., a Stroop effect). 
Using these fabricated data, we tested whether statistical methods could help  separate fabricated data sets from (assumably) genuine datasets from Many Labs 3 [[https://osf.io/n8xa7/](https://osf.io/n8xa7/); @10.1016/j.jesp.2015.10.012].

![Example of a filled in template spreadsheet used in the fabrication process. Respondents fabricated data in the yellow cells and green cells, which were used to compute the results of the hypothesis test of the condition effect. If the fabricated data confirm the hypotheses, a checkmark appeared. This template is available at [https://osf.io/2qrbs/](https://osf.io/2qrbs/).](../figures/spreadsheet2.png)

For each of the 28 transcripts, the first author coded data fabrication characteristics. Based on a first-reading of all transcripts, we identified five key data fabrication characteristics. We also identified ten participant characteristics. Subsequently, the first author As such, the first author read through three transcripts to qualitatively assess various data fabrication characteristics available in the transcripts. Additionally, we coded characteristics of the fabricator's experience, which we include in the data set ([osf.io/xxxx](https://osf.io/xxxx)) for completeness but do not analyze considering these are not part of the data fabrication strategy per se.

<!-- https://raw.githubusercontent.com/chartgerink/2015ori-2/c706d77e4d85daa285624028d379d7b9b00bd1d0/submission/manuscript.Rmd -->

# Results

# Discussion

# Author's note

All materials used in this project are available at [https://github.com/chartgerink/2015ori-2](https://github.com/chartgerink/2015ori-2) and are preserved at Zenodo.

# References
