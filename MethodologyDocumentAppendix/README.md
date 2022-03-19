# CovidVisualized Methodology Document Appendix


Methodology document appendix for CovidVisualized tools: [`CovidVisualizedGlobal`](https://github.com/pourmalek/CovidVisualizedGlobal), [`CovidVisualizedCountry`](https://github.com/pourmalek/CovidVisualizedCountry), and [`covir2`](https://github.com/pourmalek/covir2)

CovidVisualized: Visualized compilation of international updating models estimates of COVID-19 pandemic at global and country levels

Appendix: Examples of what the CovidVisualized tools provide in addition to the individual models

Farshad Pourmalek, MD PhD
Former lecturer, University of British Columbia, Vancouver, Canada
pourmalek_farshad at yahoo dot com


<br/><br/>


### TABLE OF CONTENTS:

[Summary](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/MethodologyDocumentAppendix/README.md#summary)

[CovidVisualized tools](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/MethodologyDocumentAppendix/README.md#covidvisualized-tools)

[The five international and periodically updated COVID-19 pandemic models](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/MethodologyDocumentAppendix/README.md#the-five-international-and-periodically-updated-covid-19-pandemic-models-are)

[Examples of what the CovidVisualized tools provide in addition to the individual models](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/MethodologyDocumentAppendix/README.md#examples-of-what-the-covidvisualized-tools-provide-in-addition-to-the-individual-models)

[Example 1: Iran](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/MethodologyDocumentAppendix/Example%201%20Iran/RAEDME.md)

[Example 2: Canada and its province](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/MethodologyDocumentAppendix/Example%202%20Canada%20et%20al/README.md)

[Example 3: Global level and WHO regions](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/MethodologyDocumentAppendix/Example%203%20Global%20regional/README.md)

[Postscript](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/MethodologyDocumentAppendix/README.md#postscript)

[References](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/MethodologyDocumentAppendix/README.md#references)


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

**Here** are three examples illustrating what the CovidVisualized tools provide in addition to the individual models. 

[Example 1](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/MethodologyDocumentAppendix/Example%201%20Iran/RAEDME.md) is for Iran. 

[Example 2](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/MethodologyDocumentAppendix/Example%202%20Canada%20et%20al/README.md) is for Canada and its province.

[Example 3](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/MethodologyDocumentAppendix/Example%203%20Global%20regional/README.md) looks at the global level and WHO regions. 

For sample applications of “covir2” to countries without subnational estimates see [Afghanistan](https://github.com/pourmalek/covir2/tree/main/ADAPTATIONS_EXAMPLES/Afghanistan_%2020210625/20210625), [Pakistan](https://github.com/pourmalek/covir2/tree/main/ADAPTATIONS_EXAMPLES/Pakistan_20210704), [Japan 20210506](https://github.com/pourmalek/covir2/tree/main/ADAPTATIONS_EXAMPLES/Japan_20210506), [Japan 20210928](https://github.com/pourmalek/covir2/tree/main/ADAPTATIONS_EXAMPLES/Japan_20210928)



<br/><br/>

### Postscript: 

(A) Compare Appendix Graph 93 with Appendix Graph 96. The former is a researcher-made compilation of predicted daily deaths at the global level by the models. The latter is the graph available from the CovidVisualizedGlobal tool. The difference demonstrates the added value of the CovidVisualized tools.

(B) The three CovidVisualized tools clearly warn on March 15, 2022, how and why there are possibilities of new surges, even though the models' predictions are divergent. 



<br/><br/>

### References:

1. COVID Analytics. DELPHI epidemiological case predictions. Cambridge: Operations Research Center, Massachusetts Institute of Technology. https://www.covidanalytics.io/projections and https://github.com/COVIDAnalytics/website/tree/master/data/predicted Accessed 23 June 2021. 
2. Institute for Health Metrics and Evaluation (IHME). COVID-19 mortality, infection, testing, hospital resource use, and social distancing projections. Seattle: Institute for Health Metrics and Evaluation (IHME), University of Washington. http://www.healthdata.org/covid/ and http://www.healthdata.org/covid/data-downloads Accessed 23 June 2021.
3. MRC Centre for Global Infectious Disease Analysis (MRC GIDA). Future scenarios of the healthcare burden of COVID-19 in low- or middle-income countries. London: MRC Centre for Global Infectious Disease Analysis, Imperial College London. https://mrc-ide.github.io/global-lmic-reports/ and https://github.com/mrc-ide/global-lmic-reports/tree/master/data Accessed 23 June 2021.
4. Los Alamos National Laboratory (LANL). COVID-19 cases and deaths forecasts. Los Alamos: Los Alamos National Laboratory (LANL). https://covid-19.bsvgateway.org Accessed 23 June 2021.
5. Srivastava, Ajitesh. University of Southern California (USC). COVID-19 forecast. Los Angeles: University of Southern California. https://scc-usc.github.io/ReCOVER-COVID-19 and https://github.com/scc-usc/ReCOVER-COVID-19/tree/master/results/historical_forecasts Accessed 23 June 2021.



 
 







