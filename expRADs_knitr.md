
```
## Loading required package: permute
```

```
## This is vegan 2.0-7
```

```
## Loading required package: tcltk
```

```
## Loading required package: fda
```

```
## Loading required package: splines
```

```
## Loading required package: zoo
```

```
## Attaching package: 'zoo'
```

```
## The following object is masked from 'package:base':
## 
## as.Date, as.Date.numeric
```

```
## Loading required package: Matrix
```

```
## Loading required package: lattice
```

```
## Attaching package: 'fda'
```

```
## The following object is masked from 'package:graphics':
## 
## matplot
```

```
## Loading required package: fields
```

```
## Loading required package: spam
```

```
## Spam version 0.29-3 (2013-04-23) is loaded. Type 'help( Spam)' or 'demo(
## spam)' for a short introduction and overview of this package. Help for
## individual functions is also obtained by adding the suffix '.spam' to the
## function name, e.g. 'help( chol.spam)'.
```

```
## Attaching package: 'spam'
```

```
## The following object is masked from 'package:base':
## 
## backsolve, forwardsolve
```

```
## Loading required package: maps
```

```
## Attaching package: 'fields'
```

```
## The following object is masked from 'package:plotrix':
## 
## color.scale
```

```
## Loading required package: stats4
```

```
## Attaching package: 'stats4'
```

```
## The following object is masked from 'package:spam':
## 
## mle
```

```
## Attaching package: 'VGAM'
```

```
## The following object is masked from 'package:stats4':
## 
## coef
```

```
## The following object is masked from 'package:splines':
## 
## bs, ns
```

```
## The following object is masked from 'package:vegan':
## 
## calibrate
```

```
## The following objects are masked from 'package:stats':
## 
## case.names, coef, coefficients, df.residual, dfbeta, fitted,
## fitted.values, formula, hatvalues, poly, residuals, variable.names,
## weights
```

```
## The following object is masked from 'package:base':
## 
## identity, scale.default
```

```
## Attaching package: 'lme4'
```

```
## The following object is masked from 'package:nlme':
## 
## lmList, VarCorr
```

```
## The following object is masked from 'package:stats':
## 
## AIC, BIC
```


**Title:** Assessing the impact of perturbations on taxonomic biodiversity using a cross-community approach
--------------------------------------------------------
**Authors:** Sarah R. Supp and S. K. Morgan Ernest

**Affiliations:** Utah State University, Department of Biology and the Ecology Center
5305 Old Main Hill, Logan, UT 84322-5305

The authors declare no conflict of interest

**Corresponding author information:** Address: Sarah R. Supp, 5305 Old Main Hill, Logan, UT, 84322-5305; Email: sarah.supp@usu.edu



**Abstract:**
Ecologists use a wide variety of biodiversity metrics to study the abundance and distribution of species. While it is increasingly clear that researchers will need to forecast changes in biodiversity, ecology currently lacks a framework for understanding the natural background variability in biodiversity or how biodiversity patterns will respond under environmental change scenarios. The most commonly used biodiversity metrics include species composition, species abundance, species richness, and the species abundance distribution (SAD) that incorporates the metrics of species richness, abundance, and evenness. Together, these metrics are used to describe biodiversity across ecosystems and taxonomic groups, but their sensitivity to environmental changes is unknown. Using global-span data from small-scale terrestrial animal communities, we show that the SAD and species richness are generally resilient under a suite of artificial and natural manipulations.  In contrast, species composition and abundance responded readily to manipulation. Our results suggest that species richness and the SAD are poor indicators of change, perhaps because many systems display strong compensatory dynamics. An important next step in biodiversity research is to place experimental results in a realistic context with respect to levels of background variability in species richness and to further compare the response of different metrics to manipulations. 

**Keywords:** biodiversity, species abundance distribution, disturbance, resilience, community structure



