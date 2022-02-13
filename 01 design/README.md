# Hepatitis A outbreak in the United States

## Students:

Marie-Laure Charpignon

Maria Mironova

Austin Walsh

Lorraine Wong

Saeyoung Rho

## Faculty:

Dr. Maia Majumder



## I. Abstract

Infection with hepatitis A virus is one the most common causes of acute hepatitis A worldwide. After a significant decline in the number of cases in the United States from 2001 to 2016, starting from the beginning of 2017 we have observed an outbreak of hepatitis A. The disease is predominantly spread among homeless and illicit drug users in multiple states and the rapid spread of the infection presents a public health challenge. In our study we use the combination of traditional CDC/state reports and non-traditional data sources to predict the future outbreak dynamics for better disease prevention strategy.

## II. Background

Infection with hepatitis A virus is one of the most common causes of acute hepatitis worldwide. It is a highly contagious disease that can lead to serious morbidity and occasional mortality. Hepatitis A virus (HAV) is transmitted via fecal-oral route usually via contaminated food or water or through close physical contact with the infected person. HAV infection causes acute hepatitis with nausea, abdominal pain, anorexia, vomiting, fatigue, fever and jaundice as predominant symptoms [1]. The incidence of the disease in the United States has steadily declined since the introduction of the vaccine in 1996. The Centers for Disease Control and Prevention (CDC) recommends routine vaccination of all children at the age of one year old and adults from high-risk groups – people traveling to endemic areas, men who have sex with men, patients with chronic liver disease, injection-drug users. While routine childhood hepatitis A vaccination has provided higher immunity protection in younger populations, many susceptible adults remain unvaccinated [2].

Between 2001 and 2015 the annual incidence of HAV infection continued to decrease, falling by 86.9% - from 10,615 cases in 2001 to 1,390 in 2015. In 2016, several foodborne-related outbreaks were reported which led to an increased number of HAV cases – 2,007 [3]. The new hepatitis A outbreak started in 2017. From January 2017 to April 2018, the CDC received more than 2,500 reports of hepatitis A infections associated with person-to-person transmission from multiple states. Of those reports for which risk factors are known, 68% of the infected persons report drug use (injection and non-injection), homelessness, or both [4]. The high incidence of HAV infection was also reported among men who have sex with men (MSM) in New York during the first six months of 2017 [5]. The number of hospitalizations and deaths during the current outbreak has been higher than what is normally reported through national surveillance of hepatitis A. While in 2016 the number of hospitalizations due to HAV infection was 42% and number of deaths was 0.7%, during the outbreak these numbers reached 71% and 3%, respectively [3,6]. The severity of the infection may be attributable to pre-existing chronic illnesses, including hepatitis B and C infections, other comorbidities, age and risk behaviors common among drug users and homeless [6,7].

The outbreak, which started in 2017, hit new highs in the end of 2018 through the beginning of 2019. In March 2019, the local Departments of Health from 17 states reported more than 15,000 outbreak-related cases. It shows an almost 500% increase in the number of cases since April 2018, and Kentucky is an infamous leader where 4,229 cases of infection and 43 deaths were confirmed [8]. The routine surveillance data for the ongoing hepatitis A outbreak from CDC is not yet available, but it is obvious that the rapid spread of HAV infection among under-privileged population can bring us back into the pre-vaccine era.

The near-real time estimate of the incidence is crucial for the prediction of outbreak dynamics and disease prevention strategy. The aim of our study is to predict the dynamics of the current hepatitis A outbreak among underprivileged individuals, using the combination of the traditional CDC reports and non-traditional data sources such as news media and Google search trends. Usage of non-traditional data sources such as news media and Google trends is an emerging trend in global healthcare. It has already shown utility in augmenting traditional approaches in tracking infectious diseases outbreaks when the surveillance data is missing [9-11].

## III. Specific Aims

### A. Modeling the 2017-2019 hepatitis A outbreak and assessing the time evolution of vaccination rates at the state-level

The first part of our project will consist in modeling the epidemic curve for the recent outbreak of hepatitis A in the US. We are aiming at developing a flexible framework, but will certainly focus on two states: one in which the outbreak has already ended (e.g. California) and another where it is still ongoing (e.g. Kentucky). 

