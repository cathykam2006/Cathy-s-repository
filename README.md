# U.S. Vaccination Analysis and Prediction

### Problem Statement and Background

Throughout 2020–2022, Covid-19 rampaged rampantly, putting many people’s lives and quality of life at risk.

According to a recent study published by CDC in August 2022, the estimated vaccine effectiveness of two doses of Pfizer-BioNTech vaccine in preventing MIS-C was 84%. Among children ages 5–11, vaccine effectiveness against MIS-C was estimated to be 78%, and among those ages 12–18, it was 90%.

Assuming the vaccine is helpful, we aim to use data to address the following questions in order to assist government officials in better allocating social resources and combating the COVID-19 situation:

1. Which state has the lowest/highest vaccination rate? How can we cater for the need of vaccination based on the state population and positive Covid-19 cases?

2. Which age group has the lowest/highest vaccination rate? If so, how can we better cater for the age group that has the lowest vaccination rate?

3. What is the vaccination trend looking like for the next 3 months?

4. Is there a high demand for booster doses throughout 2020–2022?

5. In which period did the demand for vaccination (administered dose / boosters) seem to decline?

### Source of the dataset

Data-driven decisions will be made through analysis of ‘COVID-19 Vaccination Age and Sex Trends in the United States, National and Jurisdictional’, which is a dataset collected by the Centers for Disease Control and Prevention between 12/13/2020 to 12/14/2022.

Reference: https://data.cdc.gov/Vaccinations/COVID-19-Vaccination-Age-and-Sex-Trends-in-the-Uni/5i5k-6cmh

Based on the data analysis, we will apply the Ridge regression model to (1) predict how many U.S. citizens have already completed the vaccination based on the census data and (2) evaluate whether the current number of vaccinations is sufficient to put COVID-19 under control.

##  Data Description

This dataset contains demographic characteristics (age, sex, and age by sex) of people receiving COVID-19 vaccinations in the United States at the national and jurisdictional levels.

Data represents all vaccine partners including jurisdictional partner clinics, retail pharmacies, long-term care facilities, dialysis centers, Federal Emergency Management Agency and Health Resources and Services Administration partner sites, and federal entity facilities. 

## Data Dictionary 

| Column Name | Data Type | Description |
| --- | --- | --- |
| Date | Object | Date |
| Location | Object | States  |
| Demographic_Category | Object | Ages |
| census | float64 | Population of State  |
| Administered_Dose1 | float64 | Amount of people who got the first dose |
| Series_Complete_Yes | float64 | Amount of people who completed series  |
| Booster_Doses | float64 | Amount of people who received booster  |
| Second_Booster | float64 | Amount of people who received second booster  |
| Administered_Dose1_pct_agegroup | float64 | Agegroup of people who received the first dose  |
| Series_Complete_Pop_pct_agegroup | float64 |Agegroup of people who received the complete series|
| Booster_Doses_Vax_pct_agegroup | float64 |Agegroup of people who received booster  |
| Second_Booster_Vax_pct_agegroup | float64 | Agegroup of people who received the second booster|

# Conclusion / Recommendation
<br>
To sum up, the vaccination rate is satisfactory. And since the number of people who have completed the entire vaccination series is higher than the weekly new positive Covid-19 cases. It is believed that the Covid-19 situation has finally brought under control now.


Wyoming, Guam, North Dakota, Alaska, Vermont, South Dakota have the lowest vaccination rate. While California, Texas, New York, Florida and Pennsylvania have the highest vaccination rate. These states are typically categorized by their greater population density. The government should take the ratio of population and confirmed Covid-19 cases into account in order to reevaluate the need of vaccination.


Of the entire population, the age group 0–12 has the lowest vaccination rate, which is also known as the infants and toddlers. Meanwhile, age group 25–49, 50–64, 65+ have the highest vaccination rate among all.

Vaccine companies, such as Pfizer, should provide a vaccine that tailored for children > 12, with a smaller dose of COVID-19 vaccine than teens and adults, so as to minimize the adverse effects that parents were concerning.


It is predicted that the number of people who will have completed the vaccination will more or less reach to plateau in the next 3 months. However, the number of new receival of the 1st dose and the boosters will significantly plummet and perhaps reach to a bottom.


The number of people completing booster doses increased drastically from 2021–10 to 2022–02, but the growth is expected to slow down after then and reach to a plateau soon.


The accumulative number of administered dose 1 completion slowed down drastically from 2021–01 to 2022–12. The demand for administered dose 1 dropped drastically after 2022 November. While the boosters share more or less the same patterns with administered dose 1.