**Introduction**
In an era of rapid natural and anthropogenic change, it is increasingly clear that ecology needs to do more than quantify biodiversity for a snapshot in time. Ecology must also be able to forecast changes in biodiversity for systems in flux (Thomas et al. 2004, Araujo & Rahbek 2006, Dawson et al. 2011). Predicting biodiversity in disturbed systems has several challenges, including the need to understand the network of processes driving biodiversity and the ability to predict changes of multiple components of biodiversity under global environmental change scenarios (Fisher et al. 2010, White et al. 2010). Disturbance itself is a fundamental process that can enhance or reduce biodiversity (Hooper et al. 2005, Dornelas et al. 2011). Since disturbance frequency and intensity (e.g. fire, flood, fragmentation) may be altered under global change scenarios (cites) a general framework understanding biodiversity response to perturbation is critical. 

Biodiversity is a multidimensional concept that can be measured with respect to many different foci, including taxonomic, genetic, phylogenetic, and functional (Magurran & McGill 2011). Even within one of these foci, researchers are often interested in multiple different aspects of diversity. For example, taxonomic diversity includes metrics that measure biodiversity as the number of species or individuals and metrics that describe how individuals are partitioned across species (Magurran 2004, Magurran & McGill 2011). The most commonly used metrics of taxonomic diversity include species composition, the number of individuals, species richness, and species evenness (Dornelas et al. 2011, Maurer & McGill 2011). The species abundance distribution (SAD) incorporates metrics of richness, abundance, and evenness and is used to describe community structure (Magurran & Henderson 2003, McGill et al. 2007, Ulrich et al. 2010). Each metric differs in how it describes diversity within a system, and thus each metric should differ in its sensitivity to disturbance and in its ability to detect community response (Dornelas et al. 2011).  Changes in one or more of these metrics may suggest fundamental shifts in the network of species interactions (e.g., Chase & Leibold 2003, Clark 2009) or in community structure (e.g., Magurran & Henderson 2003, Harte 2011). For example, the SAD may pick up important changes in the dominance structure within a community, but will not necessarily be sensitive to change in the density of individuals or species identity. For this reason, a better understanding of biodiversity response to disturbance should help ecologists choose metrics based on which provides the most useful information for the specific question or application, rather than ease of measurement.

A suite of studies has attempted to understand the consequences of decreasing taxonomic diversity on community and ecosystem structure, primarily by focusing on reductions in species richness (e.g., e.g. Naeem et al. 1995, Hector et al. 1999, Reich et al. 2012). However, observational studies suggest that, temporally, species richness appears to exhibit low background variability, at least in systems not obviously perturbed (Brown et al. 2001, Goheen et al.2005, Elmendorf & Harrison 2011). Even in disturbed systems, species richness has often been observed to be relatively insensitive to many perturbations (Chapin III et al. 2000, Hillebrand et al. 2008). This makes it unclear whether the magnitude of diversity reduction seen in experiments reflects diversity reductions that occur in nature in response to natural and anthropogenic perturbations.  Disturbance itself may play a fundamental role in driving biodiversity patterns (Dornelas et al. 2011), but a general understanding of the effects of disturbance on biodiversity remains poorly understood (Dornelas 2010, Murphy & Romanuk 2012, Chase & Knight 2013). The lack of a comprehensive understanding of how biodiversity responds to perturbations and whether all aspects of biodiversity are equally sensitive hinders the ability of researchers to predict the impacts of environmental changes on communities and ecosystems. 
  
Using a compilation of experimentally manipulated community-level data of terrestrial animal taxa from the published literature (Table S1), we evaluated if biodiversity metrics of species composition, total abundance (N), species richness (S), and the SAD respond to environmental change. This approach allows us to specifically address 1) whether community perturbations cause shifts in a suite of biodiversity metrics and 2) if community-level biodiversity-metrics exhibit different sensitivities to perturbations.	

