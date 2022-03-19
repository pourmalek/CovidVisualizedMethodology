
****************************************************************************************
****************************************************************************************
****************************************************************************************


# CovidVisualized Methodology Document Appendix


Methodology document appendix for CovidVisualized tools: [`CovidVisualizedGlobal`](https://github.com/pourmalek/CovidVisualizedGlobal), [`CovidVisualizedCountry`](https://github.com/pourmalek/CovidVisualizedCountry), and [`covir2`](https://github.com/pourmalek/covir2)

CovidVisualized: Visualized compilation of international updating models estimates of COVID-19 pandemic at global and country levels

Appendix: Examples of what the CovidVisualized tools provide in addition to the individual models

Farshad Pourmalek, MD PhD
Former lecturer, University of British Columbia, Vancouver, Canada
pourmalek_farshad at yahoo dot com


<br/><br/>


### TABLE OF CONTENTS:

[Summary](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#summary-1)

[CovidVisualized tools](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#covidvisualized-tools-1)

[The five international and periodically updated COVID-19 pandemic models](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#the-five-international-and-periodically-updated-covid-19-pandemic-models-are)

[Examples of what the CovidVisualized tools provide in addition to the individual models](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#examples-of-what-the-covidvisualized-tools-provide-in-addition-to-the-individual-models)

[References](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#references-1)

[Example 1: Iran](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#example-1-iran)

[Example 2: Canada and its province](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#example-2-canada-and-its-province)

[Example 3: Global level and WHO regions](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#example-3-global-level-and-who-regions)

[Postscript](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#postscript)

<br/><br/>


### Summary

This CovidVisualized Methodology Document Appendix provides examples of how the CovidVisualized tools can be used to examine the predictions by the international and periodically updated epidemic models for the future trajectory of the COVID-19 pandemic at global and country levels. These examples first explain what a researcher or advisor to policymakers would need to do to find and compile those predictions and what the results may look like. The examples then describe what can be found on the CovidVisualized websites. The main issue is that not all the models provide graphs (and data) of daily deaths and daily cases or infections – the minimum indicators of the future trajectory. Not all the models provide graphs (and data) for the global and regional levels. The conclusion is straightforward: If anyone ever tries to find and examine the predictions by the international and periodically updated epidemic models for the future trajectory of the COVID-19 pandemic, they will notice the obstacles. The CovidVisualized tools have already paved the way and resolved the barriers in examining the predictions in a coherent, consistent, and periodically updated framework, with underlying software codes and outputs. 


<br/><br/>

### CovidVisualized tools: 

There are three CovidVisualized tools:

(1) CovidVisualizedGlobal: Combine and visualize international and periodically updated predictions of COVID-19 pandemic at the global level and six WHO regions https://github.com/pourmalek/CovidVisualizedGlobal 

(2) CovidVisualizedCountry: Combine and visualize international and periodically updated predictions of COVID-19 pandemic at the country level: Canada, national and subnational https://github.com/pourmalek/CovidVisualizedCountry 

(3) covir2: Combine and visualize international and periodically updated predictions of COVID-19 pandemic at the country level, countries without subnational level estimates: Iran
https://github.com/pourmalek/covir2



<br/><br/>

### The five international and periodically updated COVID-19 pandemic models are:

(1) DELPHI, Massachusetts Institute of Technology, Cambridge (abbreviation used in this work: DELP) [1], 

(2) Institute for Health Metrics and Evaluation, Seattle (IHME) [2], 

(3) Imperial College, London (IMPE) [3], 

(4) Los Alamos National Laboratories, Los Alamos (LANL) [4], and 

(5) University of Southern California, Los Angeles, by Srivastava, Ajitesh (SRIV) [5]. 



<br/><br/>

### Examples of what the CovidVisualized tools provide in addition to the individual models

_Question:_ What is missing from the individual international and periodically updated models that creation of the CovidVisualized tool was needed?

_Answer:_ Nothing substantial is missing from the individual (international and periodically updated) models. However, some of those models do not report predictions of daily outcomes or do not provide the predictions at the global or regional levels. Suppose that a researcher or advisor to policymakers wants to look at the latest predictions by all international and periodically updated models for any given country or location (e.g., Canada and its provinces, or the European region). In that case, they need to know or find the website addresses for graphs and data of each model, find the graphs that are available on the websites for the models, develop the graphs that are not available, and put together and examine the graphs that use different horizontal (time) and vertical (outcome) axes. If they want to repeat this, they will need to repeat all the steps, which is time-consuming. The CovidVisualized tools have consistently performed the steps mentioned above and compiled the graphs (and data) from individual models together in a usable framework and continue to do so regularly. 

**The obstacles:** The obstacles one would encounter in examining the latest predictions by all international and periodically updated models for any given country or location are mentioned below. (1) The DELP model does not provide predictions of daily deaths and daily cases. One needs to calculate them from the provided total deaths and total cases. (2) The IMPE graphs for predicted daily deaths at the continent level and daily infections at the global and continent levels are not readily locatable. (3) The SRIV model does not provide global and continent-level graphs. (4) The researcher-made compilations of available graphs from different models are not practically usable because (a) the graphs from each model use different calendar time intervals and time bins, (b) the maximum value on the y-axis for the same outcome (e.g., daily deaths) are different across models, (c) uncertainty intervals and alternate scenarios are not shown by all the models. (5) Not all models provide graphs for all the variables they predict, e.g., hospital-related outcomes. (6) The predictions’ data files that each model provides follow that model’s unique data arrangements. These data arrangements differ across the models. Without a common data management template, it is impossible to acquire a grip on the models’ data that can lead to the creation of compiled data and graphs. 

Creation of the missing graphs and redeveloping the available graphs need a data management framework capable of compiling data (predictions’ files) from different models. While all the models present a set of common outcomes and variables, they do so in their unique way. The number of data files, the variables and data structure within each file, the nomenclature and variable names, the geographical locations covered by each model, the alternative scenarios, and many other aspects of the predictions provided by the models vary tremendously across the models. Moreover, within each model, there are systematic and random variations and alterations regarding these aspects across time (i.e., with updates released by the model). The CovidVisualized tools have covered these issues in a reproducible way, i.e., researchers can download the codes, rerun them, and see the outputs and results. 

_Conclusion:_ The CovidVisualized tools have already paved the way and resolved the obstacles in examining the predictions in a coherent, consistent, and periodically updated framework, with underlying software codes and outputs. 







<br/><br/>


### References:

1. COVID Analytics. DELPHI epidemiological case predictions. Cambridge: Operations Research Center, Massachusetts Institute of Technology. https://www.covidanalytics.io/projections and https://github.com/COVIDAnalytics/website/tree/master/data/predicted Accessed 23 June 2021. 
2. Institute for Health Metrics and Evaluation (IHME). COVID-19 mortality, infection, testing, hospital resource use, and social distancing projections. Seattle: Institute for Health Metrics and Evaluation (IHME), University of Washington. http://www.healthdata.org/covid/ and http://www.healthdata.org/covid/data-downloads Accessed 23 June 2021.
3. MRC Centre for Global Infectious Disease Analysis (MRC GIDA). Future scenarios of the healthcare burden of COVID-19 in low- or middle-income countries. London: MRC Centre for Global Infectious Disease Analysis, Imperial College London. https://mrc-ide.github.io/global-lmic-reports/ and https://github.com/mrc-ide/global-lmic-reports/tree/master/data Accessed 23 June 2021.
4. Los Alamos National Laboratory (LANL). COVID-19 cases and deaths forecasts. Los Alamos: Los Alamos National Laboratory (LANL). https://covid-19.bsvgateway.org Accessed 23 June 2021.
5. Srivastava, Ajitesh. University of Southern California (USC). COVID-19 forecast. Los Angeles: University of Southern California. https://scc-usc.github.io/ReCOVER-COVID-19 and https://github.com/scc-usc/ReCOVER-COVID-19/tree/master/results/historical_forecasts Accessed 23 June 2021.

***


<br/><br/>



Here are three examples illustrating what the CovidVisualized tools provide in addition to the individual models. 

[Example 1](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#example-1-iran) is for Iran. 

[Example 2](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#example-2-canada-and-its-province) is for Canada and its province.

[Example 3](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#example-3-global-level-and-who-regions) looks at the global level and WHO regions. 

For sample applications of “covir2” to countries without subnational estimates see [Afghanistan](https://github.com/pourmalek/covir2/tree/main/ADAPTATIONS_EXAMPLES/Afghanistan_%2020210625/20210625), [Pakistan](https://github.com/pourmalek/covir2/tree/main/ADAPTATIONS_EXAMPLES/Pakistan_20210704), [Japan 20210506](https://github.com/pourmalek/covir2/tree/main/ADAPTATIONS_EXAMPLES/Japan_20210506), [Japan 20210928](https://github.com/pourmalek/covir2/tree/main/ADAPTATIONS_EXAMPLES/Japan_20210928)



<br/><br/>

### Example 1: Iran

Here is a real-life example that explains what a researcher or advisor to policymakers would have needed to do if they wanted to examine the latest predictions by the international and periodically updated models for the future trajectory of the COVID-19 epidemic in Iran on March 7, 2022. 

To examine the latest predictions of daily deaths and daily cases in Iran by the international and periodically updated models, one needs to identify the models, locate their websites, find the graphs, create the missing graphs, (redevelop the existing graphs), and compile the graphs in a usable manner. I tried to replicate the above steps, and the results are presented below. Moreover, one needs to consider the relative strengths and weaknesses of each model, their past predictive performance profiles, and then interpret the collection of findings and predictions. The “Summary” provided at the end of the example addresses many of these considerations. 

<br/><br/>



DELP model

The DELP model does not present predictions of daily deaths and daily cases. They provide predictions of total deaths and total cases. See Appendix Graphs 1 and 2 below. 

***

Appendix Graph 1. Iran, Predicted total deaths, DELP model. || Source: https://covidanalytics.io/projections Accessed on March 7, 2022.

![image](https://user-images.githubusercontent.com/30849720/159106211-ac0ff4c7-4d53-4602-a496-636626c65b88.png)

*** 

Appendix Graph 2. Iran, Predicted total cases, DELP model. || Source: https://covidanalytics.io/projections Accessed on March 7, 2022.

![image](https://user-images.githubusercontent.com/30849720/159106159-c40e1656-3d81-4693-9306-74517afd35f5.png)
 
***




<br/><br/>

IHME model

The IHME model does not present predictions of daily cases. They provide predictions of daily infections. See Appendix Graphs 3 and 4 below. 


***

Appendix Graph 3. Iran, Predicted daily deaths, IHME model. || Source: https://covid19.healthdata.org/iran-(islamic-republic-of)?view=daily-deaths&tab=trend Accessed on March 7, 2022.

![image](https://user-images.githubusercontent.com/30849720/159106222-af6cbab2-d625-4b82-8346-466571b2319d.png)
 
***

Appendix Graph 4. Iran, Predicted daily infections, IHME model. || Source: https://covid19.healthdata.org/iran-(islamic-republic-of)?view=infections-testing&tab=trend&test=infections Accessed on March 7, 2022.

![image](https://user-images.githubusercontent.com/30849720/159106231-2ede0875-de7e-4716-ad23-36a3e2932171.png)
 
***



<br/><br/>

IMPE model

The IMPE model does not present predictions of daily cases. They provide predictions of daily infections. See Appendix Graphs 5 and 6 below. 


***

Appendix Graph 5. Iran, Predicted daily deaths, IMPE model. || Source: https://raw.githubusercontent.com/mrc-ide/global-lmic-reports/master/IRN/index.pdf Page 4. Accessed on March 7, 2022.

![image](https://user-images.githubusercontent.com/30849720/159106240-ba42a5fb-78be-4895-b6eb-8106f874d9b2.png)

***
 
Appendix Graph 6. Iran, Predicted daily infections, IMPE model. || Source: https://raw.githubusercontent.com/mrc-ide/global-lmic-reports/master/IRN/index.pdf Page 2. Accessed on March 7, 2022.

![image](https://user-images.githubusercontent.com/30849720/159106243-d594154c-e737-4d17-88ce-427883e0bb56.png)

***


<br/><br/>

LANL model

The LANL COVID-19 Team made its last real-time forecast on September 27th, 2021. || Source: https://covid-19.bsvgateway.org Accessed on March 7, 2022.






<br/><br/>

SRIV model

The SRIV model’s predictions for daily deaths and daily cases are shown in Appendix Graphs 7 and 8 below. 

***

Appendix Graph 7. Iran, Predicted daily deaths, SRIV model.|| Source: https://scc-usc.github.io/ReCOVER-COVID-19 Accessed on March 7, 2022.

![image](https://user-images.githubusercontent.com/30849720/159106256-e637e646-e97e-4c7d-a832-f3d94f7b121f.png)
 
***

Appendix Graph 8. Iran, Predicted daily cases, SRIV model|| Source: https://scc-usc.github.io/ReCOVER-COVID-19 . Accessed on March 7, 2022.

![image](https://user-images.githubusercontent.com/30849720/159106264-fc0a0606-6352-45fd-9eae-0c237b180a9a.png)
 
***





<br/><br/>

Johns Hopkins compilation of official reports

The Johns Hopkins compilation of official reports does not present daily deaths and daily cases (as of March 7, 2022). They provide weekly deaths and weekly cases. See Appendix Graphs 9 and 10 below. 

***

Appendix Graph 9. Iran, Weekly reported deaths, Johns Hopkins. || Source: https://www.arcgis.com/apps/dashboards/bda7594740fd40299423467b48e9ecf6 Accessed on March 7, 2022.

![image](https://user-images.githubusercontent.com/30849720/159106272-868f89ed-7eec-4a59-b92c-fe04e8c30db7.png)
 
***

Appendix Graph 10. Iran, Weekly reported cases, Johns Hopkins. || Source: https://www.arcgis.com/apps/dashboards/bda7594740fd40299423467b48e9ecf6 Accessed on March 7, 2022.   

![image](https://user-images.githubusercontent.com/30849720/159106275-4412abeb-dbd4-4d7d-a138-29ef8596ebe1.png)

***






<br/><br/>

Worldometers compilation of official reports to WHO

The Worldometers compilation of official reports provides daily deaths and cases, shown in Appendix Graphs 11 and 12 below. 

***

Appendix Graph 11. Iran, Daily deaths, Worldometers. Accessed on March 7, 2022. https://www.worldometers.info/coronavirus/country/iran/ 
 
![image](https://user-images.githubusercontent.com/30849720/159106306-cff25ccf-7bb8-45d0-806b-92d1ac767e1e.png)

***

Appendix Graph 12. Iran, Daily cases, Worldometers. Accessed on March 7, 2022. https://www.worldometers.info/coronavirus/country/iran/ 

![image](https://user-images.githubusercontent.com/30849720/159106312-8f8c75b0-120d-42da-b123-8a4fc8de18cc.png)

***


<br/><br/>

**Compile the graphs from individual models

The DELP model does not present predictions of daily deaths and daily cases. Predictions of daily deaths by IHME, IMPE, and SRIV and reported daily deaths by Worldometers are shown below in Appendix Graph 13. Appendix Graph 14 shows the predicted daily cases by SRIV, predicted daily infections by IHME and IMPE, and the reported daily cases by Worldometers. 

 
***

Appendix Graph 13. Iran predicted daily deaths by IHME, IMPE, SRIV and reported daily deaths by Worldometers. Accessed on March 7, 2022. || Source: Assembled from Appendix Graphs 3, 5, 7, and 11.

![image](https://user-images.githubusercontent.com/30849720/159106324-1e9a188f-84ea-4a74-9ac6-3868fdda60a6.png)

*** 

Appendix Graph 14. Iran, predicted daily cases by SRIV, predicted daily infections by IHME and IMPE, and reported daily cases, Worldometers. Accessed on March 7, 2022. || Source: Assembled from Appendix Graphs 4, 6, 8, and 12.

![image](https://user-images.githubusercontent.com/30849720/159106329-5894d9e9-719a-466b-a129-e2105eddb086.png)
  
***

<br/><br/>

**How** can the covir2 tool be practically used for the example of a researcher or advisor to policymakers who wanted to examine the latest predictions for the future trajectory of the COVID-19 epidemic in Iran on March 7, 2022? They would look at the uptake dates on the covir2 website to find the latest date equal to or before March 7, 2022. The uptake dates in the covir2 website are displayed on the top of the main web page as the names of directories for each uptake (see Appendix Exhibit 1 below). Scroll down to find the latest uptake date equal to or before March 7, 2022. Appendix Exhibit 2 shows that the date would be 20220304. Clicking on the hyperlinked name 20220304 leads to the page for the uptake 20220304 (see Appendix Exhibit 3). On the page for the uptake 20220304, “Selected graphs” can be viewed, as well as links to the code  used to produce the results and the output  of the code. 


<br/><br/>

Appendix Graphs 15 to 33 (below) show what can be found for uptake 20220304 on the covir2 website. Official reports by the country are demonstrated as the curves drawn from the Johns Hopkins University compilation (abbreviated in the graphs as “JOHN”). 

Appendix Graph 15 shows all models’ predictions by all models for Daily deaths, all-time, i.e., from January 2020 to the latest date available in the models. Appendix Graph 16 focuses on more recent times, i.e.,  2021 on. Appendix graphs 17 and 18 look in more detail at the IHME model predictions. Appendix Graph 17 shows predicted Daily deaths, 2021 on, reference scenario with uncertainty, IHME, and Appendix Graph 18 shows predicted Daily deaths, 2021 on, all scenarios, IHME. Appendix graphs 19 and 20 look in more detail at the IMPE model predictions. 

For the second outcome, i.e., daily cases, Appendix Graph 21 shows the predicted Daily cases or infections, all-time, and Appendix Graph 22 shows the predicted Daily cases or infections, 2021 on. Appendix Graph 23 demonstrates the predicted Daily cases, 2021 on, without the predicted infections. The values of the predicted infections are much higher than those for the predicted cases. When in the same graph, infections’ curves visually compress the cases’ curves. When the predicted cases are shown without the predicted infections, one can appreciate their trajectory and compare them with the past trends. 

Appendix Graphs 24 to 33 demonstrate additional outcomes and variables. Appendix Graph 24 depicts the secondary (i.e., calculated) variable Daily estimated infections IHME, IMPE to reported cases JOHN, main scenarios, 2021 on. This graph provides a gauge of how much more are the predicted infections compared with predicted cases, across time and models – a technical epidemiological and modelling insight. This graph does not have a readily accessible similar on the web, as far as I know. 

Appendix Graphs 25 and 26 provide predicted hospital-related outcomes. Appendix Graph 25 shows all the Hospital-related outcomes, all-time and by all models. Appendix Graph 26 removes the outcomes whose larger values compress the curves of outcomes with lower values and focuses on more recent time interval. There are no readily accessible similar graphs on the web as far as I know. 

Appendix Graph 27 depicts how many times more are the precited deaths compared with the reported deaths across time and models. Appendix Graph 28 shows a similar secondary (i.e., calculated) variable for the cases or infections – a technical epidemiological and modelling insight, with no ongoingly updated similar graphs on the web as far as I know.

Appendix Graphs 29 to 33 show additional variables estimated by the IHME model: Appendix Graph 29, R effective, 2 scenarios, 2021 on, IHME; Appendix Graph 30, Daily Infection-outcome ratios, 2 scenarios, 2021 onwards, IHME; Appendix Graph 31, Daily mobility, 2 scenarios, all-time, IHME; Appendix Graph 32, Daily mask use, 2 scenarios, all-time, IHME; and Appendix Graph 33, Percent cumulative vaccinated, 2021 on, IHME.


<br/><br/>

**Here is** the bottom-line conclusion from this example of a researcher or advisor to policymakers who wanted to examine the latest predictions for the future trajectory of the COVID-19 epidemic in Iran on March 7, 2022 – and how the covir2 tool can help. One can locate the latest predictions by the international and periodically updated models and come up with some sort of compilation of graphs like the Appendix Graphs 13 and 14 made here, or similar graphs for other outcomes. In the meantime, the Appendix Graphs 15 to 23 are equivalent to those graphs' compilations, readily available via the covir2 tool. The latter graphs are much more usable and demonstrate different aspects like calendar time intervals, different scenarios, mean estimates and confidence intervals, and individual models’ details. The software code used to produce the graphs is accessible  and can be rerun by others to verify the correctness and potential mistakes. The track record of the previous periodical uptakes is also accessible (via RESULTS 2021 and RESULTS 2022 for covir2, for instance). The covir2 uptake 20220311 also adds the following summary by its creator, and puts all the graphs in “Iran COVID-19 epidemic models situation report No 48 – 2022-03-11.pdf”.

<br/><br/>

**Summary 20220311:

![image](https://user-images.githubusercontent.com/30849720/159106354-c1f40cf1-93b8-4634-ab28-ef2f3858f7fe.png)

 
The New Year ceremonies and travels increase the number of contacts and the probability of transmission and spread of the virus across the country. These factors are not fully included in the models. As such, _a new surge_ could be expected in Iran in March and April.



***

Appendix Exhibit 1. The uptake dates in the covir2 website are displayed on the top of the main web page as the names of directories for each uptake. || Source: https://github.com/pourmalek/covir2 Accessed on March 7, 2022.

![image](https://user-images.githubusercontent.com/30849720/159106362-6024a173-391a-47f2-8ba2-de606c88104b.png)
 
***

Appendix Exhibit 2. The latest uptake date equal to or before March 7, 2022, is 20220304.
|| Source: https://github.com/pourmalek/covir2 Accessed on March 14, 2022.

![image](https://user-images.githubusercontent.com/30849720/159106367-0d5c68f3-f93e-45ef-a474-ec40359582a5.png)
 
***

Appendix Exhibit 3. The covir2 website page for uptake 20220304. || Source: https://github.com/pourmalek/covir2/tree/main/20220304 Accessed on March 7, 2022.

![image](https://user-images.githubusercontent.com/30849720/159106373-0e88b31a-c8c9-4438-94c5-94ecc838e219.png)

*** 

Appendix Graph 15. [Daily deaths, all-time](https://github.com/pourmalek/covir2/blob/main/20220304/output/merge/graph%2012%20COVID-19%20daily%20deaths%2C%20Iran%2C%20reference%20scenarios.pdf) || Source: [`covir2 uptake 20220304`](https://github.com/pourmalek/covir2/tree/main/20220304) Accessed on March 7, 2022.

![image](https://user-images.githubusercontent.com/30849720/157358108-10b1fa59-f944-4fc4-af88-186f02016cc0.png)

***
 
Appendix Graph 16. Iran Daily deaths, 2021 on ||  Source: [`covir2 uptake 20220304`](https://github.com/pourmalek/covir2/tree/main/20220304) Accessed on March 7, 2022.


***
 
Appendix Graph 17. Iran Daily deaths, 2021 on, reference scenario with uncertainty, IHME ||  Source: [`covir2 uptake 20220304`](https://github.com/pourmalek/covir2/tree/main/20220304) Accessed on March 7, 2022.

***
 
Appendix Graph 18. Iran Daily deaths, 2021 on, all scenarios, IHME ||  Source: [`covir2 uptake 20220304`](https://github.com/pourmalek/covir2/tree/main/20220304) Accessed on March 7, 2022.


***
 
Appendix Graph 19. Iran Daily deaths, 2021 on, reference scenario with uncertainty, IMPE ||  Source: [`covir2 uptake 20220304`](https://github.com/pourmalek/covir2/tree/main/20220304) Accessed on March 7, 2022.


***
 
Appendix Graph 20. Iran Daily deaths, 2021 on, 3 scenarios, IMPE ||  Source: [`covir2 uptake 20220304`](https://github.com/pourmalek/covir2/tree/main/20220304) Accessed on March 7, 2022.


***
 
Appendix Graph 21. Iran Daily cases or infections, all-time ||  Source: [`covir2 uptake 20220304`](https://github.com/pourmalek/covir2/tree/main/20220304) Accessed on March 7, 2022.


***
 
Appendix Graph 22. Iran Daily cases or infections, 2021 on ||  Source: [`covir2 uptake 20220304`](https://github.com/pourmalek/covir2/tree/main/20220304) Accessed on March 7, 2022.


***
 
Appendix Graph 23. Iran Daily cases, 2021 on ||  Source: [`covir2 uptake 20220304`](https://github.com/pourmalek/covir2/tree/main/20220304) Accessed on March 7, 2022.


***
 
Appendix Graph 24. Iran Daily estimated infections IHME, IMPE to reported cases JOHN, main scenarios, 2021 on ||  Source: [`covir2 uptake 20220304`](https://github.com/pourmalek/covir2/tree/main/20220304) Accessed on March 7, 2022.


***
 
Appendix Graph 25. Iran Hospital-related outcomes, all-time ||  Source: [`covir2 uptake 20220304`](https://github.com/pourmalek/covir2/tree/main/20220304) Accessed on March 7, 2022.


***
 
Appendix Graph 26. Iran Hospital-related outcomes, 2021 on ||  Source: [`covir2 uptake 20220304`](https://github.com/pourmalek/covir2/tree/main/20220304) Accessed on March 7, 2022.


***
 
Appendix Graph 27. Iran Daily deaths estimated to reported, all-time ||  Source: [`covir2 uptake 20220304`](https://github.com/pourmalek/covir2/tree/main/20220304) Accessed on March 7, 2022.


***
 
Appendix Graph 28. Iran Daily cases or infections estimated to reported cases, 2021 on ||  Source: [`covir2 uptake 20220304`](https://github.com/pourmalek/covir2/tree/main/20220304) Accessed on March 7, 2022.


***
 
Appendix Graph 29. Iran R effective, 2 scenarios, 2021 on, IHME ||  Source: [`covir2 uptake 20220304`](https://github.com/pourmalek/covir2/tree/main/20220304) Accessed on March 7, 2022.


***
 
Appendix Graph 30. Iran Daily Infection-outcome ratios, 2 scenarios, 2021 on, IHME ||  Source: [`covir2 uptake 20220304`](https://github.com/pourmalek/covir2/tree/main/20220304) Accessed on March 7, 2022.


***
 
Appendix Graph 31. Iran Daily mobility, 2 scenarios, all-time, IHME ||  Source: [`covir2 uptake 20220304`](https://github.com/pourmalek/covir2/tree/main/20220304) Accessed on March 7, 2022.


***
 
Appendix Graph 32. Iran Daily mask use, 2 scenarios, all-time, IHME ||  Source: [`covir2 uptake 20220304`](https://github.com/pourmalek/covir2/tree/main/20220304) Accessed on March 7, 2022.


***
 
Appendix Graph 33. Iran Percent cumulative vaccinated, 2021 on, IHME ||  Source: [`covir2 uptake 20220304`](https://github.com/pourmalek/covir2/tree/main/20220304) Accessed on March 7, 2022.
 

***












<br/><br/>

### Example 2: Canada and its province

Below is a real-life example that explains what a researcher or advisor to policymakers would have needed to do if they wanted to examine the latest predictions by the international and periodically updated models for the future trajectory of the COVID-19 epidemic in Canada and its provinces and territories, on March 14, 2022. 

To examine the latest predictions of daily deaths and daily cases in Canada and its subnational levels by the international and periodically updated models, one needs to identify the models, locate their websites, find the graphs, create the missing graphs, (redevelop the available graphs), and compile the graphs. I tried to replicate the above steps, and the results are presented below. 



<br/><br/>

DELP model

The DELP model does not present daily deaths and daily cases predictions – they provide total deaths and total cases. The DELP model provides predictions for nine provinces: Alberta, British Columbia, Manitoba, New Brunswick, Newfoundland and Labrador, Nova Scotia, Ontario, Quebec, and Saskatchewan. Appendix Graphs 34 and 35 show their predictions for Canada at the national level. Appendix Graphs 36 and 37 show DELP predictions for British Columbia, for instance. 


***

Appendix Graph 34. Canada, national level, Predicted total deaths, DELP model. || Source: https://covidanalytics.io/projections Accessed on March 14, 2022.

 
***

Appendix Graph 35. Canada, national level, Predicted total cases, DELP model. || Source: https://covidanalytics.io/projections Accessed on March 14, 2022.

***

Appendix Graph 36. Canada, British Columbia, Predicted total deaths, DELP model. || Source: https://covidanalytics.io/projections Accessed on March 14, 2022.


*** 

Appendix Graph 37. Canada, British Columbia, Predicted total cases, DELP model. || Source: https://covidanalytics.io/projections Accessed on March 14, 2022.

 
***









<br/><br/>

IHME model

The IHME model does not present predictions of daily cases. They provide predictions of daily infections. See Appendix Graphs 38 and 39 below. IHME provides predictions for seven provinces: Alberta, British Columbia, Manitoba, Nova Scotia, Ontario, Quebec, and Saskatchewan. Appendix Graphs 40 and 41 show IHME predictions for British Columbia, for instance. 


***

Appendix Graph 38. Canada, national level, Predicted daily deaths, IHME model. || Source: https://covid19.healthdata.org/canada?view=daily-deaths&tab=trend Accessed on March 14, 2022.


*** 

Appendix Graph 39. Canada, national level, Predicted daily infections, IHME model. || Source: https://covid19.healthdata.org/canada?view=infections-testing&tab=trend&test=infections Accessed on March 14, 2022.

*** 

Appendix Graph 40. Canada, British Columbia, Predicted daily deaths, IHME model. || Source: https://covid19.healthdata.org/canada/british-columbia?view=daily-deaths&tab=trend Accessed on March 14, 2022.

 
***

Appendix Graph 41. Canada, British Columbia, Predicted daily infections, IHME model. || Source: https://covid19.healthdata.org/canada/british-columbia?view=infections-testing&tab=trend&test=infections Accessed on March 14, 2022.

 
***






<br/><br/>

IMPE model

The IMPE model does not present predictions of daily cases. They provide predictions of daily infections. IMPE model does not provide predictions for the subnational levels. Appendix Graphs 42 and 43 show predictions for Canada. 


***

Appendix Graph 42. Canada, Predicted daily deaths, IMPE model. || Source: https://raw.githubusercontent.com/mrc-ide/global-lmic-reports/master/CAN/index.pdf Accessed on March 14, 2022.
 
***

Appendix Graph 43. Canada, Predicted daily infections, IMPE model. || Source: https://raw.githubusercontent.com/mrc-ide/global-lmic-reports/master/CAN/index.pdf Page 2. Accessed on March 14, 2022.

*** 



<br/><br/>

LANL model

The LANL COVID-19 Team made its last real-time forecast on September 27th, 2021. || Source: https://covid-19.bsvgateway.org Accessed on March 14, 2022.




<br/><br/>

SRIV model

The SRIV model’s predictions for daily deaths and daily cases are shown in Appendix Graphs 44 and 45 below. SRIV model does not provide predictions for the subnational levels. 


***

Appendix Graph 44. Canada, Predicted daily deaths, SRIV model.|| Source: https://scc-usc.github.io/ReCOVER-COVID-19 Accessed on March 14, 2022.

*** 

Appendix Graph 45. Canada, Predicted daily cases, SRIV model|| Source: https://scc-usc.github.io/ReCOVER-COVID-19 . Accessed on March 14, 2022.

 
***











<br/><br/>

Johns Hopkins compilation of official reports

The Johns Hopkins compilation of official reports does not present daily deaths and daily cases (as of March 14, 2022). They provide weekly deaths and weekly cases. See Appendix Graphs 46 and 47 below. 


***

Appendix Graph 46. Canada, Weekly reported deaths, Johns Hopkins. || Source: https://www.arcgis.com/apps/dashboards/bda7594740fd40299423467b48e9ecf6 Accessed on March 14, 2022.

*** 

Appendix Graph 47. Canada, Weekly reported cases, Johns Hopkins. || Source: https://www.arcgis.com/apps/dashboards/bda7594740fd40299423467b48e9ecf6 Accessed on March 14, 2022.   

 



<br/><br/>

Worldometers compilation of official reports to WHO

The Worldometers compilation of official reports provides reported daily deaths and daily cases, as shown in Appendix Graphs 48 and 49 below. 









Appendix Graph 48. Canada, Daily deaths, Worldometers. || Source: https://www.worldometers.info/coronavirus/country/Canada/ Accessed on March 14, 2022.

 













Appendix Graph 49. Canada, Daily cases, Worldometers || Source: https://www.worldometers.info/coronavirus/country/Canada/ Accessed on March 14, 2022.

 










<br/><br/>

**Compile the graphs from individual models

The DELP model does not present predictions of daily deaths and daily cases. Predictions of daily deaths by IHME, IMPE, and SRIV, and reported daily deaths by Worldometers for Canada at the national level are shown below in Appendix Graph 50. Appendix Graph 51 shows the predicted daily cases by SRIV, predicted daily infections by IHME and IMPE, and the reported daily cases by Worldometers. The DELP and IHME models provide predictions at the subnational level. Transforming the predictions of total deaths and total cases to daily deaths and daily cases needs calculations – performed in the CovidVisualized tools. Therefore, without the CovidVisualized tools, the predictions for the subnational levels are comprised only of those provided by IHME (Appendix Graphs 40 and 41 above). 


 
Appendix Graph 50. Canada, national level, predicted daily deaths by IHME, IMPE, SRIV, and reported daily deaths by Worldometers. Accessed on March 14, 2022. || Source: Assembled from Appendix Graphs 38, 42, 44, and 48.

 

Appendix Graph 51. Canada, predicted daily cases by SRIV, predicted daily infections by IHME and IMPE, and reported daily cases by Worldometers. Accessed on March 14, 2022. || Source: Assembled from Appendix Graphs 39, 43, 45, and 49.


<br/><br/>
  
**How** can the CovidVisualizedCountry tool be practically used for the example of a researcher or advisor to policymakers who wanted to examine the latest predictions for the future trajectory of the COVID-19 epidemic in Canada on March 14, 2022? They would look at the uptake dates in the CovidVisualizedCountry website to find the latest date equal to or before March 14, 2022. The uptake dates in the CovidVisualizedCountry website are displayed on the top of the main web page as the names of directories for each uptake (see Appendix Exhibit 4 below). Scroll down to find the latest uptake date equal to or before March 14, 2022. Appendix Exhibit 5 shows that the date would be 20220311. Clicking on the hyperlinked name 20220311, leads to the page for the uptake 20220311 (see Appendix Exhibit 6). On the page for the uptake 20220311, “Selected graphs” can be viewed, as well as links to the code  used to produce the results and the output  of the code. 

<br/><br/>

Appendix Graphs 52 to 79 (below) show what can be found for uptake 20220311 on the CovidVisualizedCountry website. Official reports by the country are demonstrated as the curves drawn from the Johns Hopkins University compilation (abbreviated as “JOHN” in the graphs). 

The CovidVisualizedCountry website presents the predictions for Canada and its subnational levels in three groups: (1) The national level, (2) Provinces together, and (3) Each province individually. 

Appendix Graph 52 to 61 are for the national level. Appendix Graph 52 shows all models’ predictions for Daily deaths, all-time, i.e., from January 2020 to the latest date available in the models. Appendix Graph 53 focuses on more recent time, i.e.,  2021 on. For the second outcome, i.e., daily cases, Appendix Graph 54 shows the predicted Daily cases or infections, all-time, and Appendix Graph 55 shows the predicted Daily cases or infections, 2021 on. 

Appendix Graphs 56 to 61 demonstrate additional outcomes and variables. Appendix Graphs 56 and 57 provide predicted hospital-related outcomes. Appendix Graph 56 shows all the Hospital-related outcomes, all-time and by all models. Appendix Graph 57 removes the outcomes whose larger sizes compress the curves of outcomes with lower values and focuses on more recent time interval.  There are no readily accessible similar graphs available on the web as far as I know. 

Appendix Graphs 58 to 61 show additional variables estimated by the IHME model: Appendix Graph 58, Daily Infection-detection, Infection-hospitalization, and Infection-fatality ratios, 2021 on, IHME; Appendix Graph 59, Daily Infection-detection, Infection-hospitalization, and Infection-fatality ratios, 2021 onwards, IHME; Appendix Graph 60, Daily mask use, IHME, 2020 on; and Appendix Graph 61, Percent cumulative vaccinated, 2021 on, IHME.

Appendix Graph 62 to 76 are for Canadian Provinces together. Appendix Graph 62 shows Daily reported deaths, JOHN, 2020 on, for eight provinces and the national level. Appendix Graphs 63 and 64 show the same for 2021 on and 2022, respectively. The values of the reported deaths for the national level, Ontario, and Quebec and much higher than those for other provinces. Removing the former group would show the latter’s trajectory more efficiently – that is the Appendix Graphs 65, Reported deaths, Canada without the national level, Ontario, and Quebec, JOHN, 2022. The recent two graphs show the reported daily deaths are mainly on the rise. Graphs 66, 67, 68, and 69 provide the counterpart results for reported daily cases. 

Appendix Graphs 70 to 75 demonstrate predictions by IHME for provinces together. Appendix Graph 70 shows Daily deaths, Reference scenario, IHME, 2020 on. Appendix Graphs 71 and 72 show similar results for 2021 on and 2020, respectively. Appendix Graphs 73, 74, and 75 show counterpart results for predicted daily infections. 

<br/><br/>

Four graphs are provided for each province: (1) Daily deaths, Reference scenario, 2020 on, (2) Daily deaths, Reference scenario, 2021 on, (3)  Daily cases or infections, Reference scenario, 2020 on, and (4) Daily cases or infections, Reference scenario, 2021 on. Appendix Graphs 76 to 79 show those predictions for British Columbia, for instance. Graphs for other provinces are not shown here to save space. Graphs other than the daily deaths and case or infections (mean estimates) for each of the provinces are available in the merge directory of the output: CovidVisualizedCountry/20220311/output/merge/ – for instance, COVID-19 daily cases, Canada, Ontario, reference scenarios with uncertainty, 2021, or COVID-19 hospital-related outcomes, Canada, Quebec, without extremes (IHME Bed need, IMPE Hospital demand), Reference scenarios, 2021 on.

<br/><br/>

Here is the bottom-line conclusion from this example of a researcher or advisor to policymakers who wanted to examine the latest predictions for the future trajectory of the COVID-19 epidemic in Canada on March 14, 2022 – and how the CovidVisualizedCountry tool can help. One can locate the latest predictions by the international and periodically updated models and come up with some sort of compilation of graphs like the Appendix Graphs 50 and 51 made here, or similar graphs for other outcomes. In the meantime, Appendix Graph 52 to 55 show the equivalent of those compilations of graphs for the national level, readily available via the CovidVisualizedCountry tool. Appendix Graphs 77 to 78 show the CovidVisualizedCountry complied graphs for British Columbia. The graphs compiled in the CovidVisualizedCountry tool are much more usable and demonstrate different aspects like calendar time intervals, different scenarios, mean estimates and confidence intervals, and individual models’ details. The software code used to produce the graphs is accessible  and can be rerun by others to verify the correctness and potential mistakes. The track record of the previous periodical uptakes is also accessible – via RESULTS CANADA, national 2021, RESULTS CANADA, national 2022, RESULTS CANADA, provinces 2021, RESULTS CANADA, provinces 2022, RESULTS British Columbia 2021, RESULTS British Columbia 2022, and similar web pages shown in the root of the CovidVisualizedCountry website. The CovidVisualizedCountry uptake 20220311 also adds the following summary by its creator, and puts all the graphs in “Canada COVID-19 epidemic models situation report No 38 – 2022-03-11.pdf”.
Summary 20220311:

<br/><br/>
Observation:

Reported daily cases are stagnating after their recent decrease at the national level and in all provinces.

Reported daily deaths have stopped decreasing after their recent decrease at the national level and in all provinces. They stagnate in Ontario and Quebec and increase Alberta, British Columbia, and Manitoba. Reporting by Saskatchewan is grossly manipulated and unreliable.


Probability:

 
Even though the models are highly divergent about the future trajectory of the epidemic, the above-observed trajectories of the reported daily deaths and cases might signify a new surge.












Appendix Exhibit 4. The uptake dates in the CovidVisualizedCountry website are displayed on the top of the main web page as the names of directories for each uptake. || Source: https://github.com/pourmalek/CovidVisualizedCountry Accessed on March 14, 2022.

 















Appendix Exhibit 5. The latest uptake date equal to or before March 14, 2022, is 20220311.
|| Source: https://github.com/pourmalek/CovidVisualizedCountry Accessed on March 14, 2022.

 










Appendix Exhibit 6. The CovidVisualizedCountry website page for uptake 20220311. || Source: https://github.com/pourmalek/CovidVisualizedCountry/tree/main/20220311 Accessed on March 14, 2022.

 













Appendix Graph 52. Canada, national, Daily deaths, all-time || Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 53. Canada, national, Daily deaths, 2021 on || Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 54. Canada, national, Daily cases or infections, all-time || Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 55. Canada, national, Daily cases or infections, 2021 on || Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 56. Canada, national, Hospital-related outcomes, all-time || Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 57. Canada, national,  Daily hospital-related outcomes, without IHME Bed need, IMPE Hospital demand, Reference scenarios, 2021 on || Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 58. Canada, national, Daily Infection-detection, Infection-hospitalization, and Infection-fatality ratios, Reference scenario, IHME, 2021 on || Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 59. Canada, national,  Daily Infection-detection, Infection-hospitalization, and Infection-fatality ratios, 2021 on, IHME || Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 60. Canada, national,  Daily mask use, IHME, 2020 on || Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 61. Canada, national,  Percent cumulative vaccinated, 2021 on, IHME || Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 62. Canada, provinces together, Daily reported deaths, JOHN, 2020 on || Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 63. Canada, provinces together, Daily reported deaths, JOHN, 2021 on || Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 64. Canada, provinces together, Daily reported deaths, JOHN, 2022 || Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 65. Canada, provinces together, Daily reported deaths, without National, Ontario, and Quebec, JOHN, 2022 || Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 66. Canada, provinces together, Daily reported cases, JOHN, 2020 on || Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 67. Canada, provinces together, Daily reported cases, JOHN, 2021 on || Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 68. Canada, provinces together, Daily reported cases, JOHN, 2022 || Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 69. Canada, provinces together, Daily reported cases, without National, Ontario, and Quebec, JOHN, 2022 || Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 70. Canada, provinces together, Daily deaths, Reference scenario, IHME, 2020 on || Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 71. Canada, provinces together, Daily deaths, Reference scenario, IHME, 2021 on || Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 72. Canada, provinces together, Daily deaths, Reference scenario, IHME, 2022 || Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 73. Canada, provinces together, Daily infections, Reference scenario, IHME, 2020 on|| Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 74. Canada, provinces together, Daily infections, Reference scenario, IHME, 2021 on|| Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 75. Canada, provinces together, Daily infections, Reference scenario, IHME, 2022|| Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 75. Canada, British Columbia, Daily deaths, Reference scenario, 2020 on|| Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 76. Canada, British Columbia, Daily deaths, Reference scenario, 2021 on|| Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 77. Canada, British Columbia, Daily cases or infections, Reference scenario, 2020 on|| Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.
 
Appendix Graph 78. Canada, British Columbia, Daily cases or infections, Reference scenario, 2021 on|| Source: CovidVisualizedCountry uptake 20220311 Accessed on March 14, 2022.







<br/><br/>
 
### Example 3: Global level and WHO regions

Here is a real-life example that explains what a researcher or advisor to policymakers would have needed to do if they wanted to examine the latest predictions by the international and periodically updated models for the future trajectory of the COVID-19 pandemic at the global level and six WHO regions, on March 15, 2022. I trust that the people in charge of world health and regional health perform a similar process – among numerous others – regularly. The European CDC runs an ensemble model for short-term forecasts of Covid-19 cases and deaths across Europe ( The European Covid-19 Forecast Hub) , as does the United States CDC . 

To examine the latest predictions of daily deaths and daily cases at the global and regional levels by the international and periodically updated models, one needs to identify the models, locate their websites, find the graphs, create the missing graphs, (redevelop the existing graphs), and compile the graphs. I tried to replicate the above steps, and the results are presented below. 


<br/><br/>

DELP model

The DELP model does not present predictions of daily deaths and daily cases. They provide predictions of total deaths and total cases. Appendix Graphs 79 and 80 show their predictions for the global level. DELP model provides predictions for the continents. Appendix Graphs 81 and 82 show DELP predictions for Europe (the closest match for the European region used in this example), for instance. 


Appendix Graph 79. Global, Predicted total deaths, DELP model. || Source: https://covidanalytics.io/projections Accessed on March 15, 2022.

 










Appendix Graph 80. Global, Predicted total cases, DELP model. || Source: https://covidanalytics.io/projections Accessed on March 15, 2022.

 











Appendix Graph 81. Europe, Predicted total deaths, DELP model. || Source: https://covidanalytics.io/projections Accessed on March 15, 2022.

 











Appendix Graph 82. Europe, Predicted total cases, DELP model. || Source: https://covidanalytics.io/projections Accessed on March 15, 2022.

 










<br/><br/>

IHME model

The IHME model does not present predictions of daily cases. They provide predictions of daily infections. See Appendix Graphs 83 and 84 below for the global level. IHME provides predictions for WHO regions and the World Bank regions. Appendix Graphs 85 and 86 show IHME predictions for the European region (WHO), for instance. 


Appendix Graph 83. Global, Predicted daily deaths, IHME model. || Source: https://covid19.healthdata.org/global?view=daily-deaths&tab=trend Accessed on March 15, 2022.

 





Appendix Graph 84. Global, Predicted daily infections, IHME model. || Source: https://covid19.healthdata.org/global?view=infections-testing&tab=trend&test=infections Accessed on March 15, 2022.

 














Appendix Graph 85. European region, Predicted daily deaths, IHME model. || Source: https://covid19.healthdata.org/european-region?view=daily-deaths&tab=trend Accessed on March 15, 2022.
 














Appendix Graph 86. European region, Predicted daily infections, IHME model. || Source: https://covid19.healthdata.org/european-region?view=infections-testing&tab=trend&test=infections Accessed on March 15, 2022.

 













<br/><br/>

IMPE model

For the global level, Appendix Graph 87 shows their predicted daily deaths from February 2020 to February 2022. The IMPE model does not present predictions of daily cases. They provide predictions of daily infections. Their graph for the predicted daily infections at the global level is not locatable for me. The IMPE model provides some predictions for the continents. Appendix Graph 88 shows Cumulative deaths by continents together, 2020-01 to 2022-01. Appendix Graph 88 shows Cumulative Deaths since 10 deaths for seven European countries. Their graphs for the predicted daily infections at the continent level are not locatable for me.


Appendix Graph 87. Global, Daily deaths, IMPE model, Feb 2020 to Feb 2022. || Source: https://mrc-ide.github.io/global-lmic-reports/ Accessed on March 15, 2022.

 




Appendix Graph 88. Cumulative deaths by continents, 2020-01 to 2022-01. || Source: https://github.com/mrc-ide/global-lmic-reports/blob/master/Europe/2022-01-20/index.pdf Page 1. Accessed on March 15, 2022.


 











Appendix Graph 88. Cumulative Deaths since 10 deaths, seven European countries.  || Source: https://github.com/mrc-ide/global-lmic-reports/blob/master/Europe/2022-01-20/index.pdf Page 2. Accessed on March 15, 2022.

 

<br/><br/>

LANL model

The LANL COVID-19 Team made its last real-time forecast on September 27th, 2021. || Source: https://covid-19.bsvgateway.org Accessed on March 15, 2022.


<br/><br/>

SRIV model

The SRIV model’s graphs are available for individual countries and the states in the United States. Their graphs for the global and regional levels are not locatable for me. 


<br/><br/>

Johns Hopkins compilation of official reports

The Johns Hopkins compilation of official reports does not present daily deaths and daily cases (as of March 15, 2022). They provide weekly deaths and weekly cases. See Appendix Graphs 89 and 90 below. 



Appendix Graph 89. Global, Weekly reported deaths, Johns Hopkins. || Source: https://www.arcgis.com/apps/dashboards/bda7594740fd40299423467b48e9ecf6 Accessed on March 15, 2022.

 



Appendix Graph 90. Global, Weekly reported cases, Johns Hopkins. || Source: https://www.arcgis.com/apps/dashboards/bda7594740fd40299423467b48e9ecf6 Accessed on March 15, 2022.   

 




Worldometers compilation of official reports to WHO

The Worldometers compilation of official reports provides reported daily deaths and daily cases, shown in Appendix Graphs 91 and 92 below. 









Appendix Graph 91. Global, Daily deaths, Worldometers. || Source: https://www.worldometers.info/coronavirus/ Accessed on March 15, 2022.

 










Appendix Graph 92. Global, Daily cases, Worldometers. || Source: https://www.worldometers.info/coronavirus/ Accessed on March 15, 2022.

 








<br/><br/>

**Compile the graphs from individual models

The DELP model does not present predictions of daily deaths and daily cases. IMPE graphs for predicted daily deaths at the continent level and daily infections at the global and continent levels are not readily locatable. The SRIV model does not provide graphs for the global and continent levels. 

Predictions of daily deaths by IHME and IMPE and the reported daily deaths by Worldometers for global level are shown below in Appendix Graph 93. Graphs of daily infections or cases are only provided by the IHME model. Therefore, it is not possible to assemble a graph by all models for the predicted daily cases or infections. For the regional or continental level, the graphs by the models are even more scarce. Only IHME provides regional-level graphs. Therefore, it is not possible to assemble a graph by all models for the predicted daily deaths or for the daily cases or infections at the regional level. 


<br/><br/>
 
Appendix Graph 93. Global, predicted daily deaths by IHME and IMPE, and the reported daily deaths by Worldometers. Accessed on March 15, 2022. || Source: Assembled from Appendix Graphs 83, 87, and 91.


<br/><br/>  

**How** can the CovidVisualizedGlobal tool be practically used for the example of a researcher or advisor to policymakers who wanted to examine the latest predictions for the future trajectory of the COVID-19 epidemic at the global and WHO regional levels on March 15, 2022? They would look at the uptake dates in the CovidVisualizedGlobal website to find the latest date equal to or before March 15, 2022. The uptake dates in the CovidVisualizedGlobal website are displayed on the top of the main web page as the names of directories for each uptake (see Appendix Exhibit 7 below). Scroll down to find the latest uptake date equal to or before March 15, 2022. Appendix Exhibit 7 shows that the date would be 20220311. Clicking on the hyperlinked name 20220311, leads to the page for the uptake 20220311 (see Appendix Exhibit 6). On the page for the uptake 20220311, “Selected graphs” can be viewed, as well as links to the code  used to produce the results and the output  of the code. 

Appendix Graphs 94 to 129 (below) show what can be found for uptake 20220311 on the CovidVisualizedGlobal website. Official reports by the country are demonstrated as the curves drawn from the Johns Hopkins University compilation (abbreviated as “JOHN” in the graphs). Most of these graphs do not have readily locatable similars on the web that I am aware of. 

The CovidVisualizedGlobal website presents the predictions for the global and WHO regional levels in three groups: (1) The global level, (2) Regions together, and (3) Each region individually. 

Appendix Graph 94 to 125 are for the global level. Appendix Graph 94 shows all models’ predictions for Daily deaths, reference scenarios, 2020 on. Appendix Graph 95 focuses on more recent times, i.e., 2021 on. Appendix Graph 96 adds IHME excess deaths. Appendix Graph 97 adds the alternate scenarios from IHME and IMPE. Appendix Graphs 98 and 99 show alternate scenarios with uncertainty by IHME and IMPE, respectively. 


For the second outcome, i.e., daily cases or infections, Appendix Graph 100 shows the predicted Daily cases or infections, reference scenarios, 2020 on, and Appendix Graph 101 shows them for 2021 onwards. Appendix Graph 102 demonstrates Daily cases or infections, 3 scenarios, 2021 on. Graph 102 Daily cases, 2021 on by DELP and SRIV. 

Appendix Graphs 103 and 104 provide additional insight. Appendix Graph 103 shows the Daily estimated infections IHME IMPE to reported cases JOHN, main scenarios, 2021 on. Appendix Graphs 104 shows Daily deaths estimated to reported, reference scenarios, 2020 onwards.

Appendix Graphs 105 and 106 depict the hospital-related outcomes. Appendix Graph 105 shows Hospital-related outcomes, 2020 on, and Appendix Graph 106 shows Hospital-related outcomes, 2021 without IHME Bed need and IMPE Hospital demand. 

Appendix Graphs 107 to 126 demonstrate additional outcomes and variables. Appendix Graph 107 shows Daily Infection outcomes ratios, 2 scenarios, 2020 on, IHME. Appendix Graph 108 shows Daily Infection -detection and -hospitalizations ratios, 2 scenarios, 2020 on, IHME. Appendix Graph 109 depicts Daily mobility, 2 scenarios, 2020 on, IHME. Appendix Graph 110 demonstrates Daily mask use, 2 scenarios, 2020 on, IHME.

Appendix Graphs 111 to 118 are for WHO regional levels together. Appendix Graph 111 shows Daily deaths, with GLOBAL, 2020 on, JOHN. Appendix Graph 112 shows the same without the global. Appendix Graph 113 and 114 depict Daily deaths, 2022 on, JOHN, with and without the global level, respectively. The latter graph is quite illustrative of the trajectory of reported deaths by different regions. 

Appendix Graphs 115 to 118 show models’ predictions for the regional levels together. Appendix Graph 115 shows Daily infections, with GLOBAL, 2020 on, IHME, IMPE. Appendix Graph 116 shows the same without the global level. Appendix Graph 117 shows Daily cases, with GLOBAL, 2022 on, DELP, SRIV, and Appendix Graph 118 shows the same without the global level. 

Appendix Graphs 119 to 124 show the predicted total deaths. Appendix Graphs 119 and 120 show Total deaths, with GLOBAL, 2020 on, IHME, IMPE and Total deaths, without GLOBAL, 2020 on, IHME, IMPE. Appendix Graphs 121 and 122 show Total deaths, with GLOBAL, 2022 on, DELP, SRIV, and Total deaths, without GLOBAL, DELP, SRIV. Appendix Graphs 123 and 124 depict  Total excess deaths, with GLOBAL, 2020 on, IHME and Total excess deaths, without GLOBAL, 2020 on, IHME. Appendix Graphs 125 and 126 show Total cases, with GLOBAL, 2022 on, DELP, SRIV and Total cases, without GLOBAL, 2022 on, DELP, SRIV. 

<br/><br/>

Four graphs are provided for each WHO region: (1) Daily deaths, reference scenarios, 2020 on, (2) Daily deaths, 3 scenarios, 2021 on, (3) Daily cases or infections, reference scenarios, 2020 on, and (4) Daily cases or infections, 3 scenarios, 2021 on. Appendix Graphs 127 to 130 show those predictions for the European region, for instance. Graphs for other regions are not shown here to save space. Graphs other than the daily deaths and infections for each of the regions are available in the “merge” directory  – for instance, Daily cases or infections, EURO, Reference scenarios with uncertainty, 2021 on, or Daily cases or infections, EURO, Reference scenarios with alternate scenarios, 2021 on. 

Here is the bottom-line conclusion from this example of a researcher or advisor to policymakers who wanted to examine the latest predictions for the future trajectory of the COVID-19 pandemic at the global and WHO regional levels on March 15, 2022 – and how the CovidVisualizedGlobal tool can help. One can locate the latest predictions by the international and periodically updated models and come up with some sort of incomplete compilation of daily deaths graphs for the global level like the Appendix Graph 93 (above) made here. It is not possible to create similar graphs for the daily cases or infections for the global level, or any meaningful graphs for the regional levels. While Appendix Graph 93 is the only graph that can be compiled for daily deaths or daily cases at the global and regional levels (without creating the missing graphs), the graphs compiled in the CovidVisualizedGlobal tool are much more meaningful. Moreover, they demonstrate different aspects like calendar time intervals, different scenarios, mean estimates and confidence intervals, and individual models’ details. The software code used to produce the graphs is accessible  and can be rerun by others to verify the correctness and potential mistakes. The track record of the previous periodical uptakes is also accessible – via RESULTS GLOBAL 2021, RESULTS GLOBAL 2022, RESULTS Regions together, RESULTS European region, and similar web pages shown at the root of the CovidVisualizedGlobal website for other regions. The CovidVisualizedGlobal uptake 20220311 also adds the following summary by its creator, and puts all the graphs in “GLOBAL and REGIONAL COVID-19 epidemic models situation report No 35 - 2022-03-11”.

<br/><br/>

Summary 20220311:

Observation:

Reported COVID-19 daily deaths are bouncing up at the Global level, in Europe, Canada and USA, and continuing to rise in the Western Pacific region.

Reported COVID-19 daily cases are bouncing up at the Global level and in Europe, continuing to rise in the Western Pacific region, and stagnating from the previous decrease in other regions.

Probability:

 

Even though the models are highly divergent about the future trajectory of the pandemic, the above-observed trajectories of the reported daily deaths and cases might signify a new surge.

<br/><br/>

Appendix Exhibit 7. The uptake dates in the CovidVisualizedGlobal website are displayed on the top of the main web page as the names of directories for each uptake. || Source: https://github.com/pourmalek/CovidVisualizedGlobal Accessed on March 15, 2022.

 














Appendix Exhibit 8. The latest uptake date equal to or before March 15, 2022, is 20220311.
|| Source: https://github.com/pourmalek/CovidVisualizedGlobal Accessed on March 15, 2022.

 











Appendix Exhibit 9. The CovidVisualizedGlobal website page for uptake 20220311. || Source: https://github.com/pourmalek/CovidVisualizedGlobal/tree/main/20220311 Accessed on March 15, 2022.
 














Appendix Graph 94. Global, Daily deaths, reference scenarios, 2020 on || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 
Appendix Graph 95. Global, Daily deaths, reference scenarios, 2021 on || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.

 
Appendix Graph 96. Global, Daily deaths, reference scenarios, 2021 on, with IHME excess deaths || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 
Appendix Graph 97. Global, Daily deaths, 3 scenarios, 2021 on || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.

 
Appendix Graph 98. Global, Daily deaths, 3 scenarios, 2021 on, IHME || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 
Appendix Graph 99. Global, Daily deaths, 3 scenarios, 2021 on, IMPE || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.

 
Appendix Graph 100. Global, Daily cases or infections, reference scenarios, 2020 on || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 
Appendix Graph 101. Global, Daily cases or infections, reference scenarios, 2021 on || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.

 
Appendix Graph 102. Global, Daily cases or infections, 3 scenarios, 2021 on || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 
Appendix Graph 103. Global, Daily estimated infections IHME IMPE to reported cases JOHN, main scenarios, 2021 on || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 
Appendix Graph 104. Global, Daily deaths estimated to reported, reference scenarios, 2020 on || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 
Appendix Graph 105. Global, Hospital-related outcomes, 2020 on|| Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.

 
Appendix Graph 106. Global, Hospital-related outcomes, 2021 on, without IHME Bed need and IMPE Hospital demand || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 
Appendix Graph 107. Global, Daily Infection outcomes ratios, 2 scenarios, 2020 on, IHME || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 
Appendix Graph 108. Global, Daily Infection -detection and -hospitalizations ratios, 2 scenarios, 2020 on, IHME || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 
Appendix Graph 109. Global, Daily mobility, 2 scenarios, 2020 on, IHME || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 
Appendix Graph 110. Global, Daily mask use, 2 scenarios, 2020 on, IHME || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 

Appendix Graph 111. Global, Daily deaths, with GLOBAL, 2020 on, JOHN|| Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 
Appendix Graph 112. Global, Daily deaths, without GLOBAL, 2020 on, JOHN || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 

Appendix Graph 113. Global, Daily deaths, with GLOBAL, 2022 on, JOHN || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 
Appendix Graph 114. Global, Daily deaths, without GLOBAL, 2022 on, JOHN || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 
Appendix Graph 115. Global, Daily infections, with GLOBAL, 2020 on, IHME, IMPE || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 

Appendix Graph 116. Global, Daily infections, without GLOBAL, 2020 on, IHME, IMPE || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 

Appendix Graph 117. Global, Daily cases, with GLOBAL, 2022 on, DELP, SRIV || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 
Appendix Graph 118. Global, Daily cases, without GLOBAL, 2022 on, DELP, SRIV || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 

Appendix Graph 119. Global, Total deaths, with GLOBAL, 2020 on, IHME, IMPE || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 
Appendix Graph 120. Global, Total deaths, without GLOBAL, 2020 on, IHME, IMPE|| Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 

Appendix Graph 121. Global, Total deaths, with GLOBAL, 2022 on, DELP, SRIV || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 
Appendix Graph 122. Global, Total deaths, without GLOBAL, DELP, SRIV || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 

Appendix Graph 123. Global, Total excess deaths, with GLOBAL, 2020 on, IHME || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 
Appendix Graph 124. Global, Total excess deaths, without GLOBAL, 2020 on, IHME || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 
Appendix Graph 125. Global, Total cases, with GLOBAL, 2022 on, DELP, SRIV || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.

 
Appendix Graph 126. Global, Total cases, without GLOBAL, 2022 on, DELP, SRIV|| Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 

Appendix Graph 127. European region, Daily deaths, reference scenarios, 2020 on || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 
Appendix Graph 128. European region, Daily deaths, 3 scenarios, 2021 on || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.
 
Appendix Graph 129. European region, Daily cases or infections, reference scenarios, 2020 on|| Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.

 
Appendix Graph 130. European region, Daily cases or infections, 3 scenarios, 2021 on || Source: CovidVisualizedGlobal uptake 20220311 Accessed on March 15, 2022.

 
<br/><br/>

### Postscript: 

(A) Compare Appendix Graph 93 with Appendix Graph 96. The former is a researcher-made compilation of predicted daily deaths at the global level by the models. The latter is the graph available from the CovidVisualizedGlobal tool. The difference demonstrates the added value of the CovidVisualized tools.

(B) The three CovidVisualized tools clearly warn on March 15, 2022, how and why there are possibilities of new surges, even though the models' predictions are divergent. 






