```{r, echo = FALSE}
fignr <- 1
tabnr <- 1

suppressPackageStartupMessages(if(!require(QCA)){install.packages('QCA', repos = 'http://cran.us.r-project.org')})
suppressPackageStartupMessages(library(QCA))

```

# Methods

## Data 

<!-- Dit kan pas goed als de andere paper af is. -->

We also reused the results from five statistical methods to detect data fabrication, as the basis for the outcome measure of our Qualitative Comparative Analysis [QCA; @rihoux2008]. In our original study [@], we compared AANTAL methods to detect data fabrication across a set of 20 genuine data sets [retrieved from @] and 28 fabricated data sets. Five statistical methods proved effective in detecting data fabrication, including four different comparisons of multivariate relations and one comparing reported effect sizes. We used the results of these methods as the outcome measures for our Qualitative Comparative Analysis (QCA; more thoroughly explained below). More specifically, we computed the dichotomous outcome measure (i.e., data detected as fabricated or not) by specifying a decision criterion such that all data sets detected as fabricated were indeed fabricated (i.e., no  false positives).

<!-- Ok, ik snap het, maar kun je proberen iets minder vaag te maken hoe dit werkte? -->

This inductive approach reulted in five high-level data fabrication characteristics, as depicted in Table `r tabnr`. The first characteristic of data fabrication, taking preparatory measures, included various things researchers did to prepare for data fabrication, including things such as reading about statistical methods to detect data fabrication, reading about previous data fabrication cases, or discussing with others how to manipulate data. Second, using a random number generator (RNG) encompasses the use of simulations or adding noise to data. Third, using real Stroop data includes reusing data that are freely available online or from previous experiments. Fourth, duplicating or transforming data, includes behaviors such as copy-pasting rows of data or creating a score on another condition based on a simple transformation of the scores on the other condition, guaranteeing the presence of an effect. Finally, we considered the behavior of checking the data for detectability of being fabricated as the final characteristic of data fabrication.

<!-- Op zich een goed idee… maar twee dezelfde vectoren 10100 kunnen toch op een total verschillende manier data genereren. Persoonlijk zou ik het fijn vinden als dat snel dudielijk is

Meeer in het algemeen, en nog belangrijker, helpt het je te weten wleke van de 32 werd gebruikt, om het te detecteren? Maar goed, hier kom je later nog op terug, hoop ik.
 -->

## Analysis


The number of observable patterns is dependent on the number of characteristics available and increases exponentially ($2^k$, with $k$ being the number of characteristics). Hence, in the example with three characteristics, there are eight possible patterns. Consequently, some patterns are likely to remain unobserved if the number of cases is much less than the number of potential patterns (i.e., logical remainders; depicted as `?` in Table `r tabnr`). As such, we limited ourselves to five high-level characteristics of data fabrication strategies with 32 possible patterns, considering only 28 transcripts are available.

Another relevant aspect of truth tables, as depicted in Table `r tabnr` by `C`, is that of conflicting outcomes. Conflicting outcomes occur when one pattern occurs for two different cases, but yields different outcomes. For our case, that means that the same pattern results in both detection and non-detection of data fabrication. Typically, in csQCA, these cases are simply omitted in the analysis (conceptually comparable to listwise deletion) or omitted characteristics are inductively searched for that resolve the conflict [@rihoux2008]. We qualitatively investigate what might cause these conflicting outcomes and present results for both the original five characteristics and the potential additional characteristics in case of conflicting outcomes.

```{r, echo=FALSE}
tabnr <- tabnr + 1
```

We used the `R` package `QCA` [@r-core;@10.1016/j.jbusres.2007.01.002] for our QCA analysis (see [osf.io/XXXX]() for analysis script). More specifically, we used the outcomes of five different statistical methods to detect data fabrication [as presented in @], with the five characteristics mentioned in Table X as characteristics. We minimized the truth table using the enhanced Quine-McCluskey algorithm [@] for both detecting data as fabricated, and for fabricated data going undetected. As such, we initially conduct ten QCA's, with at most ten more in the case of conflicting outcomes in for all methods.
