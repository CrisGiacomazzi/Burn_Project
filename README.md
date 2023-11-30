# Burn_Project

**Burn patient in South Brazil: a Descriptive Analysis with open database of 10 years (2013-2023)**

Cristiane Mecca Giacomazzi (Data Analyst)

This project was developed with Cross-industry standard process for data mining (CRISP-DM) methodology.

The following topics will be presented:
1. Business Understanding
2. Data Understanding
3. Data Preparation
4. Dictionary
5. Analysis
6. Interpretation and Conclusions
7. Communication and Action
8. SWOT Analysis

**1) Business Understanding**

A burn is a skin or tissue injury caused by different sources.
Burn injuries not only impact the quality of life of those affected, however also leave sequelae, including scars and contractures that often result in a persistent distortion of body image. Furthermore, the treatment of burns involves a significant allocation of financial resources, particularly in the context of the Unified Health System in Brazil (SUS). Annually, the SUS spends approximately 55 million reais on treating burn victims. A brazilian study from França et al (2023) estimated an average cost of USD 214.666,45 (R$ 43.809,48) each patient.

Understanding the epidemiological characteristics of burns is imperative for promoting education, evaluating care for this population and providing the basis for public strategies for prevention, intervention and cost reduction.
* Objective: The purpose of this study is to describe the epidemiological and mortality profile of patients affected by burns in the state of Rio Grande do Sul between the years 2013 and 2023.

This study, centered on secondary data in the public domain, did not require submission to the Research Ethics Committee, presenting no risk to the confidentiality and anonymity of the individuals involved in the work; however, all ethical guidelines were strictly adhered to, as stipulated in Decree No. 7,724/2012 and Resolutions No. 510/2016 and Resolution 466/2012, issued by the Brazil National Health Council.

In order to facilitate the analysis, the groups available received the following names, according to International Classification of Diseases,Tenth Revision (ICD-10), the actual in Brazil, yet:
* Group 1 - W85-W99 (Exposure to electrical current, radiation or extreme environmental temperatures and pressures)
* Group 2 - X00-X09 (Exposure to smoke, fire and flames)
* Group 3 - X10-X19 (Contact with heat source and hot substances)

**2) Data Understanding**

* **Data Source**: The databases were chosen within the Hospital Morbidity section of the SUS of the Hospital Information System (SIH/SUS) in [DATASUS](https://https://datasus.saude.gov.br/informacoes-de-saude-tabnet/), using External causes, by place of hospitalization from 2008 onwards. Data are available from 2008 however, we selected January 2013 until August 2023 (maximum available).

* **Initial data exploration**: the original dataframes are in csv format and showed an error when reading directly in Google Colab, due to the existence of graphic signs, which is why I opted for structuring and cleaning on Google sheets, focusing on data analysis here.

**3) Data Preparation**

* Missing data were not removed. They means the absence of a case.
* There were no duplicate data.
* All accents and graphic signs were removed on Google sheets.
* No important outliers were identified that needed to be removed.
* "Totals" columns in the raw dataframe were excluded in cases that could interfere with the analysis and creation of graphs.
* In some cases it was necessary to join columns from different dataframes to generate a graph.

**4) Dictionary** 
(main file)

**5) Analysis**
(main file)

**6) Interpretation and Conclusion**

In the last decade in South Brazil (RGS), a predominance of males and white people in hospitalizations due to burns was observed, with a progressive increase also between females throughout the period analyzed.

Exposure to smoke, fire and flames (group 2) was the most importante cause of hospitalization for burns in RGS between 2013 and 2023. Then, contact with heat sources and hot substances (group 3) and finally exposure to electrical current, radiation, or extreme environmental temperatures and pressures (group 1). It is noteworthy that the number of hospitalizations has fluctuated since 2013, less variation in group 1.

It is essential to highlight that the etiology of burns in group 2 was the most prevalent in relation to hospitalizations, while group 1 had the highest number od deaths. Also, in relation to deaths, there was a more significant increase in 2018 and 2020 in group 1 with the maximum value in 2022, while in groups 2 and 3, the incidence remained stable.

The regions with the longest length of stay are nearby, probably due to the accredited and reference hospital network available. According to the Brazilian Burns Society website, the reference centers for burn treatment are in Porto Alegre city, at the Hospital Cristo Redentor and Pronto Socorro Hospital. Therefore, the lower average in other regions may be due to hospital transfers to treatment reference centers.

These results provide significant insights into the epidemiology of burns in the region, contributing to a more comprehensive understanding of these occurrences.

**7) Communication and Action**
(main file)

**8) SWOT Analysis**

Strengths:  
- Large volume databases by DATASUS;
- Exchange of knowledge with experts in burn rehabilitation;
- Knowledge for society;
- Possibility of institutional support.

Weakness:
- Data quality in DATASUS;
- Initial research requires further investigation and more advanced techniques;
- Difficulty calculating hospitalization costs directly in DATASUS.

Oportunities:
- Education, prevention and awareness programs;
- Multidisciplinary work;
- Modification of legislation and public policies;
- Comparison of results with other regions and learning from other successful places in prevention.

Threats:
- Dependence on resources and public agents for changes (changes of government and changes of positions);
- Underreporting of data, filling errors;
- Project not very attractive for financing.
