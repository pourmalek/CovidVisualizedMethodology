# CovidVisualizedMethodology
CovidVisualized Methodology Documents

<br/><br/>

This repository contains the CovidVisualized Methodology Documents:

[CovidVisualized Methodology Document](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#covidvisualized-methodology-document) 
|| [PDF](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/CovidVisualized%20Methodology%20Document.pdf)

This CovidVisualized methodology document explains the conceptual and computational details of the development of CovidVisualized tools. Examples of “what the CovidVisualized tools provide in addition to the individual models” are provided in the companion “CovidVisualized methodology document appendix”. 

<br/><br/>

[CovidVisualized Methodology Document Appendix](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#covidvisualized-methodology-document-appendix)
|| [PDF](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/CovidVisualized%20Methodology%20Document%20Appendix.pdf)

This CovidVisualized Methodology Document Appendix provides examples of how the CovidVisualized tools can be used to examine the predictions by the international and periodically updated epidemic models for the future trajectory of the COVID-19 pandemic at global and country levels.

<br/><br/>


****************************************************************************************
****************************************************************************************
****************************************************************************************


# CovidVisualized Methodology Document

Methodology document for CovidVisualized tools: [`CovidVisualizedGlobal`](https://github.com/pourmalek/CovidVisualizedGlobal), [`CovidVisualizedCountry`](https://github.com/pourmalek/CovidVisualizedCountry), and [`covir2`](https://github.com/pourmalek/covir2)

CovidVisualized: Visualized compilation of international updated models' estimates of COVID-19 pandemic at global and country levels

Farshad Pourmalek, MD PhD
Former lecturer, University of British Columbia, Vancouver, Canada.
pourmalek_farshad at yahoo dot com

<br/><br/>


### TABLE OF CONTENTS:

[Summary](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#summary)

[CovidVisualized tools](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#covidvisualized-tools)

[International and periodically updated COVId-19 pandemic models](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#international-and-periodically-updated-covid-19-pandemic-models)

[Study justification and added value](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#study-justification-and-added-value)

[Characteristics of the models](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#characteristics-of-the-models)

[Data management](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#data-management)

[Primary and secondary variables](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#primary-and-secondary-variables)

[Smoothing](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#smoothing)

[Models’ scenarios](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#models-scenarios)

[Models’ versions](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#models-versions)

[Periodical updates and uptakes](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#periodical-updates-and-uptakes)


<br/><br/>


### Summary

This CovidVisualized methodology document explains the conceptual and computational details of the development of CovidVisualized tools. Examples of “what the CovidVisualized tools provide in addition to the individual models” are provided in the companion “CovidVisualized methodology document appendix”. 

<br/><br/>



### CovidVisualized tools

There are three CovidVisualized tools:

(1) CovidVisualizedGlobal: Combine and visualize international periodically updated estimates of COVID-19 pandemic at the global level and six WHO regions [1] https://github.com/pourmalek/CovidVisualizedGlobal 

(2) CovidVisualizedCountry: Combine and visualize international periodically updated estimates of COVID-19 pandemic at the country level: Canada, national and subnational [2] https://github.com/pourmalek/CovidVisualizedCountry 

(3) covir2: Combine and visualize international periodically updated estimates of COVID-19 pandemic at the country level, countries without subnational level estimates: Iran [3] https://github.com/pourmalek/covir2 


<br/><br/>


### International and periodically updated COVId-19 pandemic models

The five international and periodically updated COVId-19 pandemic models included in this work are (1) DELPHI , Massachusetts Institute of Technology, Cambridge (abbreviation used in this work: DELP) [4], (2) Institute for Health Metrics and Evaluation, Seattle (IHME) [5], (3) Imperial College, London (IMPE) [6], (4) Los Alamos National Laboratories, Los Alamos (LANL) [7], (5) University of Southern California, Los Angeles, by Srivastava, Ajitesh (SRIV) [8].

<br/><br/>


### Study justification and added value

What is missing from the individual international and periodically updated models that creation of the CovidVisualized tools [1-3] was needed? Nothing substantial is missing from the individual (international and periodically updated) models. However, some of those models do not report predictions of daily outcomes or do not provide the predictions at the global or regional levels. Suppose that a researcher or advisor to policymakers wants to look at the latest predictions by all international and periodically updated models for any given country or location (e.g., Canada and its provinces, or the European region). In that case, they need to know or find the website addresses for graphs and data of each model, find the graphs that are available on the websites for the models, develop the graphs that are not available, and put together and examine the graphs that use different horizontal (time) and vertical (outcome) axes. If they want to repeat this, they will need to repeat all the steps, which is time-consuming. The CovidVisualized tools have consistently performed the steps mentioned above and compiled the graphs (and data) from individual models together in a usable framework and continue to do so regularly. 

**The obstacles:** The obstacles one would encounter in examining the latest predictions by all international and periodically updated models for any given country or location are mentioned below. (1) The DELP model [4] does not provide predictions of daily deaths and daily cases. One needs to calculate them from the provided total deaths and total cases. (2) The IMPE model [6] graphs for predicted daily deaths at the continent level and daily infections at the global and continent levels are not readily locatable. (3) The SRIV model [8] does not provide global and continent-level graphs. (4) The researcher-made compilations of available graphs from different models are not practically usable because (a) the graphs from each model use different calendar time intervals and time bins, (b) the maximum value on the y-axis for the same outcome (e.g., daily deaths) are different across models, (c) uncertainty intervals and alternate scenarios are not shown by all the models. (5) Not all models provide graphs for all the variables they predict, e.g., hospital-related outcomes. (6) The predictions’ data files that each model provides follow that model’s unique data arrangements. These data arrangements differ across the models. Without a common data management template, it is impossible to acquire a grip on the models’ data that can lead to the creation of compiled data and graphs. 

Creation of the missing graphs and redeveloping the available graphs need a data management framework capable of compiling data (predictions’ files) from different models. While all the models present a set of common outcomes and variables, they do so in their unique way. The number of data files, the variables and data structure within each file, the nomenclature and variable names, the geographical locations covered by each model, the alternative scenarios, and many other aspects of the predictions provided by the models vary tremendously across the models. Moreover, within each model, there are systematic and random variations and alterations regarding these aspects across time (i.e., with updates released by the model). The CovidVisualized tools [1-3] have covered these issues in a reproducible way, i.e., researchers can download the codes, rerun them, and see the outputs and results. The CovidVisualized tools have already paved the way and resolved the obstacles in examining the predictions in a coherent, consistent, and periodically updated framework, with underlying software codes and outputs. 


<br/><br/>



 
### Characteristics of the models

General characteristics of the five international and periodically updated COVID-19 pandemic models included in this work are described below in Appendix Table 1. These characteristics are taken from a “Rapid review of COVID-19 epidemic estimation studies for Iran” [9]. 

No model is 100% complete, accurate, and valid, and no model is 100% wrong and useless. As described by Vynnycky  and White, models identify the essential elements which determine real life behaviour of the epidemic (i.e., the model assumptions) and then properly include those elements in the model structure and calculations. If these essential elements are identified and incorporated wisely then the model may provide realistic predictions [10] [25]. The first three essential elements of the COVID-19 epidemic are (1) under-reporting of deaths and cases [11-17] [26-32], (2) asymptomatic transmission [11, 18-20] [26, 33-35], and (3) seasonality [21-23] [36-38]. The foreseeable advent of vaccines and variants shifted the epidemiologic landscape of the disease transmission, and hence vaccines and variants belong among the essential elements of the epidemic [24-25] [39-40]. Including alternate scenarios in the models can be quite illustrative and useful for policymakers about future trends in the epidemic and potential role of the interventions [26] [41]. The above-mentioned technical characteristics of the models are mentioned in Appendix Table 2. The whole set of model’s characteristics provides a profile of models’ strengths and weaknesses – that should be considered while examining the predictions by models. 
 
<br/><br/>

Table 1. General characteristics of the included models 

![image](https://user-images.githubusercontent.com/30849720/159102934-6680fa54-5327-48d6-8edb-70d0d5f26009.png)

<br/><br/>



Table 2. Technical characteristics of the included models 

![image](https://user-images.githubusercontent.com/30849720/159103048-936de8be-daad-4b87-afb6-8d152e59e5bf.png)

<br/><br/>




### Data management 

Estimates of (1) Daily Deaths, (2) Total Deaths, (3) Daily Cases (incident or prevalent), and (4) Total Cases (incident) from the five models are the primary outcome variables of interest in this work. Hospital-related and other outcomes from the five models are the secondary outcome variables.

The CovidVisualized tools do not change any outcomes or variables taken from the five international and periodically updated models. Secondary variables are calculated in CovidVisualized tools: (1) Daily deaths and daily cases are calculated from the provided cumulative deaths and cases by JOHN [27], DELP [4], and SRIV [8]. (2) Case Fatality Ratios (CFR), and (3) smoothed variables for daily deaths daily cases from JOHN and DELP. Details of [smoothing](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#smoothing) are provided further below. 

<br/><br/>



### Primary and secondary variables

Primary variables are taken from the five models. Secondary variables are calculated in this work. To facilitate data management, the primary variables were -rename-d or -renvar-ed using the variables from the five models according to the following conventions. The same set of conventions was adhered to in naming all outcome variables.

Primary variables include primary outcome variables, i.e., deaths and cases, and secondary outcome variables, e.g., hospital demand. As described below through examples, primary variable names have six parts, each part denoting one piece of information about the variable. All the variables have descriptive var -label-s that show what the variable stores. Stata commands are displayed as -command- and Stata non-command syntax as -syntax-. 


.

Variable names

_Primary outcome variable names:_

Example:

TotDeaMeRaA01S00

1234567890123456

-varname- has 16 positions.

Tot...Dea...Me....Ra.....A01.....S00

1-3...4-6...7-8...9-10...11-13...14-16 

.

•	Positions 1-3: Tot or Day: Total (cumulative) or Daily

•	Positions 4-6: Dea, Cas, or Act: Dea for Deaths, Cas for incident Cases, or Act for Active cases (for primary outcomes; for secondary outcomes, see below)

•	Positions 7-8: Me, Lo, or Up: Mean, Lower, or Upper (uncertainty bound)

•	Positions 9-10: Ra or Sm: Raw (not smoothed) or Smoothed

•	Positions 11-13: A00 to A05: Model number (see details below)

•	Positions 14-16 S??: Scenario number within the model (see details below)

The example primary variable name, TotDeaMeRaA01S00, denotes Total Deaths, mean, raw, DELPHI, single scenario.

.

_Secondary outcome variable names:_

•	Positions 4-6 in variable name can be, for instance,  Act, which means Active cases [DELP]

•	Positions 4-6: meaning [study]:

•	Act: Active cases [DELP]

•	Adm: Admissions (hospital admissions by day) [IHME]

•	Bed: Bed need (covid beds needed by day) [IHME]

•	Beo: Bed over ([covid all beds needed] - ([total bed capacity] - [average all bed usage])) [IHME]

•	Hod: Hospital Demand [IMPE]

•	Hos: Hospitalized [DELP]

•	Hoi: Hospital incidence [IMPE]

•	Icd: ICU Demand [IMPE]

•	Ici: ICU incidence [IMPE]

•	Icn: ICU new (number of new people going to the ICU by day) [IHME]

•	Ico: ICU over ([covid ICU beds needed] - ([total ICU capacity] - [average ICU bed usage])) [IHME]

•	Icu: ICU need (ICU covid beds needed by day) [IHME]

•	Pre: Prevalence [IMPE]

•	Ref: R effective [IMPE]

•	Rtt: R t [IMPE]

•	Ser: Seroprevalence (seroprevalence) [IHME]

•	Tes: Tests (total tests) [IHME]

•	Ven: Ventilated [DELP]

•	Ven: Vent need (invasive Ventilation needed by day) [IHME]


Example: The -varname- DayIcdMeRaA03S01 carries -varlabel- "Daily ICU demand Mean A03 S01". It is the daily ICU demand, mean estimate, in study A03 (IMPE), scenario 1.

Variable names and short descriptions for hospital-related (and other) outcomes by IHME are mentioned in "IHME_COVID_19_Data_Release_Information_Sheet.pdf" released with each estimates' update of IHME. 


.

_Secondary variable names:_

Secondary variables have two subtypes: (1) variable that store a calculated daily Case Fatality Ratio (CFR), (1) variable that store values created to visualize temporal succession of daily cases and daily deaths peaks.


(1) store a calculated daily CFR

•	Positions 4-6 read as CFR.

Example:

DayCfrMeRaA00S00V00 "Daily CFR JOHN [27]" 

(2) store values created for visualization of temporal succession of daily cases and daily deaths peaks

•	CaM: (Cases Mean) "Daily Cases Mean" 

•	CbD (Cases by Deaths) "Daily cases mean divided by daily deaths mean JOHN" 

•	DeM: (Deaths Mean) "Daily Deaths Mean "


<br/><br/>


### Smoothing

Smoothed outcomes are useful for visualization when the raw outcomes are jagged because of day-to-day fluctuations and weekend patterns in reporting. This is true for reported daily deaths and reported daily cases (JOHN) [27]. It is also true for predicted daily deaths and predicted daily cases or infections in the time interval before a model update, i.e., when a model is backcating the daily outcomes in the past. 

The DELP model [4] does not provide smoothed version of predicted daily variables. Therefore, smoothing is performed in CovidVisualized tools. The IHME model [5] provides smoothed version of predicted daily variables. Their smoothed version of predicted daily variables is used for visualization. The IMPE [6] and LANL [7] models do not provide smoothed version of predicted daily variables. However, their raw (non-smoothed) version of daily outcomes is not very jaggy. Therefore, their raw version of daily outcomes is used in the graphs. The SRIV model [8] does not provide predictions for the past, and their predicted daily outcomes are used in the graphs. Official reports of daily death and daily cases (JOHN) are the prototype of outcomes for which adding the smoothed version is useful for visualization.   

In summary, smoothing is performed for daily deaths daily cases from JOHN and DELP. Moving averages are calculated for those raw daily deaths and raw daily cases, using the -tssmooth ma- command of Stata. The code and output segment used for smoothing the raw daily deaths from Johns Hopkins (variable name is DayDeaMeRaA00S00) is shown below. This segment is taken from: https://github.com/pourmalek/CovidVisualizedCountry/blob/main/20220311/code/JOHN/do%20CovidVisualizedCountry%20JOHN.do that is the -do- file for downloading and preparing the official reports from Johns Hopkins for Canada and its provinces in the uptake 20220311 of CovidVisualizedCountry tool. 

.

// Start of the Stata code segment

. tssmooth ma DayDeaMeRaA00S00_window = DayDeaMeRaA00S00 if DayDeaMeRaA00S00 >= 0, window(3 1 3)

The smoother applied was

by provincestate_encoded : (1/7)*[x(t-3) + x(t-2) + x(t-1) + 1*x(t) + x(t+1) + x(t+2) + x(t+3)]; x(t)= DayDeaMeRaA00S00
     
. tssmooth ma DayDeaMeSmA00S00 = DayDeaMeRaA00S00_window, weights( 1 2 3 <4> 3 2 1) replace

The smoother applied was

by provincestate_encoded : (1/16)*[1*x(t-3) + 2*x(t-2) + 3*x(t-1) + 4*x(t) + 3*x(t+1) + 2*x(t+2) + ...; x(t)= DayDeaMeRaA00S00_window
     
// End of the code segment


<br/><br/>



.

Numbers assigned to the models in this work:

A00 JOHN Johns Hopkins [27]

A01 DELP DELPHI  [4]

A02 IHME Institute for Health Metrics and Evaluation [5]

A03 IMPE Imperial College [6]

A04 LANL Los Alamos National Laboratory [7]

A05 SRIV Srivastava [8]


<br/><br/>


### Models’ scenarios

Scenario numbers within the models: 

[Names within brackets are assigned in this work.]

.

A00 JOHN

S00 = [Not Applicable]

.

A01 DELP

S00 = [Single scenario]

.

A02 IHME  (see more details below)

All updates up to and including 20211217:

S01 = Reference scenario [Status Quo]

S02 = Best scenario (Universal masks) [Best]

S03 = Worse scenario (Mandates easing) [Worst] 

.

Updates 20211221 to 20220110:

S01 = Current projection [Status Quo, Reference scenario]

S02 = 80% mask use [Best scenario]

S03 = High severity of Omicron [Worse scenario]

S04 = Third dose of vaccine [Second best scenario]

S05 = Reduced vaccine hesitancy [Third best scenario] 

.

Updates 20220114 to 20220121:

S01 = Current projection [Status Quo, Reference scenario]

S02 = 80% mask use [Best scenario]

S04 = Third dose of vaccine [Second best scenario]

S05 = Reduced vaccine hesitancy [Third best scenario]

The previous scenario, "severe omicron," was omitted starting from update 20220114. The "current projection" or "reference scenario" is functionally the "worse scenario," i.e., the scenario with highest magnitude of estimated deaths and infections.

.

Updates 20220204 onwards:

S01 = Current projection [Status Quo, Reference scenario]

S02 = 80% mask use 

S03 = Third dose of vaccine [Second best scenario]

.

A03 IMPE

S01 = Additional 50% Reduction [Best]

S02 = Current level of interventions [Reference]

S03 = Relax Interventions 50% [Worst]

S04 = Surged Additional 50% Reduction [Best, Surged]

S05 = Surged Maintain Status Quo [Reference, Surged]

S06 = Surged Relax Interventions 50% [Worst, Surged]

.

A04 LANL

S00 = [Single scenario]

.

A05 SRIV

S00 = [current]

<br/><br/>

Details about IHME scenarios:

All updates up to and including 20211217:

IHME. COVID-19 Results Briefing, The Eastern Mediterranean Region. May 13, 2021. Page 19, Projections and scenarios "The model was run on May 12, 2021."

(S1) The reference scenario is our forecast of what we think is most likely to happen:

1- Vaccines are distributed at the expected pace.

2- Governments adapt their response by re-imposing social distancing mandates for six weeks whenever daily deaths reach 8 per million, unless a location has already spent at least 7 of the last 14 days with daily deaths above this rate and not yet re-imposed social distancing mandates. In this case, the scenario assumes that mandates are re-imposed when daily deaths reach 15 per million.

3- Variants B.1.1.7 (first identified in the UK), B.1.351 (first identified in South Africa), and P1 (first identified in Brazil) continue to spread from locations with (a) more than five sequenced variants, and (b) reports of community transmission, to adjacent locations following the speed of variant scale-up observed in the regions of the UK.

4- In one-quarter of those vaccinated, mobility increases toward pre-COVID-19 levels.

(S2) The universal masks scenario makes all the same assumptions as the reference scenario but also assumes 95% of the population wear masks in public in every location.

(S3) The worse scenario modifies the reference scenario assumptions in three ways:

1- First, it assumes that variants B.1.351 or P1 begin to spread within three weeks in adjacent locations that do not already have B.1.351 or P1 community transmission.

2- Second, it assumes that all those vaccinated increase their mobility toward pre-COVID-19 levels.

3- Third, it assumes that among those vaccinated, mask use starts to decline exponentially one month after completed vaccination.


Updates 20220114 onwards:

Added: Waning immunity, Fitting the past (improved methods), and Omicron specific changes

Including use of integro-differential equations; Fitting the past (IDR, IHR, IFR, for different exposure categories), and Integration of rate estimation within the SEIR fitting approach, simultaneously estimating COVID rates and underlying transmission intensity.


<br/><br/>


### Models’ versions

DELP model versions:

DELP V1 2020-04-17 to 2020-07-04

DELP V2 2020-07-04 to 2020-11-19

DLEP V3 (could not be located)

DELP V4 2020-11-19 to when specified otherwise

DELP source for model versions: 
https://github.com/COVIDAnalytics/website/tree/master/data/predicted

.

IHME model versions:

IHME V1 2020-03-25 to 2020-04-29: IHME-CF = Curve Fitting]

IHME V2 2020-05-04 to 2020-05-26: IHME-CF-SEIR = Curve Fitting and SEIR

IHME V3 2020-05-29 to 2021-04-30: IHME-MS-SEIR = Mortality Spline and SEIR

IHME V4 2021-05-06 to 2022-01-10: IHME-MS-SEIR + Total Covid-19 Mortality 

IHME V5 2022-01-14 onwards: IHME-MS-SEIR + Total Covid-19 Mortality + Waning immunity, Fitting the past (improved methods), and Omicron specific changes

.

IHME source for model versions: 

All models label their versions within their data files or on their websites, except the IHME model. The first three versions of the IHME have been described in [2]. Since May 2021, they changed their key metric from reported deaths to the total number of COVID-19 deaths [32]. This included estimation of the ratio of the total number of COVID-19 death to reported deaths from COVID-19. Hence, the IHME model is labelled V4, in this work, starting from May 6, 2021.

V1: Beginning March 25, IHME initially produced COVID forecasts using a statistical curve fit model (IHME-CF), which was used through April 29 for publicly released forecasts. V2: On May 4, IHME switched to using a hybrid model, drawing on a statistical curve fit in the first stage, followed by a second-stage epidemiological model with susceptible, exposed, infectious, recovered compartments (SEIR). This model was used through May 26. V3: On May 29, the curve fit stage was replaced by a spline fit to the relationship between log cumulative deaths and log cumulative cases, while the second-stage SEIR model remained the same.


.

IMPE model versions:

IMPE V1 2020-04-28 to 2020-05-30

IMPE V2 2020-05-31 to 2020-06-09

IMPE V3 2020-06-14 to 2020-06-26

IMPE V4 2020-06-14 to 2020-07-31

IMPE V5 2020-08-08 to 2020-11-01

IMPE V6 2020-11-10 to 2021-01-12

IMPE V7 2021-01-18 to 2021-04-24

IMPE V8 2021-05-10 to when specified otherwise

IMPE V9 2021-11-03 to when specified otherwise

V8 and V9 run together from 2021-11-03 to when specified otherwise

IMPE source for model versions: 
https://github.com/mrc-ide/global-lmic-reports/tree/master/data


.

LANL model versions:

LANL V1 2020-04-05 to 2020-10-28

LANL V2 2020-10-28 to 2021-09-26

LANL source for model versions: https://covid-19.bsvgateway.org 

The LANL COVID-19 Team made its last real-time forecast on September 27th, 2021. 
Source: https://covid-19.bsvgateway.org


.

SRIV model versions:

SRIV V1 2020-05-02 to 2020-06-02 

SRIV V2 2020-06-03 to when specified otherwise

SRIV source for model versions: 
https://github.com/scc-usc/ReCOVER-COVID-19#our-papers and 
https://github.com/scc-usc/ReCOVER-COVID-19/tree/master/results/historical_forecasts

***

<br/><br/>

#### Models’ websites for estimates files

DELP https://github.com/COVIDAnalytics/website/tree/master/data/predicted

IHME http://www.healthdata.org/covid/data-downloads

IMPE https://github.com/mrc-ide/global-lmic-reports/tree/master/data

LANL https://covid-19.bsvgateway.org

SRIV https://github.com/scc-usc/ReCOVER-COVID-19/tree/master/results/historical_forecasts

JOHN https://github.com/CSSEGISandData/COVID-19 


<br/><br/>

#### Models’ websites for graphs

DELP https://covidanalytics.io/projections

IHME https://covid19.healthdata.org/iran-(islamic-republic-of)?view=cumulative-deaths&tab=trend

IMPE https://github.com/mrc-ide/global-lmic-reports/tree/master/IRN https://github.com/mrc-ide/global-lmic-reports/tree/master/CAN

LANL https://covid-19.bsvgateway.org  

SRIV https://scc-usc.github.io/ReCOVER-COVID-19/

JOHN https://www.arcgis.com/apps/dashboards/bda7594740fd40299423467b48e9ecf6
 
 
 
<br/><br/>

 
### Periodical updates and uptakes


#### Model updates, estimates updates, and CovidVisualized uptakes

With daily accumulation of official country reports to WHO, curated by the Johns Hopkins University [27] and other curators, and other data types used in the models, models update their estimations (predictions) on a rather regular basis. The CovidVisualized tools [1-3] use the estimations updates released by the models on a regular basis. To semantically differentiate between what is released by the models and what is performed by the CovidVisualized tools, the latter is labeled “uptake”. Updates belong to the models. Uptakes belong to the CovidVisualized tools. Updates are released by the model creators. Uptakes are added to CovidVisualized tools by its creator.

The two models with the least frequency of periodic updates of estimates are IHME [5] and IMPE [6], updated almost weekly and bi-weekly, respectively – until November 2021. After spread of the Omicron variants, these models reduced the frequency of their update releases. Therefore, two sets of arrangements ruled the frequency of performing uptakes in the CovidVisualized tools [1-3]. The first set covered the year 2021: With the release of each update of either of these two models, the whole set of the five included models is updated in all the three CovidVisualized GitHub repositories. The most recent update of each model is used. The conventions for periodical uptake are described in more detail below. Estimates of the LANL model [7] get updated about every 3-4 days, and DELP [4] and SRIV [8] models get updated daily. The second set of arrangements for the frequency of performing uptakes in the CovidVisualized tools started in 2022. Uptakes are performed each week on Friday. Each uptake uses the latest available update of each model.  


With much less frequency than that of models’ estimations updates releases, models improve their internal and calculations structures. These are “model versions” that are distinct from models’ estimations updates. Model versions are described in detail below. 

<br/><br/>

#### Detailed description of the of rule for uptakes of CovidVisualized tools in 2021

This is a description of the rule of adding uptakes to CovidVisualized tools [1-3]. The overarching principle for creating uptakes is to create an uptake for each calendar date on which an update is available for either IHME [5] or IMPE [6] and using the most recent update for the other study (IMPE or IHME) for that uptake. The rationale for not including every new update by DELP [4], LANL [7], or SRIV [8] in the overarching principle is that it would lead to too frequent uptakes, which would defy the purpose of gaining new insight with each uptake of the covir2.

Algorithmic details of the rule for adding uptakes to the covir2 repository are as follows. For every single calendar date, (1) Check for new updates by IHME. (2) If a new update by IHME is available, start a new uptake with today's date, and use this new update by IHME. (3) Look for the latest available update by IMPE and include that in this uptake. (4) Look for the latest available update by LANL and include that in this uptake. (5) Look for updates by DELP and SRIV for which the date is equal to the date for IHME. (6) If no new update by IHME is available (from step 1), check for new updates by IMPE. If a new update by IMPE is available, start a new uptake with today's date, and use this new update by IMPE. (7) Look for the latest available update by IHME and include that in this uptake. (8) Look for the latest available update by LANL and include that in this uptake. (9) Look for updates by DELP and SRIV for which the date is equal to the date for IMPE. (10) If no new update by IMPE is available (from step 6), there is no new uptake for this calendar date. 


<br/><br/>

### Abbreviations

CovidVisualizedCountry: Covid Visualized Country. A GitHub repository that was created in this work to visualize the COVID-19 epidemic models' estimates at country level – countries with subnational estimates, e.g., Canada

CovidVisualizedGlobal: Covid Visualized Global. A GitHub repository that was created in this work to visualize the COVID-19 epidemic models' estimates at global level

covir2: COVID Iran Review Number 2. A GitHub repository that was created in this work to visualize the COVID-19 epidemic models' estimates at country level – countries without subnational estimates, e.g., Iran

DELP: DELPHI. Differential Equations Lead to Predictions of Hospitalizations and Infections. COVID-19 pandemic model named DELPHI developed by Massachusetts Institute of Technology, Cambridge

IHME: Institute for Health Metrics and Evaluation. COVID-19 pandemic model by developed Institute for Health Metrics and Evaluation, Seattle

IMPE: Imperial. COVID-19 pandemic model developed by Imperial College, London

LANL: Los Alamos National Laboratories. COVID-19 pandemic model developed by Los Alamos National Laboratories, Los Alamos

SRIV: Srivastava, Ajitesh. COVID-19 pandemic model developed by Ajitesh Srivastava, University of Southern California, Los Angeles

WHO: World Health Organization 



<br/><br/>



### References

1. Pourmalek, F. pourmalek/CovidVisualizedGlobal: 1.1 public release. 2021. Zenodo. https://doi.org/10.5281/zenodo.5019030 Accessed 23 June 2021.
2. Pourmalek, F. pourmalek/CovidVisualizedCountry: 1.1 public release. 2021. Zenodo. http://doi.org/10.5281/zenodo.5019482 Accessed 23 June 2021.
3. Pourmalek, F. pourmalek/covir2: 2.2 public release. 2021. Zenodo. http://doi.org/10.5281/zenodo.5020797 Accessed 23 June 2021.
4. COVID Analytics. DELPHI epidemiological case predictions. Cambridge: Operations Research Center, Massachusetts Institute of Technology. https://www.covidanalytics.io/projections Accessed 23 June 2021. 
5. Institute for Health Metrics and Evaluation (IHME). COVID-19 mortality, infection, testing, hospital resource use, and social distancing projections. Seattle: Institute for Health Metrics and Evaluation (IHME), University of Washington. http://www.healthdata.org/covid/ Accessed 23 June 2021.
6. MRC Centre for Global Infectious Disease Analysis (MRC GIDA). Future scenarios of the healthcare burden of COVID-19 in low- or middle-income countries. London: MRC Centre for Global Infectious Disease Analysis, Imperial College London. https://mrc-ide.github.io/global-lmic-reports/ Accessed 23 June 2021.
7. Los Alamos National Laboratory (LANL). COVID-19 cases and deaths forecasts. Los Alamos: Los Alamos National Laboratory (LANL). https://covid-19.bsvgateway.org Accessed 23 June 2021.
8. Srivastava, Ajitesh. University of Southern California (USC). COVID-19 forecast. Los Angeles: University of Southern California. https://scc-usc.github.io/ReCOVER-COVID-19 and Accessed 23 June 2021.
9. Pourmalek F, Rezaei Hemami M, Janani L, Moradi-Lakeh M. Rapid review of COVID-19 epidemic estimation studies for Iran. BMC Public Health. 2021 Feb 1;21(1):257. doi: 10.1186/s12889-021-10183-3.
10. Vynnycky E, White R. An Introduction to Infectious Disease Modelling. Oxford University Press. 2010.
11. Fox MP, Gower EW. Infectious Disease Epidemiology. In: Lash TL, VanderWeele TJ, Haneause S, Rothman K. (Editors). Modern Epidemiology. Lippincott Williams & Wilkins. 2021.
12. Watts A. Deaths from COVID-19 are undercounted, WHO says. https://cnnphilippines.com/world/2020/9/5/covid-deaths-undercounted-WHO-says.html?fbclid=lwAR2 Accessed 23 June 2021. 
13. Russell TW, Golding N, Hellewell J, Abbott S, Wright L, et al; CMMID COVID-19 working group. Reconstructing the early global dynamics of under-ascertained COVID-19 cases and infections. BMC Med. 2020 Oct 22;18(1):332. doi: 10.1186/s12916-020-01790-9.
14. Bhatia S, Imai N, Cuomo-Dannenburg G, Baguelin M, Boonyasiri A, et al. Report 6: Relative sensitivity of international surveillance. Imperial College London COVID-19 Response Team. 21 February 2020. https://www.imperial.ac.uk/mrc-global-infectious-disease-analysis/covid-19/report-6-international-surveillance/ Accessed 23 June 2021. 
15. Melka AB, Louzoun Y. Evaluation of the number of undiagnosed infected in an outbreak using source of infection measurements. Sci Rep. 2021 Feb 11;11(1):3601. doi: 10.1038/s41598-021-82691-6. 
16. Buitrago-Garcia D, Egli-Gany D, Counotte MJ, Hossmann S, Imeri H, Ipekci AM, Salanti G, Low N. Occurrence and transmission potential of asymptomatic and presymptomatic SARS-CoV-2 infections: A living systematic review and meta-analysis. PLoS Med. 2020 Sep 22;17(9):e1003346. doi: 10.1371/journal.pmed.1003346.
17. COVID-19 Excess Mortality Collaborators. Estimating excess mortality due to the COVID-19 pandemic: a systematic analysis of COVID-19-related mortality, 2020-21. Lancet. 2022 Mar 10;S0140-6736(21)02796-3. doi: 10.1016/S0140-6736(21)02796-3.
18. Gandhi M, Yokoe DS, Havlir DV. Asymptomatic Transmission, the Achilles' Heel of Current Strategies to Control Covid-19. N Engl J Med. 2020 May 28;382(22):2158-2160. doi: 10.1056/NEJMe2009758. Epub 2020 Apr 24.
19. Saad-Roy CM, Wingreen NS, Levin SA, Grenfell BT. Dynamics in a simple evolutionary-epidemiological model for the evolution of an initial asymptomatic infection stage. Proc Natl Acad Sci U S A. 2020 May 26;117(21):11541-11550. doi: 10.1073/pnas.1920761117. Epub 2020 May 8.
20. Rasmussen AL, Popescu SV. SARS-CoV-2 transmission without symptoms. Science. 2020 Mar 19:1206-1207.
21. Mecenas P, Bastos RTDRM, Vallinoto ACR, Normando D. Effects of temperature and humidity on the spread of COVID-19: A systematic review. PLoS One. 2020 Sep 18;15(9):e0238339. doi: 10.1371/journal.pone.0238339. eCollection 2020.
22. Park S, Lee Y, Michelow IC, Choe YJ. Global Seasonality of Human Coronaviruses: A Systematic Review. Open Forum Infect Dis. 2020 Oct 18;7(11):ofaa443. doi: 10.1093/ofid/ofaa443. eCollection 2020 Nov.
23. Bukhari Q, Massaro JM, D'Agostino RB Sr, Khan S. Effects of Weather on Coronavirus Pandemic. Int J Environ Res Public Health. 2020 Jul 27;17(15):5399. doi: 10.3390/ijerph17155399.
24. Tregoning JS, Flight KE, Higham SL, Wang Z, Pierce BF. Progress of the COVID-19 vaccine effort: viruses, vaccines and variants versus efficacy, effectiveness and escape. Nat Rev Immunol. 2021 Oct;21(10):626-636. doi: 10.1038/s41577-021-00592-1. Epub 2021 Aug 9.
25. Caldwell JM, Le X, McIntosh L, Meehan MT, Ogunlade S, et al. Vaccines and variants: Modelling insights into emerging issues in COVID-19 epidemiology. Paediatr Respir Rev. 2021 Sep;39:32-39. doi: 10.1016/j.prrv.2021.07.002. Epub 2021 Jul 21.
26. Eker, S. Validity and usefulness of COVID-19 models. Humanit Soc Sci Commun. 2020. 7, 54. https://doi.org/10.1057/s41599-020-00553-4
27. Johns Hopkins University Center for Systems Science and Engineering. COVID-19 Data Repository. https://github.com/CSSEGISandData/COVID-19 Accessed 23 June 2021.



<br/><br/>


<br/><br/>


<br/><br/>



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

Appendix Graph 1. Iran, Predicted total deaths, DELP model. || Source: https://covidanalytics.io/projections Accessed on March 7, 2022.

![image](https://user-images.githubusercontent.com/30849720/159105023-fc8e5a43-5859-4caa-87d7-4c1f5454492b.png)

this

![image](https://user-images.githubusercontent.com/30849720/159105099-698afdad-5192-4dfd-b590-65913a9d5c01.png)

 









Appendix Graph 2. Iran, Predicted total cases, DELP model. || Source: https://covidanalytics.io/projections Accessed on March 7, 2022.

 





<br/><br/>

IHME model

The IHME model does not present predictions of daily cases. They provide predictions of daily infections. See Appendix Graphs 3 and 4 below. 


Appendix Graph 3. Iran, Predicted daily deaths, IHME model. || Source: https://covid19.healthdata.org/iran-(islamic-republic-of)?view=daily-deaths&tab=trend Accessed on March 7, 2022.

 









Appendix Graph 4. Iran, Predicted daily infections, IHME model. || Source: https://covid19.healthdata.org/iran-(islamic-republic-of)?view=infections-testing&tab=trend&test=infections Accessed on March 7, 2022.

 














<br/><br/>

IMPE model

The IMPE model does not present predictions of daily cases. They provide predictions of daily infections. See Appendix Graphs 5 and 6 below. 


Appendix Graph 5. Iran, Predicted daily deaths, IMPE model. || Source: https://raw.githubusercontent.com/mrc-ide/global-lmic-reports/master/IRN/index.pdf Page 4. Accessed on March 7, 2022.

 
Appendix Graph 6. Iran, Predicted daily infections, IMPE model. || Source: https://raw.githubusercontent.com/mrc-ide/global-lmic-reports/master/IRN/index.pdf Page 2. Accessed on March 7, 2022.

 

<br/><br/>

LANL model

The LANL COVID-19 Team made its last real-time forecast on September 27th, 2021. || Source: https://covid-19.bsvgateway.org Accessed on March 7, 2022.






<br/><br/>

SRIV model

The SRIV model’s predictions for daily deaths and daily cases are shown in Appendix Graphs 7 and 8 below. 

Appendix Graph 7. Iran, Predicted daily deaths, SRIV model.|| Source: https://scc-usc.github.io/ReCOVER-COVID-19 Accessed on March 7, 2022.

 







Appendix Graph 8. Iran, Predicted daily cases, SRIV model|| Source: https://scc-usc.github.io/ReCOVER-COVID-19 . Accessed on March 7, 2022.

 












<br/><br/>

Johns Hopkins compilation of official reports

The Johns Hopkins compilation of official reports does not present daily deaths and daily cases (as of March 7, 2022). They provide weekly deaths and weekly cases. See Appendix Graphs 9 and 10 below. 


Appendix Graph 9. Iran, Weekly reported deaths, Johns Hopkins. || Source: https://www.arcgis.com/apps/dashboards/bda7594740fd40299423467b48e9ecf6 Accessed on March 7, 2022.

 







Appendix Graph 10. Iran, Weekly reported cases, Johns Hopkins. || Source: https://www.arcgis.com/apps/dashboards/bda7594740fd40299423467b48e9ecf6 Accessed on March 7, 2022.   

 














<br/><br/>

Worldometers compilation of official reports to WHO

The Worldometers compilation of official reports provides daily deaths and cases, shown in Appendix Graphs 11 and 12 below. 

Appendix Graph 11. Iran, Daily deaths, Worldometers. Accessed on March 7, 2022. https://www.worldometers.info/coronavirus/country/iran/ 
 








Appendix Graph 12. Iran, Daily cases, Worldometers. Accessed on March 7, 2022. https://www.worldometers.info/coronavirus/country/iran/ 

 




<br/><br/>

Compile the graphs from individual models

The DELP model does not present predictions of daily deaths and daily cases. Predictions of daily deaths by IHME, IMPE, and SRIV and reported daily deaths by Worldometers are shown below in Appendix Graph 13. Appendix Graph 14 shows the predicted daily cases by SRIV, predicted daily infections by IHME and IMPE, and the reported daily cases by Worldometers. 

 

Appendix Graph 13. Iran predicted daily deaths by IHME, IMPE, SRIV and reported daily deaths by Worldometers. Accessed on March 7, 2022. || Source: Assembled from Appendix Graphs 3, 5, 7, and 11.

 

Appendix Graph 14. Iran, predicted daily cases by SRIV, predicted daily infections by IHME and IMPE, and reported daily cases, Worldometers. Accessed on March 7, 2022. || Source: Assembled from Appendix Graphs 4, 6, 8, and 12.

  
  
<br/><br/>

How can the covir2 tool be practically used for the example of a researcher or advisor to policymakers who wanted to examine the latest predictions for the future trajectory of the COVID-19 epidemic in Iran on March 7, 2022? They would look at the uptake dates on the covir2 website to find the latest date equal to or before March 7, 2022. The uptake dates in the covir2 website are displayed on the top of the main web page as the names of directories for each uptake (see Appendix Exhibit 1 below). Scroll down to find the latest uptake date equal to or before March 7, 2022. Appendix Exhibit 2 shows that the date would be 20220304. Clicking on the hyperlinked name 20220304 leads to the page for the uptake 20220304 (see Appendix Exhibit 3). On the page for the uptake 20220304, “Selected graphs” can be viewed, as well as links to the code  used to produce the results and the output  of the code. 


<br/><br/>

Appendix Graphs 15 to 33 (below) show what can be found for uptake 20220304 on the covir2 website. Official reports by the country are demonstrated as the curves drawn from the Johns Hopkins University compilation (abbreviated in the graphs as “JOHN”). 

<br/><br/>

Appendix Graph 15 shows all models’ predictions by all models for Daily deaths, all-time, i.e., from January 2020 to the latest date available in the models. Appendix Graph 16 focuses on more recent times, i.e.,  2021 on. Appendix graphs 17 and 18 look in more detail at the IHME model predictions. Appendix Graph 17 shows predicted Daily deaths, 2021 on, reference scenario with uncertainty, IHME, and Appendix Graph 18 shows predicted Daily deaths, 2021 on, all scenarios, IHME. Appendix graphs 19 and 20 look in more detail at the IMPE model predictions. 


<br/><br/>

For the second outcome, i.e., daily cases, Appendix Graph 21 shows the predicted Daily cases or infections, all-time, and Appendix Graph 22 shows the predicted Daily cases or infections, 2021 on. Appendix Graph 23 demonstrates the predicted Daily cases, 2021 on, without the predicted infections. The values of the predicted infections are much higher than those for the predicted cases. When in the same graph, infections’ curves visually compress the cases’ curves. When the predicted cases are shown without the predicted infections, one can appreciate their trajectory and compare them with the past trends. 

<br/><br/>

Appendix Graphs 24 to 33 demonstrate additional outcomes and variables. Appendix Graph 24 depicts the secondary (i.e., calculated) variable Daily estimated infections IHME, IMPE to reported cases JOHN, main scenarios, 2021 on. This graph provides a gauge of how much more are the predicted infections compared with predicted cases, across time and models – a technical epidemiological and modelling insight. This graph does not have a readily accessible similar on the web, as far as I know. 

<br/><br/>

Appendix Graphs 25 and 26 provide predicted hospital-related outcomes. Appendix Graph 25 shows all the Hospital-related outcomes, all-time and by all models. Appendix Graph 26 removes the outcomes whose larger values compress the curves of outcomes with lower values and focuses on more recent time interval. There are no readily accessible similar graphs on the web as far as I know. 

Appendix Graph 27 depicts how many times more are the precited deaths compared with the reported deaths across time and models. Appendix Graph 28 shows a similar secondary (i.e., calculated) variable for the cases or infections – a technical epidemiological and modelling insight, with no ongoingly updated similar graphs on the web as far as I know.

Appendix Graphs 29 to 33 show additional variables estimated by the IHME model: Appendix Graph 29, R effective, 2 scenarios, 2021 on, IHME; Appendix Graph 30, Daily Infection-outcome ratios, 2 scenarios, 2021 onwards, IHME; Appendix Graph 31, Daily mobility, 2 scenarios, all-time, IHME; Appendix Graph 32, Daily mask use, 2 scenarios, all-time, IHME; and Appendix Graph 33, Percent cumulative vaccinated, 2021 on, IHME.


<br/><br/>

Here is the bottom-line conclusion from this example of a researcher or advisor to policymakers who wanted to examine the latest predictions for the future trajectory of the COVID-19 epidemic in Iran on March 7, 2022 – and how the covir2 tool can help. One can locate the latest predictions by the international and periodically updated models and come up with some sort of compilation of graphs like the Appendix Graphs 13 and 14 made here, or similar graphs for other outcomes. In the meantime, the Appendix Graphs 15 to 23 are equivalent to those graphs' compilations, readily available via the covir2 tool. The latter graphs are much more usable and demonstrate different aspects like calendar time intervals, different scenarios, mean estimates and confidence intervals, and individual models’ details. The software code used to produce the graphs is accessible  and can be rerun by others to verify the correctness and potential mistakes. The track record of the previous periodical uptakes is also accessible (via RESULTS 2021 and RESULTS 2022 for covir2, for instance). The covir2 uptake 20220311 also adds the following summary by its creator, and puts all the graphs in “Iran COVID-19 epidemic models situation report No 48 – 2022-03-11.pdf”.

<br/><br/>

Summary 20220311:
 
The New Year ceremonies and travels increase the number of contacts and the probability of transmission and spread of the virus across the country. These factors are not fully included in the models. As such, a new surge could be expected in Iran in March and April.




Appendix Exhibit 1. The uptake dates in the covir2 website are displayed on the top of the main web page as the names of directories for each uptake. || Source: https://github.com/pourmalek/covir2 Accessed on March 7, 2022.

 















Appendix Exhibit 2. The latest uptake date equal to or before March 7, 2022, is 20220304.
|| Source: https://github.com/pourmalek/covir2 Accessed on March 14, 2022.

 











Appendix Exhibit 3. The covir2 website page for uptake 20220304. || Source: https://github.com/pourmalek/covir2/tree/main/20220304 Accessed on March 7, 2022.

 










Appendix Graph 15. Iran Daily deaths, all-time || Source: covir2 uptake 20220304 Accessed on March 7, 2022.
 
Appendix Graph 16. Iran Daily deaths, 2021 on || Source: covir2 uptake 20220304 Accessed on March 7, 2022.
 
Appendix Graph 17. Iran Daily deaths, 2021 on, reference scenario with uncertainty, IHME || Source: covir2 uptake 20220304 Accessed on March 7, 2022.
 
Appendix Graph 18. Iran Daily deaths, 2021 on, all scenarios, IHME || Source: covir2 uptake 20220304 Accessed on March 7, 2022.
 
Appendix Graph 19. Iran Daily deaths, 2021 on, reference scenario with uncertainty, IMPE || Source: covir2 uptake 20220304 Accessed on March 7, 2022.
 
Appendix Graph 20. Iran Daily deaths, 2021 on, 3 scenarios, IMPE || Source: covir2 uptake 20220304 Accessed on March 7, 2022.
 
Appendix Graph 21. Iran Daily cases or infections, all-time || Source: covir2 uptake 20220304 Accessed on March 7, 2022.
 
Appendix Graph 22. Iran Daily cases or infections, 2021 on || Source: covir2 uptake 20220304 Accessed on March 7, 2022.
 
Appendix Graph 23. Iran Daily cases, 2021 on || Source: covir2 uptake 20220304 Accessed on March 7, 2022.
 
Appendix Graph 24. Iran Daily estimated infections IHME, IMPE to reported cases JOHN, main scenarios, 2021 on || Source: covir2 uptake 20220304 Accessed on March 7, 2022.
 
Appendix Graph 25. Iran Hospital-related outcomes, all-time || Source: covir2 uptake 20220304 Accessed on March 7, 2022.
 
Appendix Graph 26. Iran Hospital-related outcomes, 2021 on || Source: covir2 uptake 20220304 Accessed on March 7, 2022.
 
Appendix Graph 27. Iran Daily deaths estimated to reported, all-time || Source: covir2 uptake 20220304 Accessed on March 7, 2022.
 
Appendix Graph 28. Iran Daily cases or infections estimated to reported cases, 2021 on || Source: covir2 uptake 20220304 Accessed on March 7, 2022.
 
Appendix Graph 29. Iran R effective, 2 scenarios, 2021 on, IHME || Source: covir2 uptake 20220304 Accessed on March 7, 2022.
 
Appendix Graph 30. Iran Daily Infection-outcome ratios, 2 scenarios, 2021 on, IHME || Source: covir2 uptake 20220304 Accessed on March 7, 2022.
 
Appendix Graph 31. Iran Daily mobility, 2 scenarios, all-time, IHME || Source: covir2 uptake 20220304 Accessed on March 7, 2022.
 
Appendix Graph 32. Iran Daily mask use, 2 scenarios, all-time, IHME || Source: covir2 uptake 20220304 Accessed on March 7, 2022.
 
Appendix Graph 33. Iran Percent cumulative vaccinated, 2021 on, IHME || Source: covir2 uptake 20220304 Accessed on March 7, 2022.
 














<br/><br/>

### Example 2: Canada and its province

Below is a real-life example that explains what a researcher or advisor to policymakers would have needed to do if they wanted to examine the latest predictions by the international and periodically updated models for the future trajectory of the COVID-19 epidemic in Canada and its provinces and territories, on March 14, 2022. 

To examine the latest predictions of daily deaths and daily cases in Canada and its subnational levels by the international and periodically updated models, one needs to identify the models, locate their websites, find the graphs, create the missing graphs, (redevelop the available graphs), and compile the graphs. I tried to replicate the above steps, and the results are presented below. 



<br/><br/>

DELP model

The DELP model does not present daily deaths and daily cases predictions – they provide total deaths and total cases. The DELP model provides predictions for nine provinces: Alberta, British Columbia, Manitoba, New Brunswick, Newfoundland and Labrador, Nova Scotia, Ontario, Quebec, and Saskatchewan. Appendix Graphs 34 and 35 show their predictions for Canada at the national level. Appendix Graphs 36 and 37 show DELP predictions for British Columbia, for instance. 






Appendix Graph 34. Canada, national level, Predicted total deaths, DELP model. || Source: https://covidanalytics.io/projections Accessed on March 14, 2022.

 










Appendix Graph 35. Canada, national level, Predicted total cases, DELP model. || Source: https://covidanalytics.io/projections Accessed on March 14, 2022.

 











Appendix Graph 36. Canada, British Columbia, Predicted total deaths, DELP model. || Source: https://covidanalytics.io/projections Accessed on March 14, 2022.

 











Appendix Graph 37. Canada, British Columbia, Predicted total cases, DELP model. || Source: https://covidanalytics.io/projections Accessed on March 14, 2022.

 










<br/><br/>

IHME model

The IHME model does not present predictions of daily cases. They provide predictions of daily infections. See Appendix Graphs 38 and 39 below. IHME provides predictions for seven provinces: Alberta, British Columbia, Manitoba, Nova Scotia, Ontario, Quebec, and Saskatchewan. Appendix Graphs 40 and 41 show IHME predictions for British Columbia, for instance. 


Appendix Graph 38. Canada, national level, Predicted daily deaths, IHME model. || Source: https://covid19.healthdata.org/canada?view=daily-deaths&tab=trend Accessed on March 14, 2022.

 




Appendix Graph 39. Canada, national level, Predicted daily infections, IHME model. || Source: https://covid19.healthdata.org/canada?view=infections-testing&tab=trend&test=infections Accessed on March 14, 2022.

 













Appendix Graph 40. Canada, British Columbia, Predicted daily deaths, IHME model. || Source: https://covid19.healthdata.org/canada/british-columbia?view=daily-deaths&tab=trend Accessed on March 14, 2022.

 













Appendix Graph 41. Canada, British Columbia, Predicted daily infections, IHME model. || Source: https://covid19.healthdata.org/canada/british-columbia?view=infections-testing&tab=trend&test=infections Accessed on March 14, 2022.

 














<br/><br/>

IMPE model

The IMPE model does not present predictions of daily cases. They provide predictions of daily infections. IMPE model does not provide predictions for the subnational levels. Appendix Graphs 42 and 43 show predictions for Canada. 


Appendix Graph 42. Canada, Predicted daily deaths, IMPE model. || Source: https://raw.githubusercontent.com/mrc-ide/global-lmic-reports/master/CAN/index.pdf Accessed on March 14, 2022.
 



Appendix Graph 43. Canada, Predicted daily infections, IMPE model. || Source: https://raw.githubusercontent.com/mrc-ide/global-lmic-reports/master/CAN/index.pdf Page 2. Accessed on March 14, 2022.

 



<br/><br/>

LANL model

The LANL COVID-19 Team made its last real-time forecast on September 27th, 2021. || Source: https://covid-19.bsvgateway.org Accessed on March 14, 2022.




<br/><br/>

SRIV model

The SRIV model’s predictions for daily deaths and daily cases are shown in Appendix Graphs 44 and 45 below. SRIV model does not provide predictions for the subnational levels. 



Appendix Graph 44. Canada, Predicted daily deaths, SRIV model.|| Source: https://scc-usc.github.io/ReCOVER-COVID-19 Accessed on March 14, 2022.

 






Appendix Graph 45. Canada, Predicted daily cases, SRIV model|| Source: https://scc-usc.github.io/ReCOVER-COVID-19 . Accessed on March 14, 2022.

 












<br/><br/>

Johns Hopkins compilation of official reports

The Johns Hopkins compilation of official reports does not present daily deaths and daily cases (as of March 14, 2022). They provide weekly deaths and weekly cases. See Appendix Graphs 46 and 47 below. 



Appendix Graph 46. Canada, Weekly reported deaths, Johns Hopkins. || Source: https://www.arcgis.com/apps/dashboards/bda7594740fd40299423467b48e9ecf6 Accessed on March 14, 2022.

 








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





