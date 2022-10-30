## FOR BIOL3207_ASSIGNMENT#2
BY Yusheng Wang

---

## VERSION HISTORY

V2.1:
Finish proofread.
Re-write the README file
Debug: 1. Remove the problem .bib file; 2. Correct spelling errors.

V1.2: 
Add references and the README file. 
Change some sub-title. 
Debug: 1. Change "InRR" to "lnRR"; 2. Repair references list; 3. Correct spelling errors.
wait for the final proofread.

V1.1: 
Finish all the task. 
Wait for references and a README file.

V1.0: 
Finish all coding part. 
Wait for adding some interpretations.

V0.3: 
Finish to task#9.

V0.2: 
Finish to task#4.

V0.1: 
Start the work, set up this repository and add the original data files.


---

## ABOUT

The goal of this work is to conduct a meta-analysis on ocean acidification effects on behaviour. I explore the publication bias over the past decade regarding direct effects of ocean acidification on fish behavior. By reviewing and meta-analysing of 92 studies empirically testing effects of ocean acidification on fish behavior, I provide quantitative evidence that the research to date on this topic is characterized by a decline effect, where large effects in initial studies have all but disappeared in subsequent studies over a decade. It suggest that the initial studies could be particular cases.

---

## CONTENT

The ".rmd" file is the main coding files, which can do some certain meta-analyses process.

The "raw_data" floder includes original data from [Clark et al., 2020](https://doi.org/10.1038/s41586-019-1903-y) and meta-data from other 91 studies, which will be used as a data resource.

The "out_data" floder includes outcome meta-data of these codes.

The "README" file includes some instructions.

The ".html" file is the output markdown of ".rmd" file.

The ".Rproj" file help you set the work direction.

The ".gitignore" file includes direction that not be tracked.

---

## HOW TO USE

The fist step, put existing meta-data (from 91 studies here) into the "raw_data" file. The detailed meta-data for each column are as follows:

| Column Name | Description|
| - | - |
| Obs | Observation|
| Study | Code for each individual study|
| Authors | Authors of each paper|
| Year (online) | Year the final paper was made available online|
| Year (print) | Year the final paper was included in a journal volume/issue|
| Title | Title of each paper|
| Pub year IF | The journal impact factor for the year the paper was published; obtained from InCites Journal Citation Reports|
| 2017 IF | The journal impact factor for 2017 (i.e., most recent journal impact factor); obtained from InCites Journal Citation Reports|
| Average n | Average sample size for the study; average of indiviudal sample sizes for the contol and experimental groups|
| Effect type | The type of effect concluded by the study regarding the effect of OA on behaviour; strong, weak, or no effect (see Supplementary Methods for details)|
| Species | The species used in each individual experiment|
| Climate (FishBase) | Climatic region for each species; obtained from FishBase|
| Env cue/stimulus? | Whether or not the experiment included a cue or stimulus in the experiment (olfactory, visual, auditory, or physical)|
| Cue/stimulus type | The type of cue or stimulus used|
| Behavioural metric | The specific measure of behaviour tested|
| Life stage | Life stage of the fish tested|
| ctrl.n | Sample size of the control group|
| ctrl.mean | Mean of the control group|
| ctrl.sd | The standard deviation of the control group, calculated from ctrl.vartype|
| oa.n | Sample size of the experimental group|
| oa.mean | Mean of the experimental group|
| oa.sd | The standard deviation of the experimental group, calculated from ctrl.vartype|
| lnRR | Raw effect size (natural log transformed response ratio)|
| lnRR_V | Sampling variance of lnRR|

The second step, put the new data ([Clark et al., 2020](https://doi.org/10.1038/s41586-019-1903-y) here) you want to add to meta-data in the first step into the "raw_data" file. The detailed meta-data for each column are same as above.

P.S. If you use other data, please DO NOT change the original file name.

Finally, knit the ".rmd" file.

In this meta-analyses, I first do some data cleansing to merge data from [Clark et al., 2020](https://doi.org/10.1038/s41586-019-1903-y) here) with the format. Then, I do some overall meta-analyses to calculate the effect sizes and heterogeneity analyses among the 92 studies. Finally, I identify some potential publication bias in these studies and give some views on early research in this field.

---

## READ RESULTS

1. The "metadata.csv" in direction "./out_data" is processed 92-study meta-data removed irrelevant and missing value from original data. 

2. The "lnRR_metadata.csv" in direction "./out_data" is 92-study meta-data with effect size "lnRR" and sampling variance "lnRR_V". 

3. The ".html" file shows results and interpretatiions of each step of the process.