**Methods**
*Database compilation*
We conducted a literature search using Google Scholar October 2011 – February 2012. Peer-reviewed articles that included data tables that reported species-level abundance for a control community and at least one manipulated community were recorded. Published data was often summed or averaged over replicates, rather than reporting abundance separately for each replicate. The data were recorded from a wide variety of sites including manipulated, artificial experiments (i.e., caged exclosures, habitat modules, nutrient addition) and human-mediated “natural” experiments (i.e., controlled burn, silvicultural treatment, grazed plots). Sites represent all continents except Antarctica, and widely varying terrestrial animal taxa (e.g., zooplankton, arachnid, mammal, bird). The data were recorded in linked tables describing the reference, site, experiment, and community details (Appendix A).  

*Data selection*
For analysis, we eliminated communities where > 10% of individuals were not identified to the species level or where the area sampled for paired control – experiment communities was unequal. We used data where raw abundance was reported as a summed total for each species or where mean abundance was reported across the replicates, excluding percent cover, biomass, and presence-only data. In rare cases where mean abundance was reported using less than symbols (e.g. < 0.01) we assumed the value was at the top of that bin. SADs are difficult to characterize when the number of species or total abundance is very low, so we included only communities with S ≥ 5 and N ≥ 30. We compared pairs of communities at sites that were sampled at the same spatial scales and at similar temporal scales (e.g., we did not compare data from different seasons or across a time-series) to avoid complications due to differences in sampling intensity or timing (Gotelli & Colwell 2001, Magurran 2004). Data meeting the criteria was comprised of 59 control and 113 experiments (0 sites were compared both as control and experiment), representing 115 paired control-experiment comparisons from 41 published papers. Species richness ranged 5-189 and total abundance ranged 30.3-6483.

*Characterizing and comparing paired communities*
For each paired community, we compared the relative rank abundance distributions (RAD), species composition, total abundance, and species richness (for plots of all comparisons, Appendix B). RADs are an alternate visualization to SADs where the relative abundance of each species in the community is ordered from most abundant to least abundant. The RAD uses relative abundances and thus minimizes the impacts on the distribution caused primarily by change in total abundance, and also minimizes the information lost using histogram binning methods, especially in smaller communities (McGill et al. 2007).

We used the Bray-Curtis dissimilarity metric (BC) to quantify differences between controls and experiments for each of our biodiversity metrics (vegan, function vegdist; Oksanen et al. 2010). Bray-Curtis dissimilarity is a semi-metric index that provides a dissimilarity measure ranging from 0 (two communities are the same) to 1 (completely different). It is commonly used to examine similarity of ecological communities. When used to examine species composition or the RAD, it takes into account the presence/absence of a given species or rank across the two communities, but also the relative abundance of each species or rank. We also characterized RADs using Simpson’s evenness (J), which describes how similar species are in their abundances and is somewhat independent of S and N (Magurran 2004, McGill 2011; vegan, function diversity; Oksanen et al. 2010). For other biodiversity metrics, S and N, we calculated the BC dissimilarity and percent difference for each control-experiment community pair.

This research is not focused on which model fits empirical distributions best, but we compared the performance of the log-series to the Poisson lognormal distribution, which is often considered a superior model for describing SADs (Preston 1948, McGill et al. 2007, Ulrich et al. 2010) compared to the log-series, an alternate model (Fisher et al. 1943, Harte 2011). We used methods following White et al. (2012) to indicate the relative probability that one distribution best describes each empirical abundance distribution.

*Statistical analysis*
To compare measures of relative abundance at each rank (a proxy for the shape of the rank abundance distribution), Simpson’s evenness, total abundance, and species richness, we calculated fit of values to the 1:1 line (R2), which represents no change in values from control to experimental manipulation (Fig. 1). We also calculated root mean squared error (rmse), which is used to obtain the standard deviation of model prediction error, where lower values indicate better performance. Here, we used the control data as our “observed” and the experimental data as our “predicted” data in order to determine the degree of change, or variance between N, S, and evenness at paired sites (package hydroGOF, function rmse; Zambrano-Bigiarini 2011).

