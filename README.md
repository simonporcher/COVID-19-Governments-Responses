# COVID-19-Governments-Responses
Dataset and papers on Governments' Responses to the COVID-19 

This PORCHER_GOVCOVID19_Readme.txt file was generated on 2020-04-20 by Simon PORCHER


GENERAL INFORMATION

1. Title of Dataset: Governments' Responses to COVID-19

2. Author Information
	A. Principal Investigator Contact Information
		Name: Porcher Simon	
		Institution: IAE Paris / Sorbonne Business School
		Address: 8 bis rue Croix de Jarry 75013 Paris France
		Email: porcher.iae@univ-paris1.fr

3. Date of data collection : 2020-03-16 to 2020-04-15 

4. Geographic location of data collection : Paris, France.  

5. Information about funding sources that supported the collection of the data: No funding. 


SHARING/ACCESS INFORMATION

1. Licenses/restrictions placed on the data: please cite the data as Porcher, Simon "A novel dataset on governments' responses to COVID-19 all around the world", chaire eppp discussion paper 2020-02.

2. Links to publications that cite or use the data: 

3. Links to other publicly accessible locations of the data: https://www.openicpsr.org/openicpsr/project/119061/version/V2/view

4. Was data derived from another source? yes
	A. If yes, list source(s): the IMF https://www.imf.org/en/Topics/imf-and-covid19/Policy-Responses-to-COVID-19; the IGC https://www.theigc.org/covid-19/; the UNESCO https://en.unesco.org/covid19/educationresponse; the ACAPS https://www.acaps.org/who-we-are/in-short

5. Recommended citation for this dataset: Porcher, Simon "A novel dataset on governments' responses to COVID-19 all around the world", working paper, 2020. 


DATA & FILE OVERVIEW

1. File List: 
Gov_Responses_Covid19.dta, stata file
Porcher, Simon "A novel dataset on governments' responses to COVID-19 all around the world", explaining the coding of the dataset.

2. The updated file is the version of April, 15th, 2020. Updated version will be uploaded on a monthly basis.


METHODOLOGICAL INFORMATION

1. Description of methods used for collection/generation of data: 
Data coding is precised in Porcher, Simon "A novel dataset on governments’ responses to COVID-19 all around the world", working paper.

2. Methods for processing the data: 
Data was coded by hand

3. Instrument- or software-specific information needed to interpret the data: 
Data is coded in Stata 14 for PC

4. People involved with sample collection, processing, analysis and/or submission: Simon Porcher


DATA-SPECIFIC INFORMATION FOR: Gov_Responses_Covid19.dta


1. Number of variables: 24

2. Number of cases/rows: 11,034

3. Variables List: 

Variables	Source	Coding scheme
Public health measures
Bans on mass gatherings	ACAPS / IMF	1 if the ban is national, 0.5 if the ban is localized and 0 if there is no ban. 
Schools closure	UNESCO	1 if the closure is national, 0.5 if the ban is localized and 0 if there is no ban.
Travel restrictions	ACAPS / IMF	1 if the restriction is global (border closed / commercial flights cancelled), 0.5 if the restriction is targeted to some countries and 0 if there are no restrictions.
Domestic lockdown	ACAPS / IMF	1 if the lockdown is national, 0.5 if the lockdown is localized and 0 if there is no lockdown.
Cancellation of sporting and large events	ACAPS / IMF	1 if the cancellation is national, 0.5 if the cancellation is localized and 0 if there is no cancellation.
Restaurants closing	ACAPS	1 if the closing is global and national, 0.5 if the closing is localized or limited (e.g. number of customers is limited) and 0 if there is no closing.
Elections postponing	IDEA	1 if elections are postponed, 0.5 if some elections are postponed and 0 if elections were programmed but not postponed. N/A if no elections were to take place. 
State of Emergency	ACAPS / IMF	1 if State emergency (or health emergency) is implemented, 0 if not. 
Public testing	ACAPS	1 if public testing is (or aims at being) general, 0.5 if testing is done only at the hospital or people potentially contaminated, 0 if no testing is done. N/A if no information.
Enhanced surveillance	ACAPS	1 if monitoring app surveillance is active, 0 if not. 
Economic measures
Wage support	IMF / IGC	1 if wage support is implemented, 0 if not.
Cash transfer	IMF / IGC	1 if cash transfers are implemented, 0 if not.
Credit schemes	IMF / IGC	1 if credit schemes are implemented, 0 if not.
Tax cuts and delays	IMF / IGC	1 if tax cuts or tax delays are implemented, 0 if not.
Support to importers / exporters	IMF / IGC	1 if support to importers and exporters is implemented, 0 if not.
Interest rate cuts	IMF / IGC	1 if interest rate cuts are implemented, 0 if not. 


4. Missing data codes: "."