Indeed, we would like (1) to develop a model of the epidemic dynamics from start to end, and (2) to predict the next stages of the outbreak using currently available information for the states that are still affected. Ideally, we should be able to build two types of models, both at the state and county-level.

#### For this, we need to collect and merge various types of data: 

##### Cases and Deaths

* Variables: 
Number of confirmed cases of hepatitis A
Number of deaths due to hepatitis A

* Time Granularity: 
Daily/weekly, from January 2017 to mid-March 2019

 * Geographical Levels: 
 State, county, city, zip code

##### Vaccination Data

* Variables: 
Number of hepatitis A vaccine doses ordered
Number of hepatitis A vaccine doses administered

* Time Granularity: 
Daily/weekly, from January 2017 to mid-March 2019

* Geographical Levels: 
State, county, city, zip code

Note: Ideally, we would be able to identify the location of health clinic/centers along with their vaccination start dates, as well dates and locations of street van campaigns.

##### Population Data
In addition to the time series of cases, deaths and vaccinations, we need to estimate the size of the population at-risk in each locality. This involves getting statistics on homelessness, illicit drug use and health insurance at different geographical levels. We have already identified a reliable data source for each of these, using respectively data from the United States Interagency Council on Homelessness (2017 & 2018, state-level), the National Survey on Drug Abuse and Health or NSDUH (2017, state-level) and the Kaiser Family Foundation (2017, state-level).

### B. Using non-traditional data sources to complement hepatitis A disease surveillance data.

Non-traditional data sources will be used for the sentiment analysis of the outbreak. We will search those data sources to identify statistically significant predictors of the acceptance of vaccination by the most vulnerable populations. We plan to use two main data sources: Google search trends and article headlines extracted from HealthMap.

Google Trends will be helpful to assess the reaction of the population to the ongoing outbreak and interest in the preventive measures and vaccination. To query Google Trends, we will use combination of key terms that can represent multiple questions conveying people’s concerns. This can also be used to evaluate presence of distrust to healthcare among underprivileged population.


#### Examples of general question

* [Hep A, risk]:
*“Am I at risk for hepatitis A?”*

* [Hep A, contagious]:
*“Is hepatitis A contagious?”*

#### Examples of positive reactions to vaccination: 

* [Where, Hep A, Vaccine]:
*“Where can I get the hepatitis A vaccine?”*

* [Price, Hep A, Vaccine]:
*“How much does hepatitis A vaccine cost?”*

#### Examples of negative reactions to vaccination and / or stigmatization:

* [!@#!$ (bad) drug, Hep A]:
*“Are drug users/junkies at a high risk of hepatitis A?”*,
*“If I have hepatitis A, do people think I am a junkie?”*,
*“Can I get hepatitis A after smoking a pot?”*

* [Hep A, homeless, contagious]:
*“Can I get infected with hepatitis A by sitting near a homeless?”*

* [Hep A, jail, contagious]:
*“Can I get infected with hepatitis A by sitting near a person jailed?”*

* [Hep A, Vaccine, Autism]:
*“Does hepatitis vaccine cause autism?”*

* [Hep A, Vaccine, Side effects]:
*“What are the side effects of hepatitis A vaccine?”*

To understand the outbreak coverage in the news we will analyze the articles and their headlines extracted from HealthMap. The relationship/association between state health outcomes and outbreak coverage in news will be done by creating rank lists (first rank – outbreak severity in each state by number of cases per 100,000 and cause-specific mortality rate, second rank – outbreak coverage in news in each state by number of articles and reports in a period of time).

In summary, we expect that the analysis of both types of data sources, traditional and non-traditional, will provide us with a model which will enable robust predictions of hepatitis A outcomes and a larger acceptance of vaccination among vulnerable populations.

## IV. Deliverables

### A. Interim Deliverable

#### 1. Intermediary report

* Status of data collection process

* Summary of findings so far

### B. Final Deliverable

#### 1. Final report of findings

#### 2. Final presentation

## V. Team & Roles

### Team

* Marie-Laure Charpignon, PhD student in Statistics, MIT (1,2,3,4,5)

* Maria Mironova, MD, MIT (1,2,3,4,5)

* Austin Walsh, Master’s student in Health Informatics, USF (1,3,4,5)

* Lorraine Wong, BSN, RN, Master’s student in Health Informatics, USF (1,3,4,5)

* Saeyoung Rho, Master’s student in Technology & Policy Program + EECS, MIT (3,5)

### Roles

#### We have identified several responsibilities members of the team can take on throughout the project: 

(1) data acquisition, (2) data analysis and interpretation, (3) contribution to conception and design, (4) Google slides presentation and (5) drafting the report.


#### This may evolve during the semester, but based on our first three group meetings:

* *Marie-Laure, Maria, Austin and Lorraine* would be in charge of data acquisition (e.g. reaching out to state and local health departments.)

* *Marie-Laure and Maria* would be responsible for processing that data as well as analyzing the results from the HealthMap query.

* *Everyone* would be involved in the conception and design of the study, especially regarding the methodology to assess news coverage and compare it to health outcomes at the local level.

* *Marie-Laure, Maria, Austin and Lorraine* would be producing the presentation. 

* *Everyone* would be involved in the compilation of the final report, as well as in the draft paper.

## VI. Strategy

### A. Specific Steps Taken Over the Semester

* Collect hepatitis A data from CDC and state departments of health (cases, deaths, vaccinations)

* Perform data collection of various news media (articles, videos, tweets) related to hepatitis A

* Query Google Trends for hepatitis A related searches

### B. Timeline

#### By March 29, 2019: 
* Gather data on hepatitis A in the US (infection incidence, death rates and vaccination rates / locations)

* CDC information

* State/County-level information

* Various news media (reports, articles, videos, tweets)

#### By April 6, 2019: 

Focus on Google trends data collection

#### By April 12, 2019: 

Submit interim deliverable

#### By May 2, 2019: 

Finalize slides for presentation

#### May 3, 2019: 

Project Presentation

#### By May 13, 2019: 

Submit final report/findings







## VII. References

1. Koenig KL, Shastry S, Burns MJ. Hepatitis A virus: Essential knowledge and a novel Identify-Isolate-Inform tool for frontline healthcare providers. West J Emerg Med. 2017 Oct;18(6):1000-1007.
2. Campos-Outcalt D. CDC provides advice on recent hepatitis A outbreaks J Fam Pract. 2018 January;67(1):30-32.
3. CDC. Viral hepatitis surveillance, United States 2016. Atlanta, GA: US Department of Health and Human Services, CDC; 2017.
4. Health Alert Network (HAN) No.412. Outbreak of Hepatitis A Virus (HAV) Infections among Persons Who Use Drugs and Persons Experiencing Homelessness.https://emergency.cdc.gov/han/han00412.asp 
5. Latash J, Dorsinville M, Del Rosso P, et al. Notes from the Field: Increase in Reported Hepatitis A Infections Among Men Who Have Sex with Men — New York City, January–August 2017. MMWR Morb Mortal Wkly Rep 2017;66:999–1000.
6. Foster M, Ramachandran S, Myatt K, et al. Hepatitis A Virus Outbreaks Associated with Drug Use and Homelessness — California, Kentucky, Michigan, and Utah, 2017. MMWR Morb Mortal Wkly Rep 2018;67:1208–1210.
7. Kreshak AA, Brennan JJ, Vilke GM et al. A description of a health system's emergency department patients who were part of a large hepatitis A outbreak. J Emerg Med. 2018, Nov; 5(55):620-626.
8. Outbreaks of hepatitis A in multiple states among people who use drugs and/or people experiencing homelessness. https://www.cdc.gov/hepatitis/outbreaks/2017March-HepatitisA.htm 
9. Chan EH, Sahai V, Conrad C, Brownstein JS. Using web search query data to monitor dengue epidemics: a new model for neglected tropical disease surveillance. PLoS Negl Trop Dis. 2011;5(5):e1206.
10. Ghosh, S. et al. Temporal topic modeling to assess associations between news trends and infectious disease outbreaks. Sci. Rep. 7, 40841.
11. Majumder MS, Santillana M, Mekaru SR, McGinnis DP, Khan K, Brownstein JS. Utilizing nontraditional data sources for near real-time estimation of transmission dynamics during the 2015-2016 Colombian Zika virus disease outbreak. JMIR Public Health Surveill. 2016;2(1):e30