To determine the explanatory influence of species composition and community-level S and N on observed variation in the form of paired rank abundance distributions, we standardized all the data to make it compatible for statistical analysis and used standardized parameters in a variance-partitioning framework with multiple regression (Legendre and Legendre 2012) to determine the relative importance of composition and of community-level S and N in explaining the observed variation among paired RADs. We analyzed the data using both standardized BC dissimilarity in S and N and standardized absolute percent difference in S and N to avoid bias in the metric of difference chosen, since there is not a well-recognized way to characterize differences in S and N across disparate communities. We performed the analysis using all the data (Table 1), and using a smaller subset of the data including only communities with N >= 300 (n = 53, pairs = 37) to avoid bias by including communities which were more likely to be under sampled (McGill 2003), by including experimental type and taxonomic group as predictors for observed variation in the rank abundance distribution (Appendix C). Data and all necessary code for replicating the results are available online  and in the Supplement. 

**Results**
All communities experienced compositional differences between compared manipulated and control sites (Fig 1a, Fig 2a; R2=0.3615, rmse=0.0552, BC values ranged 0.105-0.994). Many communities experienced a change in total abundance (Fig 1b, Fig 2b; R2=0.4234, rmse=1021.7701; BC values ranged 0-0.795). Most communities experienced relatively small magnitude change in species richness (Fig 1c, Fig 2c; R2=0.7701, rmse=15.5407, BC values ranged 0-0.484). Change in the abundance at each rank for paired RADs (Fig1e, Fig 2e; R2=0.8098, rmse=0.0333, BC values ranged 0.062-0.502) and in evenness (Fig 1d, Fig 2d; R2=0.549, rmse=0.1207, BC values ranged 0.003-0.633) were also generally small magnitude. 
	
Although we were not explicitly testing RAD fit to a specific model, we found that nearly all our communities were best described by the log-series (n=147), rather than the lognormal, distribution (n=7). Communities reporting mean abundance could not be weighted using our function (n=18).  Although fit to lognormal distribution may indicate that that a community has been well-sampled (Preston 1948, McGill et al. 2007, Ulrich et al. 2010), other models predict the log-series distribution (Fisher et al. 1943, Harte 2011). Our finding is consistent with White et al. (2012), who also found that log-series was a good descriptor of communities across a wide range of taxonomic groups and ecosystems.  

Variance partitioning analysis suggested that composition and community-level S and N explained little of the observed variation among paired RADs; results were qualitatively similar for both metrics of S and N change used. Results were qualitatively similar when the analysis was restricted to only communities with N >= 300 (Table C1). Taxonomic group and experiment type were relatively uninformative for predicting RAD response to change (Table C2).

####**Discussion**
  Across a wide range of taxonomic groups, ecosystems, and experimental treatments, community perturbations caused shifts in a suite of biodiversity metrics, but metrics exhibited different sensitivities to perturbations. Measures of community structure, especially the rank abundance distribution and species richness, demonstrated low magnitude responses to disturbance, whereas species composition and total abundance responded readily to disturbance. The small magnitude of changes observed in species richness and the rank abundance distribution suggests that they are relatively insensitive to disturbance, including perturbations that most ecologists would agree constitute as “major” changes to a system (e.g., wildfire, clear-cuts). Although disturbance often has an important impact on the identity, abundance and distribution of species (e.g., Chase & Leibold 2003, Clark 2009), even large changes in composition and abundance often had little or no influence on species richness or on the shape of the abundance distribution. Since changes in species composition may influence the kind of diversity in which land managers are interested (e.g., functional diversity [Prinzig et al. 2008, Tilman et al. 1997], phylogenetic diversity [Mace et al. 2003, Webb et al. 2002] and ecosystem function [Flynn et al. 2011, Hooper & Vitousek 1997]) while having little effect on species richness or SAD shape, we suggest that these metrics are poor indicators for change within a system or of escalating disturbance impact. Until species richness and the SAD are better understood in a dynamic context, these metrics may play a more valuable role in conservation biology as static descriptors of community structure or by setting a baseline for biodiversity monitoring.

