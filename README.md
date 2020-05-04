Governments’ responses to COVID-19 - Dataset

This PORCHER_GOVCOVID19_Readme.txt file was first generated on 2020-04-20 by Simon PORCHER. A modified version is generated on 2020-05-04. 

The dataset tracks governments’ responses to COVID-19 all around the world. The dataset is at the country-level and covers the January-April 2020 period. It tracks 17 measures – 10 public health measures and 7 economic measures – taken by 228 governments. The tracking of the measures allows creating an index of the rigidity of public health measures and an index of economic response to the pandemic. The objective of the dataset is both to inform citizens and to help researchers and governments in fighting the pandemic. 
The dataset can be downloaded and used freely. Please properly cite the name of the dataset (“Governments’ Responses to COVID-19”) and the reference: Porcher, Simon "A novel dataset on governments' responses to COVID-19 all around the world", Chaire EPPP 2020-03 discussion paper, 2020. 

GENERAL INFORMATION

1.	Title of Dataset: Governments' Responses to COVID-19

2.	Author Information

The principal investigator is Simon Porcher. 	
Contact:
IAE Paris / Sorbonne Business School
8 bis rue Croix de Jarry 75013 Paris France
porcher.iae@univ-paris1.fr

Research assistants: Lorena Demichelis (v1), Léa Reville (v2). 

3.	 Date of data collection: 2020-03-16 to 2020-04-29.

4.	Geographic location of data collection: Paris, France.  

5.	Information about funding sources that supported the collection of the data: No funding. 

SHARING/ACCESS INFORMATION

1.	Licenses/restrictions placed on the data: please cite the data as Porcher, Simon "A novel dataset on governments' responses to COVID-19 all around the world", Chaire EPPP discussion paper 2020-03. Link: https://www.chaire-eppp.org/documents-de-travail-publications/

2.	Links to publications that cite or use the data: 
https://www.chaire-eppp.org/contagion-the-determinants-of-governments-public-health-responses-to-covid-19-all-around-the-world/

3.	Links to other publicly accessible locations of the data: https://www.openicpsr.org/openicpsr/project/119061/version/V2/view

