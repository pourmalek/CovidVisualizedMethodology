# CovidVisualizedMethodology
CovidVisualized Methodology Documents


This repository contains the CovidVisualized Methodology Documents:

CovidVisualized Methodology Document

CovidVisualized Methodology Document Appendix


<br/><br/>

CovidVisualized Methodology Document:

This CovidVisualized methodology document explains the conceptual and computational details of the development of CovidVisualized tools. Examples of “what the CovidVisualized tools provide in addition to the individual models” are provided in the companion “CovidVisualized methodology document appendix”. 

<br/><br/>

CovidVisualized Methodology Document Appendix:


This CovidVisualized Methodology Document Appendix provides examples of how the CovidVisualized tools can be used to examine the predictions by the international and periodically updated epidemic models for the future trajectory of the COVID-19 pandemic at global and country levels.

<br/><br/>



### CovidVisualized Methodology Document

Methodology document for CovidVisualized tools: CovidVisualizedGlobal, CovidVisualizedCountry, and covir2

CovidVisualized: Visualized compilation of international updated models' estimates of COVID-19 pandemic at global and country levels

Farshad Pourmalek, MD PhD
Former lecturer, University of British Columbia, Vancouver, Canada
pourmalek_farshad at yahoo dot com


### TABLE OF CONTENTS:

[Summary](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#summary)

[CovidVisualized tools](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#covidvisualized-tools)

[International and periodically updated COVId-19 pandemic models](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#international-and-periodically-updated-covid-19-pandemic-models)

[Study justification and added value](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#study-justification-and-added-value)

[Characteristics of the models](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#characteristics-of-the-models)

[Data management](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#data-management)

[Primary and secondary variables]()

[Smoothing](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#smoothing)

[Models’ scenarios]()

[Models’ versions]()

[Periodical updates and uptakes](https://github.com/pourmalek/CovidVisualizedMethodology/blob/main/README.md#periodical-updates-and-uptakes)




### Summary

This CovidVisualized methodology document explains the conceptual and computational details of the development of CovidVisualized tools. Examples of “what the CovidVisualized tools provide in addition to the individual models” are provided in the companion “CovidVisualized methodology document appendix”. 


### CovidVisualized tools

There are three CovidVisualized tools:
(1) CovidVisualizedGlobal: Combine and visualize international periodically updated estimates of COVID-19 pandemic at the global level and six WHO regions [1]
https://github.com/pourmalek/CovidVisualizedGlobal 
(2) CovidVisualizedCountry: Combine and visualize international periodically updated estimates of COVID-19 pandemic at the country level: Canada, national and subnational [2]
https://github.com/pourmalek/CovidVisualizedCountry 
(3) covir2: Combine and visualize international periodically updated estimates of COVID-19 pandemic at the country level, countries without subnational level estimates: Iran [3]
https://github.com/pourmalek/covir2 

### International and periodically updated COVId-19 pandemic models

The five international and periodically updated COVId-19 pandemic models included in this work are (1) DELPHI , Massachusetts Institute of Technology, Cambridge (abbreviation used in this work: DELP) [4], (2) Institute for Health Metrics and Evaluation, Seattle (IHME) [5], (3) Imperial College, London (IMPE) [6], (4) Los Alamos National Laboratories, Los Alamos (LANL) [7], (5) University of Southern California, Los Angeles, by Srivastava, Ajitesh (SRIV) [8].


### Study justification and added value

What is missing from the individual international and periodically updated models that creation of the CovidVisualized tools [1-3] was needed? Nothing substantial is missing from the individual (international and periodically updated) models. However, some of those models do not report predictions of daily outcomes or do not provide the predictions at the global or regional levels. Suppose that a researcher or advisor to policymakers wants to look at the latest predictions by all international and periodically updated models for any given country or location (e.g., Canada and its provinces, or the European region). In that case, they need to know or find the website addresses for graphs and data of each model, find the graphs that are available on the websites for the models, develop the graphs that are not available, and put together and examine the graphs that use different horizontal (time) and vertical (outcome) axes. If they want to repeat this, they will need to repeat all the steps, which is time-consuming. The CovidVisualized tools have consistently performed the steps mentioned above and compiled the graphs (and data) from individual models together in a usable framework and continue to do so regularly. 

The obstacles: The obstacles one would encounter in examining the latest predictions by all international and periodically updated models for any given country or location are mentioned below. (1) The DELP model [4] does not provide predictions of daily deaths and daily cases. One needs to calculate them from the provided total deaths and total cases. (2) The IMPE model [6] graphs for predicted daily deaths at the continent level and daily infections at the global and continent levels are not readily locatable. (3) The SRIV model [8] does not provide global and continent-level graphs. (4) The researcher-made compilations of available graphs from different models are not practically usable because (a) the graphs from each model use different calendar time intervals and time bins, (b) the maximum value on the y-axis for the same outcome (e.g., daily deaths) are different across models, (c) uncertainty intervals and alternate scenarios are not shown by all the models. (5) Not all models provide graphs for all the variables they predict, e.g., hospital-related outcomes. (6) The predictions’ data files that each model provides follow that model’s unique data arrangements. These data arrangements differ across the models. Without a common data management template, it is impossible to acquire a grip on the models’ data that can lead to the creation of compiled data and graphs. 

Creation of the missing graphs and redeveloping the available graphs need a data management framework capable of compiling data (predictions’ files) from different models. While all the models present a set of common outcomes and variables, they do so in their unique way. The number of data files, the variables and data structure within each file, the nomenclature and variable names, the geographical locations covered by each model, the alternative scenarios, and many other aspects of the predictions provided by the models vary tremendously across the models. Moreover, within each model, there are systematic and random variations and alterations regarding these aspects across time (i.e., with updates released by the model). The CovidVisualized tools [1-3] have covered these issues in a reproducible way, i.e., researchers can download the codes, rerun them, and see the outputs and results. The CovidVisualized tools have already paved the way and resolved the obstacles in examining the predictions in a coherent, consistent, and periodically updated framework, with underlying software codes and outputs. 





 
### Characteristics of the models

General characteristics of the five international and periodically updated COVID-19 pandemic models included in this work are described below in Appendix Table 1. These characteristics are taken from a “Rapid review of COVID-19 epidemic estimation studies for Iran” [9]. 

No model is 100% complete, accurate, and valid, and no model is 100% wrong and useless. As described by Vynnycky  and White, models identify the essential elements which determine real life behaviour of the epidemic (i.e., the model assumptions) and then properly include those elements in the model structure and calculations. If these essential elements are identified and incorporated wisely then the model may provide realistic predictions [10] [25]. The first three essential elements of the COVID-19 epidemic are (1) under-reporting of deaths and cases [11-17] [26-32], (2) asymptomatic transmission [11, 18-20] [26, 33-35], and (3) seasonality [21-23] [36-38]. The foreseeable advent of vaccines and variants shifted the epidemiologic landscape of the disease transmission, and hence vaccines and variants belong among the essential elements of the epidemic [24-25] [39-40]. Including alternate scenarios in the models can be quite illustrative and useful for policymakers about future trends in the epidemic and potential role of the interventions [26] [41]. The above-mentioned technical characteristics of the models are mentioned in Appendix Table 2. The whole set of model’s characteristics provides a profile of models’ strengths and weaknesses – that should be considered while examining the predictions by models. 
 
Table 1. General characteristics of the included models 

Study / Model	DELP [4]	IHME [5]	IMPE [6]	LANL [7]	SRIV [8]
Compartmental model (a)	SEIR+	SEIR	SIR, SEIR, SEIR+	SEIR+	SIR+
Statistical methods	Regression trees	Spline fit and excess mortality estimation	Regression trees	Dynamic growth parameter modeling	Hyper-parametric learning
Scenarios number	1	3-5	6	1	3
Primary outcomes	Total deaths and cases	Total and daily deaths and infections	Total and daily deaths and infections	Total and daily deaths and cases	Total deaths and cases
Locations (in data)	National, subnational	Global, regional, national, subnational	National	National	National
Locations (in graphs)	Global, continental, national, 
subnational	Global, regional, national, subnational	Global, (b) National (c)	National	National (and US states)
(a) Compartmental models: S: Susceptible, E: Exposed, I: Infected, R: Removed or Recovered, L: Latent. In any model with a + sign, there are other components for augmentation of model. (b) Global daily deaths only. (c) National daily deaths and infections only. 





Table 2. Technical characteristics of the included models 

Study / Model	DELP [4]	IHME [5]	IMPE [6]	LANL [7]	SRIV [8]
Adjusting for under-reporting	Yes	Yes	Yes	No	Yes
Including asymptomatic transmission	Yes	No	Yes	No	Yes
Including seasonal variations 	Yes	Yes	No	No	No
Model validation by creators	Yes	Yes	Yes	No	Yes
Alternate scenarios	No	Yes	Yes	No	No
Including vaccines	Unknown	Yes	Yes	Unknown	Unknown
Including variants	Unknown	Yes	Yes	Unknown	Unknown










### Data management 

Estimates of (1) Daily Deaths, (2) Total Deaths, (3) Daily Cases (incident or prevalent), and (4) Total Cases (incident) from the five models are the primary outcome variables of interest in this work. Hospital-related and other outcomes from the five models are the secondary outcome variables.

The CovidVisualized tools do not change any outcomes or variables taken from the five international and periodically updated models. Secondary variables are calculated in CovidVisualized tools: (1) Daily deaths and daily cases are calculated from the provided cumulative deaths and cases by JOHN [27], DELP [4], and SRIV [8]. (2) Case Fatality Ratios (CFR), and (3) smoothed variables for daily deaths daily cases from JOHN and DELP. Details of smoothing are provided further below. 

### Primary and secondary variables

Primary variables are taken from the five models. Secondary variables are calculated in this work. To facilitate data management, the primary variables were -rename-d or -renvar-ed using the variables from the five models according to the following conventions. The same set of conventions was adhered to in naming all outcome variables.

Primary variables include primary outcome variables, i.e., deaths and cases, and secondary outcome variables, e.g., hospital demand. As described below through examples, primary variable names have six parts, each part denoting one piece of information about the variable. All the variables have descriptive var -label-s that show what the variable stores. Stata commands are displayed as -command- and Stata non-command syntax as -syntax-. 



Variable names
Primary outcome variable names:
Example:
TotDeaMeRaA01S00
1234567890123456
-varname- has 16 positions.
Tot...Dea...Me....Ra.....A01.....S00
1-3...4-6...7-8...9-10...11-13...14-16 


•	Positions 1-3: Tot or Day: Total (cumulative) or Daily
•	Positions 4-6: Dea, Cas, or Act: Dea for Deaths, Cas for incident Cases, or Act for Active cases (for primary outcomes; for secondary outcomes, see below)
•	Positions 7-8: Me, Lo, or Up: Mean, Lower, or Upper (uncertainty bound)
•	Positions 9-10: Ra or Sm: Raw (not smoothed) or Smoothed
•	Positions 11-13: A00 to A05: Model number (see details below)
•	Positions 14-16 S??: Scenario number within the model (see details below)
The example primary variable name, TotDeaMeRaA01S00, denotes Total Deaths, mean, raw, DELPHI, single scenario.

Secondary outcome variable names:
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


Secondary variable names:
Secondary variables have two subtypes: (1) variable that store a calculated daily Case Fatality Ratio (CFR), (1) variable that store values created to visualize temporal succession of daily cases and daily deaths peaks.


(1) store a calculated daily CFR
•	Positions 4-6 read as CFR.
Example:
DayCfrMeRaA00S00V00 "Daily CFR JOHN [27]" 

(2) store values created for visualization of temporal succession of daily cases and daily deaths peaks
•	CaM: (Cases Mean) "Daily Cases Mean" 
•	CbD (Cases by Deaths) "Daily cases mean divided by daily deaths mean JOHN" 
•	DeM: (Deaths Mean) "Daily Deaths Mean "


### Smoothing

Smoothed outcomes are useful for visualization when the raw outcomes are jagged because of day-to-day fluctuations and weekend patterns in reporting. This is true for reported daily deaths and reported daily cases (JOHN) [27]. It is also true for predicted daily deaths and predicted daily cases or infections in the time interval before a model update, i.e., when a model is backcating the daily outcomes in the past. 

The DELP model [4] does not provide smoothed version of predicted daily variables. Therefore, smoothing is performed in CovidVisualized tools. The IHME model [5] provides smoothed version of predicted daily variables. Their smoothed version of predicted daily variables is used for visualization. The IMPE [6] and LANL [7] models do not provide smoothed version of predicted daily variables. However, their raw (non-smoothed) version of daily outcomes is not very jaggy. Therefore, their raw version of daily outcomes is used in the graphs. The SRIV model [8] does not provide predictions for the past, and their predicted daily outcomes are used in the graphs. Official reports of daily death and daily cases (JOHN) are the prototype of outcomes for which adding the smoothed version is useful for visualization.   

In summary, smoothing is performed for daily deaths daily cases from JOHN and DELP. Moving averages are calculated for those raw daily deaths and raw daily cases, using the -tssmooth ma- command of Stata. The code and output segment used for smoothing the raw daily deaths from Johns Hopkins (variable name is DayDeaMeRaA00S00) is shown below. This segment is taken from: https://github.com/pourmalek/CovidVisualizedCountry/blob/main/20220311/code/JOHN/do%20CovidVisualizedCountry%20JOHN.do that is the -do- file for downloading and preparing the official reports from Johns Hopkins for Canada and its provinces in the uptake 20220311 of CovidVisualizedCountry tool. 

* Start of the code segment
. tssmooth ma DayDeaMeRaA00S00_window = DayDeaMeRaA00S00 if DayDeaMeRaA00S00 >= 0, window(3 1 3)
The smoother applied was
     by provincestate_encoded : (1/7)*[x(t-3) + x(t-2) + x(t-1) + 1*x(t) + x(t+1) + x(t+2) + x(t+3)]; x(t)= DayDeaMeRaA00S00
. tssmooth ma DayDeaMeSmA00S00 = DayDeaMeRaA00S00_window, weights( 1 2 3 <4> 3 2 1) replace
The smoother applied was
     by provincestate_encoded : (1/16)*[1*x(t-3) + 2*x(t-2) + 3*x(t-1) + 4*x(t) + 3*x(t+1) + 2*x(t+2) + ...; x(t)= DayDeaMeRaA00S00_window
* End of the code segment






Numbers assigned to the models in this work:

A00 JOHN Johns Hopkins [27]
A01 DELP DELPHI  [4]
A02 IHME Institute for Health Metrics and Evaluation [5]
A03 IMPE Imperial College [6]
A04 LANL Los Alamos National Laboratory [7]
A05 SRIV Srivastava [8]


### Models’ scenarios
Scenario numbers within the models: 
[Names within brackets are assigned in this work.]

A00 JOHN
S00 = [Not Applicable]

A01 DELP
S00 = [Single scenario]

A02 IHME  (see more details below)
All updates up to and including 20211217:
S01 = Reference scenario [Status Quo]
S02 = Best scenario (Universal masks) [Best]
S03 = Worse scenario (Mandates easing) [Worst] 


Updates 20211221 to 20220110:
S01 = Current projection [Status Quo, Reference scenario]
S02 = 80% mask use [Best scenario]
S03 = High severity of Omicron [Worse scenario]
S04 = Third dose of vaccine [Second best scenario]
S05 = Reduced vaccine hesitancy [Third best scenario] 

Updates 20220114 to 20220121:
S01 = Current projection [Status Quo, Reference scenario]
S02 = 80% mask use [Best scenario]
S04 = Third dose of vaccine [Second best scenario]
S05 = Reduced vaccine hesitancy [Third best scenario]
The previous scenario, "severe omicron," was omitted starting from update 20220114. The "current projection" or "reference scenario" is functionally the "worse scenario," i.e., the scenario with highest magnitude of estimated deaths and infections.

Updates 20220204 onwards:
S01 = Current projection [Status Quo, Reference scenario]
S02 = 80% mask use 
S03 = Third dose of vaccine [Second best scenario]

A03 IMPE
S01 = Additional 50% Reduction [Best]
S02 = Current level of interventions [Reference]
S03 = Relax Interventions 50% [Worst]
S04 = Surged Additional 50% Reduction [Best, Surged]
S05 = Surged Maintain Status Quo [Reference, Surged]
S06 = Surged Relax Interventions 50% [Worst, Surged]

A04 LANL
S00 = [Single scenario]

A05 SRIV
S00 = [current]


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



### Models’ versions

DELP model versions:
DELP V1 2020-04-17 to 2020-07-04
DELP V2 2020-07-04 to 2020-11-19
DLEP V3 (could not be located)
DELP V4 2020-11-19 to when specified otherwise
DELP source for model versions: 
https://github.com/COVIDAnalytics/website/tree/master/data/predicted

IHME model versions:
IHME V1 2020-03-25 to 2020-04-29: IHME-CF = Curve Fitting]
IHME V2 2020-05-04 to 2020-05-26: IHME-CF-SEIR = Curve Fitting and SEIR
IHME V3 2020-05-29 to 2021-04-30: IHME-MS-SEIR = Mortality Spline and SEIR
IHME V4 2021-05-06 to 2022-01-10: IHME-MS-SEIR + Total Covid-19 Mortality 
IHME V5 2022-01-14 onwards: IHME-MS-SEIR + Total Covid-19 Mortality + Waning immunity, Fitting the past (improved methods), and Omicron specific changes


IHME source for model versions: 
All models label their versions within their data files or on their websites, except the IHME model. The first three versions of the IHME have been described in [2]. Since May 2021, they changed their key metric from reported deaths to the total number of COVID-19 deaths [32]. This included estimation of the ratio of the total number of COVID-19 death to reported deaths from COVID-19. Hence, the IHME model is labelled V4, in this work, starting from May 6, 2021.

V1: Beginning March 25, IHME initially produced COVID forecasts using a statistical curve fit model (IHME-CF), which was used through April 29 for publicly released forecasts. V2: On May 4, IHME switched to using a hybrid model, drawing on a statistical curve fit in the first stage, followed by a second-stage epidemiological model with susceptible, exposed, infectious, recovered compartments (SEIR). This model was used through May 26. V3: On May 29, the curve fit stage was replaced by a spline fit to the relationship between log cumulative deaths and log cumulative cases, while the second-stage SEIR model remained the same.

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

LANL model versions:
LANL V1 2020-04-05 to 2020-10-28
LANL V2 2020-10-28 to 2021-09-26
LANL source for model versions: https://covid-19.bsvgateway.org 
The LANL COVID-19 Team made its last real-time forecast on September 27th, 2021. 
Source: https://covid-19.bsvgateway.org

SRIV model versions:
SRIV V1 2020-05-02 to 2020-06-02 
SRIV V2 2020-06-03 to when specified otherwise
SRIV source for model versions: 
https://github.com/scc-usc/ReCOVER-COVID-19#our-papers and 
https://github.com/scc-usc/ReCOVER-COVID-19/tree/master/results/historical_forecasts

***

Models’ websites for estimates files
DELP https://github.com/COVIDAnalytics/website/tree/master/data/predicted
IHME http://www.healthdata.org/covid/data-downloads
IMPE https://github.com/mrc-ide/global-lmic-reports/tree/master/data
LANL https://covid-19.bsvgateway.org
SRIV https://github.com/scc-usc/ReCOVER-COVID-19/tree/master/results/historical_forecasts
JOHN https://github.com/CSSEGISandData/COVID-19 


Models’ websites for graphs
DELP https://covidanalytics.io/projections
IHME https://covid19.healthdata.org/iran-(islamic-republic-of)?view=cumulative-deaths&tab=trend
IMPE https://github.com/mrc-ide/global-lmic-reports/tree/master/IRN
LANL https://covid-19.bsvgateway.org  
SRIV https://scc-usc.github.io/ReCOVER-COVID-19/
JOHN https://www.arcgis.com/apps/dashboards/bda7594740fd40299423467b48e9ecf6
 
 
 
 
 
### Periodical updates and uptakes


Model updates, estimates updates, and CovidVisualized uptakes

With daily accumulation of official country reports to WHO, curated by the Johns Hopkins University [27] and other curators, and other data types used in the models, models update their estimations (predictions) on a rather regular basis. The CovidVisualized tools [1-3] use the estimations updates released by the models on a regular basis. To semantically differentiate between what is released by the models and what is performed by the CovidVisualized tools, the latter is labeled “uptake”. Updates belong to the models. Uptakes belong to the CovidVisualized tools. Updates are released by the model creators. Uptakes are added to CovidVisualized tools by its creator.

The two models with the least frequency of periodic updates of estimates are IHME [5] and IMPE [6], updated almost weekly and bi-weekly, respectively – until November 2021. After spread of the Omicron variants, these models reduced the frequency of their update releases. Therefore, two sets of arrangements ruled the frequency of performing uptakes in the CovidVisualized tools [1-3]. The first set covered the year 2021: With the release of each update of either of these two models, the whole set of the five included models is updated in all the three CovidVisualized GitHub repositories. The most recent update of each model is used. The conventions for periodical uptake are described in more detail below. Estimates of the LANL model [7] get updated about every 3-4 days, and DELP [4] and SRIV [8] models get updated daily. The second set of arrangements for the frequency of performing uptakes in the CovidVisualized tools started in 2022. Uptakes are performed each week on Friday. Each uptake uses the latest available update of each model.  



With much less frequency than that of models’ estimations updates releases, models improve their internal and calculations structures. These are “model versions” that are distinct from models’ estimations updates. Model versions are described in detail below. 

Detailed description of the of rule for uptakes of CovidVisualized tools in 2021

This is a description of the rule of adding uptakes to CovidVisualized tools [1-3]. The overarching principle for creating uptakes is to create an uptake for each calendar date on which an update is available for either IHME [5] or IMPE [6] and using the most recent update for the other study (IMPE or IHME) for that uptake. The rationale for not including every new update by DELP [4], LANL [7], or SRIV [8] in the overarching principle is that it would lead to too frequent uptakes, which would defy the purpose of gaining new insight with each uptake of the covir2.

Algorithmic details of the rule for adding uptakes to the covir2 repository are as follows. For every single calendar date, (1) Check for new updates by IHME. (2) If a new update by IHME is available, start a new uptake with today's date, and use this new update by IHME. (3) Look for the latest available update by IMPE and include that in this uptake. (4) Look for the latest available update by LANL and include that in this uptake. (5) Look for updates by DELP and SRIV for which the date is equal to the date for IHME. (6) If no new update by IHME is available (from step 1), check for new updates by IMPE. If a new update by IMPE is available, start a new uptake with today's date, and use this new update by IMPE. (7) Look for the latest available update by IHME and include that in this uptake. (8) Look for the latest available update by LANL and include that in this uptake. (9) Look for updates by DELP and SRIV for which the date is equal to the date for IMPE. (10) If no new update by IMPE is available (from step 6), there is no new uptake for this calendar date. 



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