Compensatory dynamics may be an important mechanism influencing the generally low magnitude of changes in richness and community structure mitigating the effects of species loss in compositionally reorganized systems in our study. If sites maintain adequate connectivity with regional species pools that enable compensatory dynamics or if the species pool is relatively large (Chao & Jost 2012), high magnitude changes in species richness and the SAD may be relatively rare (e.g., Ernest & Brown 2001, Gonzalez & Loreau 2009, Dornelas 2010). Because species richness and the form of the SAD are relatively resilient to disturbance, and thus may be sensitive to larger-scale regional changes, we suggest that cases in which high magnitude shifts do occur may indicate fundamental changes in specific processes within a system that warrant further study and attention. Critical conservation decisions for threatened areas are often made based on continuing function of ecosystem services (e.g., Chan et al. 2006, Nelson et al. 2009), which in turn are often dependent on maintaining specific biological interactions. As such, the details of biotic interactions are often quite important and high magnitude changes in species composition and abundance cannot be ignored. 

Although species richness is often used to quantify the influence of disturbance on a community or ecosystem (Costello et al. 2004, Dornelas et al. 2011), our results and others (e.g., Chapin III et al. 2000, Hillebrand et al. 2008) suggest that species richness is often surprisingly insensitive to the changes applied to a system. Decades of diversity experiments have manipulated species richness to understand the impacts of species gain or loss on ecosystems (e.g. Naeem et al. 1995, Hector et al. 1999, Reich et al. 2012), but ecologists still generally lack an understanding of the existing background variability of species richness at natural sites, the magnitude of changes that occur in response to disturbance, or what magnitude of change in richness is biologically significant. In our analysis, only one site experienced more than a twofold change in species richness. This raises the important question of what diversity experiments actually reveal about ecological response to disturbance if the magnitude of species richness change studied in these systems is often much larger than what is empirically observed.

A major challenge facing biodiversity research is to bridge the existing gap between basic and applied ecological research. Our results suggest that biodiversity response to disturbance is complex and highly dependent on which component of biodiversity is being studied. More research is needed to evaluate the sensitivity of different biodiversity metrics to environmental change and the background variability in biodiversity in relatively undisturbed systems in order to develop a dynamic framework for better prediction. Future research placing biodiversity experiments in the context of realistic rates of change in ecological time is an important next step forward. 	

###**Acknowledgements.** We thank E.P. White, P.B. Adler, D.N. Koons, M.E. Pfrender, B.J. McGill, and the Weecology Group at Utah State University for their statistical advice and discussions that greatly improved the manuscript.  We thank all the authors who collected and published the data. SRS was supported by USU Ecology Center and School of Graduate Studies fellowships.

Figures and Tables:
-------------------

**Figure 1.** Panel of 1:1 plots with R2 for a) species composition relative abundance b) total abundance, c) species richness, d) rank evenness, and d) relative abundance at each rank of the RAD. Control data is on the x-axis and experimental data is on the y-axis. Fit to the 1:1 line (dashed line) suggests no change in the parameter among the paired control-experiment comparison. 

![plot of chunk unnamed-chunk-2](figure/unnamed-chunk-2.png) 


**Figure 2.** Panel showing the change in the four parameters among the paired control-experiment sites: a) Bray-Curtis dissimilarity in species composition, b) absolute percent change in total abundance, c) absolute percent change in species richness, d) Bray-Curtis dissimilarity of rank evenness, and e) Bray-Curtis dissimilarity of the relative abundance at each rank for compared RADs. 

![plot of chunk unnamed-chunk-3](figure/unnamed-chunk-3.png) 