4.	The data is derived from the following sources: 
The coding of public health measures is based on cross-country information reported by the Assessment Capacities Project (ACAPS; https://www.acaps.org/covid19-government-measures-dataset), the International Institute for Democracy and Electoral Assistance (IDEA; https://www.idea.int/publications/catalogue/elections-and-covid-19) for elections and the United Nations Educational Scientific and Cultural Organization (UNESCO; https://en.unesco.org/covid19/educationresponse) for schools closures. For economic measures, the information comes from the IMF (https://www.imf.org/en/Topics/imf-and-covid19/Policy-Responses-to-COVID-19) and the International Growth Centre (https://www.theigc.org/covid-19/).

Detailed country-level sources are  reported here: Gov_Responses_Sources.xls.

5.	Cite the dataset as Porcher, Simon "A novel dataset on governments' responses to COVID-19 all around the world", Chaire EPPP 2020-03 discussion paper, 2020.

DATA & FILE OVERVIEW

1.	File List: 
Gov_Responses_Covid19_02May.dta, Stata file
Gov_Responses_Covid19_02May.xls, Excel file
Gov_Responses_Sources.xls, Excel file

2.	The updated file is the version of May 04, 2020. Updated version will be uploaded on a bi-monthly basis.

METHODOLOGICAL INFORMATION

1.	Description of methods used for collection/generation of data: 
Data coding is detailed in Porcher, Simon "A novel dataset on governments’ responses to COVID-19 all around the world", Chaire EPPP discussion paper 2020-03, 2020. 

2.	Methods for processing the data: 
For all measures, dataset is coded by hand. UNESCO data is merged with our dataset. More information can be found in Porcher, Simon "A novel dataset on governments’ responses to COVID-19 all around the world", Chaire EPPP discussion paper 2020-03, 2020. 

3.	Instrument- or software-specific information needed to interpret the data: 
Data is coded in Excel and modified in Stata 14 for PC. 

4.	People involved with sample collection, processing, analysis and/or submission: 
Simon Porcher (principal investigator). Verifications by: Lorena Demichelis, Léa Réville. 

DATA-SPECIFIC INFORMATION FOR: Gov_Responses_Covid19_02May.dta

1.	Number of variables: 34

2.	Number of cases/rows: 14,601 observations; 228 countries. 

3.	Variables List: 

- country: name of the country or the territory;
- iso: three-letters country code;
- d: date of the observation;
- cases: number of cases reported on the given day by the European Centre for Disease Prevention and Control;
- deaths: number of deaths reported on the given day by the European Centre for Disease Prevention and Control;
- school: binary variable equal to1 if schools are closed and 0 either;
- school_local: binary flag to distinguish localized schools closures from other cases. 1 denotes that schools closures were implemented at the local level and 0 that schools closures were not implemented at the local level (either at the national level or no schools closures). The data on the nature of schools closures is imported from the UNESCO. The interaction of school and school_local allows researchers to create three levels of measures: no schools closures (school=0 and school_local=0), localized school closures (school=1 and school_local==1) or national schools closures (school=1 and school_local=0);
- domestic: binary variable equal to 1 if there is a domestic lockdown and 0 either;
- domestic_local: binary variable to distinguish localized domestic lockdowns from other cases. 1 denotes that domestic lockdowns were implemented at the local level and 0 that domestic lockdowns were not implemented at the local-level (either at the national level or not implemented). The nature of the domestic lockdown is based on our reading of the measures reported by the ACAPS. The interaction of domestic and domestic_local allows researchers to create three levels of measures: no domestic lockdown (domestic=0 and domestic_local=0), localized domestic lockdowns (domestic=1 and domestic_local==1) or national domestic lockdowns (domestic=1 and domestic_local=0);
- travel: binary variable equal to1 if travel restrictions are closed and 0 either;
- travel_partial: binary flag to differentiate partial travel restrictions from other cases. 1 denotes that travel restrictions were partial and 0 that travel restrictions were not partial (either strict or not implemented). The nature of the travel restrictions is based on our reading of the measures reported by the ACAPS. The interaction of travel and travel_partial allows researchers to create three levels of measures: no travel restrictions (travel=0 and travel_partial=0), partial travel restrictions (travel=1 and travel_partial=1) or strict travel restrictions (travel=1 and travel_partial=0);
- mass: binary variable equal to1 if bans on mass gatherings are implemented and 0 either;
- mass_partial: binary flag to distinguish localized bans on mass gatherings from other cases. 1 denotes that bans on mass gatherings were localized and 0 that bans on mass gatherings are not localized (either national or no bans implemented). The nature of the bans on mass gatherings is based on our reading of the measures reported by the ACAPS. The interaction of mass and mass_partial allows researchers to create three levels of measures: no bans on mass gatherings (mass=0 and mass_partial=0), localized bans (mass=1 and mass_partial=1) or national bans (mass=1 and mass_partial=0);
- elect: binary variable equal to1 if some elections are postponed and 0 either;
- elect_partial: binary flag to differentiate countries which postponed only some of the elections from the others. 1 denotes that countries both maintained and postponed elections and 0 that elections were either postponed, maintained or were not scheduled. IDEA lists all maintained and postponed elections since the beginning of 2020. The interaction of elect and elect_partial allows researchers to differentiate three settings: all elections were maintained despite COVID-19 (elect=0 and elect_partial=0), some elections were maintained and others were postponed (elect=1 and elect_partial=1) or all elections were postponed (elect=1 and elect_partial=0);
- sport: binary variable equal to1 if bans on sporting and large events are implemented and 0 either;
- sport_partial: binary flag to distinguish partial bans and cancellations of sporting and large events. 1 denotes that bans on sporting and large events were localized or behind closed doors, 0 that bans on sporting and large events are not localized (either national or no measures implemented). The nature of the bans on sporting and large events is based on our reading of the measures reported by the ACAPS. The interaction of sport and sport_partial allows researchers to create three levels of measures: no bans (sport=0 and sport_partial=0), partial bans (sport=1 and sport_partial=1) or national bans on mass gatherings (sport=1 and sport_partial=0);
- rest: binary variable equal to1 if restaurants are closed and 0 either;
- rest_local: binary flag to distinguish localized and/or partial restaurants and bars closures from other cases. The variable is coded 1 in the three following situations: localized closures, limitations on the number of customers in bars and restaurants, and closures of bars without mentioning restaurants. 0 indicates national closures or no closures at all. The coding is based on our reading of the measures reported by the ACAPS. The interaction of rest and rest_local allows researchers to create three levels of measures: no closures (rest=0 and rest_local=0), localized closures (rest=1 and rest_local=1) or national closures (rest=1 and rest_local=0);
- testing: binary variable equal to1 if there is a public testing policy and 0 either;
- testing_narrow:  binary flag to distinguish narrow testing policies from large testing policies. 1 denotes that testing policies were targeted to some individuals, 0 that testing policies were not targeted (either large or not implemented). The nature of the testing policy is based on the information reported in the measures “mass population testing” and “testing policy” in the ACAPS. When the measure was targeted, testing_narrow was coded 1. On the contrary, when the measure was not targeted, testing_narrow was coded 0. The interaction of testing and testing_narrow allows researchers to create three levels of measures: no testing policy  (testing=0 and testing_narrow =0), narrow testing policy (testing=1 and testing_narrow =1) or large testing policy (testing=1 and testing_narrow =0);
- surveillance: binary variable equal to1 if mobile app or bracelet surveillance is implemented and 0 either;
- state: binary variable equal to1 if the state of emergency is declared, 0 either;
- cash: binary variable equal to1 if cash transfers are implemented, 0 either;
- wage: binary variable equal to1 if wage support is implemented, 0 either;
- credit: binary variable equal to1 if credit schemes are implemented, 0 either;
- taxc: binary variable equal to1 if tax credits and  tax cuts are implemented;
- taxd: binary variable equal to1 if tax credits and  tax delays are implemented;
- export: binary variable equal to1 if supports to importers or exporters are implemented, 0 either;
- rate: binary variable equal to1 if the Central Bank lowered the interest rates, 0 either;
- Rigidity_Public_Health: average of the ten coded public health measures. Public health measures are valued 0.5 if they are localized or partial, 1 if they are national or strict;
- Economic_Measures: average of the coded economic measures. 

4.	Missing data codes: "."

5.	Miscellaneous: 

The dataset is based on manual recording of policy measures implemented all around the world. Even though we made the best attempt to report data as accurately as possible, there might be some remaining errors and we apologize in advance for that. Please email the corresponding author if you wish to point some errors or leave a message on the GitHub repository. 

