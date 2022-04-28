# GOVERNMENTS' RESPONSES TO COVID-19 (response2covid19) - DATASET

Last update: 2021-06-30. 

Data visualisations are available here: https://response2covid19.org/

The dataset tracks governments’ responses to COVID-19 all around the world. The dataset is at the country-level and covers the January 2020 - June 2021 period. It tracks 20 measures – 13 public health measures and 7 economic measures – taken by more than 213 governments. The tracking of the measures allows creating an index of the rigidity of public health measures and an index of economic response to the pandemic. The objective of the dataset is both to inform citizens and to help researchers and governments in fighting the pandemic.

The dataset can be downloaded and used freely. Please properly cite the name of the dataset (“Response2covid19”) and the reference: Porcher, Simon "Response2covid19, a dataset of governments' responses to COVID-19 all around the world", Scientific Data, 7, 423, 2020. https://doi.org/10.1038/s41597-020-00757-y

## GENERAL INFORMATION

#### 1.	Title of Dataset: 

Response2covid19

#### 2.	Authors Information

The principal investigator is Simon Porcher. 	
Contact:
IAE Paris / Sorbonne Business School
8 bis rue Croix de Jarry 75013 Paris France
porcher.iae@univ-paris1.fr

Research assistants: Sarah Chauveau (v7), Lorena Demichelis (v1, v3, v5, v7), Oriane Maille-Lefranc (v6, v7), Léa Reville (v2, v3 and v4), Aziz Goumiri (v3 and v4). 

#### 3.	Date of data collection: 2020-03-16 to 2021-06-30.

#### 4.	Geographic location of data collection: Paris, France.  

#### 5.	Information about funding sources that supported the collection of the data: No funding. 

## SHARING/ACCESS INFORMATION

#### 1.	Licenses/restrictions placed on the data: 

The dataset can be used for free. Please properly acknowledge the author's name, name of the dataset and the paper presenting the data as Porcher, Simon "Response2covid19, a dataset of governments' responses to COVID-19 all around the world", Scientific Data, 7, 423, 2020. https://doi.org/10.1038/s41597-020-00757-y

#### 2.	Links to other publicly accessible locations of the data: https://www.openicpsr.org/openicpsr/project/119061/version/V7/view

#### 3.	The data is derived from the following sources: 

The coding of public health measures is based on cross-country information primarily reported by the Assessment Capacities Project (ACAPS), the International Institute for Democracy and Electoral Assistance (IDEA) for elections and the United Nations Educational Scientific and Cultural Organization (UNESCO) for schools closures. For economic measures, the information comes from the IMF and the International Growth Centre. In the latest version of the dataset, other sources of information are used and reported in the sources file.

Detailed country-level sources are  reported in the Gov_Responses_Sources.xlsx file in the Latest version folder.

#### 5.	Cite the dataset as Porcher, Simon "Response2covid19, a dataset of governments' responses to COVID-19 all around the world", Scientific Data, 7, 423, 2020. https://doi.org/10.1038/s41597-020-00757-y

## DATA & FILE OVERVIEW

#### 1.	File List: 
Gov_Responses_Covid19_last.dta, Stata file
Gov_Responses_Covid19_last.xls, Excel file
Gov_Responses_Sources.xls, Excel file
script.do, a Stata file to write the spreadsheet, Do file

#### 2.	Last update:

The updated file is the latest version. There will be no update.

## METHODOLOGICAL INFORMATION

#### 1.	Description of methods used for collection/generation of data: 

Data coding is detailed in Porcher, Simon "Response2covid19, a dataset of governments' responses to COVID-19 all around the world", Scientific Data, 7, 423, 2020. https://doi.org/10.1038/s41597-020-00757-y

#### 2.	Methods for processing the data: 

For all measures, dataset is coded by hand. UNESCO data on schools is merged with our dataset. More information can be found in Porcher, Simon "Response2covid19, a dataset of governments' responses to COVID-19 all around the world", Scientific Data, 7, 423, 2020. https://doi.org/10.1038/s41597-020-00757-y

#### 3.	Softwares used to collect the data: 

Data was first coded in Excel and then corrected in Stata 14 for PC. From June 2020, the dataset is based on a unique script (script.do) under Stata.

#### 4.	People involved with sample collection, processing, analysis and/or submission: 

Simon Porcher (principal investigator). Coding by Sarah Chauveau, Oriane Maille-Lefranc, and Simon Porcher. Verifications by: Sarah Chauveau, Oriane Maille-Lefranc, Lorena Demichelis, Baoqin Dong, Léa Réville, Aziz Goumiri, Pauline Colin.

## DATA-SPECIFIC INFORMATION FOR: Gov_Responses_Covid19_last.dta 

#### 1.	Number of variables: 

39.

#### 2.	Number of cases/rows: 

117,576 observations; 213 countries. 

#### 3.	Variables List: 

- country: name of the country or the territory;
-  geodi: two-letters country code;
- iso: three-letters country code;
- d: date of the observation;
- school: binary variable equal to1 if schools were closed and 0 otherwise;
- school_local: binary flag to distinguish localized school closures from other cases. 1 denotes that school closures were implemented at the local level and 0 denotes that school closures were not implemented at the local level (either at the national level or no school closures). The data on the scale of school closures is imported from the UNESCO. The interaction of school and school_local allows researchers to create three levels of measures: no school closures (school=0 and school_local=0), localized school closures (school=1 and school_local==1) or national school closures (school=1 and school_local=0);
- domestic: binary variable equal to 1 if there was a domestic lockdown and 0 otherwise;
- domestic_local: binary variable to distinguish localized domestic lockdowns from other cases. 1 denotes that domestic lockdowns were implemented at the local level and 0 means that domestic lockdowns were not implemented at the local-level (either at the national level or not implemented). The nature of the domestic lockdown is based on our reading of the measures reported by the ACAPS. The interaction of domestic and domestic_local allows researchers to create three levels of measures: no domestic lockdown (domestic=0 and domestic_local=0), localized domestic lockdowns (domestic=1 and domestic_local=1) or national domestic lockdowns (domestic=1 and domestic_local=0);
- travel: binary variable equal to1 if travel restrictions were implemented and 0 otherwise;
- travel_partial: binary flag to differentiate partial travel restrictions from other cases. 1 denotes that travel restrictions were partial and 0 denotes that travel restrictions were not partial (either strict or not implemented). The nature of the travel restrictions is based on our reading of the measures reported by the ACAPS. The interaction of travel and travel_partial allows researchers to create three levels of measures: no travel restrictions (travel=0 and travel_partial=0), partial travel restrictions (travel=1 and travel_partial=1) or strict travel restrictions (travel=1 and travel_partial=0);
-	travel_dom: binary variable equal to1 if travel restrictions within the country  (e.g. inter-region travels) were implemented and 0 otherwise;
-	travel_dom_partial: binary flag to differentiate partial domestic travel restrictions from other cases. 1 denotes that travel restrictions were partial and 0 denotes that travel restrictions were not partial (either strict or not implemented). The nature of the travel restrictions is based on our reading of the measures reported by the ACAPS. The interaction of travel and travel_partial allows researchers to create three levels of measures: no domestic travel restrictions (travel_dom=0 and travel_dom_partial=0), partial domestic travel restrictions (travel_dom=1 and travel_dom_partial=1) or strict domestic travel restrictions (travel_dom=1 and travel_dom_partial=0);
-	curf: binary variable equal to1 if a curfew was implemented and 0 otherwise;
-	curf_partial: binary flag to differentiate partial curfews from other cases. 1 denotes that the curfew was partial and 0 denotes that the curfew was not partial (either strict or not implemented). The nature of the curfew is based on our reading of the measures reported by the ACAPS. The interaction of curf and curf_partial allows researchers to create three levels of measures: no curfew (curf=0 and curf_partial=0), partial curfew (curf=1 and curf_partial=1) or strict curfew (curf=1 and curf_partial=0);
- mass: binary variable equal to1 if bans on mass gatherings were implemented and 0 otherwise;
- mass_partial: binary flag to distinguish localized bans on mass gatherings from other cases. 1 denotes that bans on mass gatherings were partial and 0 denotes that bans on mass gatherings were not partial (either strict or not implemented). The nature of the bans on mass gatherings is based on our reading of the measures reported by the ACAPS. The interaction of mass and mass_partial allows researchers to create three levels of measures: no bans on mass gatherings (mass=0 and mass_partial=0), localized or partial bans (mass=1 and mass_partial=1) or national or strict bans (mass=1 and mass_partial=0);
- elect: binary variable equal to1 if some elections were postponed and 0 otherwise;
- elect_partial: binary flag to differentiate countries which postponed only some of the elections from the others. 1 denotes that countries both maintained and postponed elections and 0 denotes that elections were either postponed, maintained or were not scheduled. IDEA lists all maintained and postponed elections since the beginning of 2020. The interaction of elect and elect_partial allows researchers to differentiate three settings: all elections were maintained despite COVID-19 (elect=0 and elect_partial=0), some elections were maintained and others were postponed (elect=1 and elect_partial=1) or all elections were postponed (elect=1 and elect_partial=0);
- sport: binary variable equal to1 if bans on sporting and large events were implemented and 0 otherwise;
- sport_partial: binary flag to distinguish partial bans and cancellations of sporting and large events. 1 denotes that bans on sporting and large events were localized, strict or with no spectators, 0 that bans on sporting and large events are not localized or partial (either national or no measures implemented). The nature of the bans on sporting and large events is based on our reading of the measures reported by the ACAPS. The interaction of sport and sport_partial allows researchers to create three levels of measures: no bans (sport=0 and sport_partial=0), partial bans (sport=1 and sport_partial=1) or national bans on mass gatherings (sport=1 and sport_partial=0);
- rest: binary variable equal to1 if restaurants were closed and 0 otherwise;
- rest_local: binary flag to distinguish localized and/or partial restaurant and bar closures from other cases. The variable is coded 1 in the three following situations: localized closures, limitations on the number of customers in bars and restaurants, and closures of either bars or restaurants. 0 indicates national closures or no closures at all. The coding is based on our reading of the measures reported by the ACAPS. The interaction of rest and rest_local allows researchers to create three levels of measures: no closures (rest=0 and rest_local=0), localized closures (rest=1 and rest_local=1) or national closures (rest=1 and rest_local=0);
- testing: binary variable equal to1 if there was a public testing policy and 0 otherwise;
- testing_narrow:  binary flag to distinguish narrow testing policies from large testing policies. 1 denotes that testing policies were targeted to some individuals, 0 that testing policies were not targeted (either large or not implemented). The nature of the testing policy is based on the information reported in the measures “mass population testing” and “testing policy” in the ACAPS. When the measure was targeted, testing_narrow was coded 1. On the contrary, when the measure was not targeted, testing_narrow was coded 0. The interaction of testing and testing_narrow allows researchers to create three levels of measures: no testing policy (testing=0 and testing_narrow =0), narrow testing policy (testing=1 and testing_narrow =1) or large testing policy (testing=1 and testing_narrow =0);
- surveillance: binary variable equal to1 if mobile app or bracelet surveillance was implemented and 0 otherwise;
- surveillance_partial: binary variable equal to1 if the enhanced surveillance is optional or reserved for a category of person (e.g. certain professions or foreigners) and 0 otherwise, based on information in the ACAPS.  When the measure was partial, surveillance_partial was coded 1. On the contrary, when the measure was strict (anybody suspected of having COVID-19), surveillance_partial was coded 0. The interaction of surveillance and surveillance_partial allows researchers to create three levels of measures: no surveillance (surveillance=0 and surveillance_partial =0), partial surveillance (surveillance=1 and surveillance_partial=1) or strict surveillance (surveillance=1 and surveillance_partial =0);
- masks : binary variable equal to1 if mandates to wear masks in public spaces were implemented and 0 otherwise;
- masks_partial: binary variable equal to1 if the obligation to wear masks is regional, based on information in the ACAPS.  When the measure was regional, masks_partial was coded 1. On the contrary, when the measure was national, masks_partial was coded 0. The interaction of masks and masks_partial allows researchers to create three levels of measures: no obligations to wear masks (masks=0 and masks_partial =0), regional obligations to wear masks (masks=1 and masks_partial=1) or national obligations to wear masks (masks=1 and masks_partial =0);
- state: binary variable equal to1 if the state of emergency is declared and 0 otherwise;
- state_partial: binary variable equal to1 if the state of emergency is declared on a local basis and 0 otherwise, based on information in the ACAPS.  When the measure was local, state_partial was coded 1. On the contrary, when the measure was not localized, state_partial was coded 0. The interaction of state and state_partial allows researchers to create three levels of measures: no state of emergency (state=0 and state_partial =0), partial state of emergency (state=1 and state_partial=1) or national state of emergency (state=1 and state_partial =0);
- cash: binary variable equal to1 if cash transfers are implemented and 0 otherwise;
- wage: binary variable equal to1 if wage support is implemented and 0 otherwise;
- credit: binary variable equal to1 if credit schemes are implemented and 0 otherwise;
- taxc: binary variable equal to1 if tax credits are implemented and 0 otherwise;
- taxd: binary variable equal to1 if tax delays are implemented and 0 otherwise;
- export: binary variable equal to1 if supports to importers or exporters are implemented and 0 otherwise;
- rate: binary variable equal to1 if the Central Bank lowered the interest rates and 0 otherwise;
- Rigidity_Public_Health: average of the ten coded public health measures. Public health measures are valued 0.5 if they are localized or partial and 1 if they are national or strict. 0 indicates no measures;
- Economic_Measures: average of the coded economic measures. 

#### 4.	Missing data codes: 

Missing variables, e.g. when the country was not covered by our sources, are flagshiped with a gap ("." in Stata, empty cell in Excel).

#### 5.	Miscellaneous: 

The dataset is mainly based on manual recording of policy measures implemented all around the world. Even though we made the best attempt to report data as accurately as possible, there might be some remaining errors and we apologize in advance for that. Please email the corresponding author if you wish to point some errors or leave a message on the GitHub repository. 

