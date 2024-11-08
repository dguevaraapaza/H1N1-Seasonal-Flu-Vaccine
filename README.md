# H1N1 and Seasonal Flu Vaccine (Kaggle)

## Content

The goal is to predict how likely individuals are to receive their H1N1 and seasonal flu vaccines. Specifically, you'll be predicting two probabilities: one for `h1n1_vaccine` and one for `easonal_vaccine` as well as any sophisticates EDAs.

Each row in the dataset represents one person who responded to the National 2009 H1N1 Flu Survey and there are two target variables:

- `h1n1_vaccine`: Whether respondent received H1N1 flu vaccine.
- `seasonal_vaccine`: Whether respondent received seasonal flu vaccine.

Both are binary variables: 0 = No; 1 = Yes. Some respondents didn't get either vaccine, others got only one, and some got both. This is formulated as a multilabel (and not multiclass) problem.

## Variables

The first column `respondent_id` is a unique and random identifier. The remaining 35 features are described below(For all binary variables: 0 = No; 1 = Yes) :

1. `h1n1_concern` *int* - (category) - Level (0 - 3) of concern about the H1N1 flu.
   **Values:** 0 = Not at all concerned; 1 = Not very concerned; 2 = Somewhat concerned; 3 = Very concerned.
2. `h1n1_knowledge` *int* - (category) - Level (0 - 2) of knowledge about H1N1 flu.
   **Values:** 0 = No knowledge; 1 = A little knowledge; 2 = A lot of knowledge.
3. `behavioral_antiviral_meds` *int* - (binary) Has taken antiviral medications.
4. `behavioral_avoidance` *int* - (binary) - Has avoided close contact with others with flu-like symptoms.
5. `behavioral_face_mask` *int* - (binary) - Has bought a face mask.
6. `behavioral_wash_hands` *int* - (binary) - Has frequently washed hands or used hand sanitizer.
7. `behavioral_large_gatherings` *int* - (binary) - Has reduced time at large gatherings.
8. `behavioral_outside_home` *int* - (binary) - Has reduced contact with people outside of own household.
9. `behavioral_touch_face` *int* - (binary) - Has avoided touching eyes, nose, or mouth.
10. `doctor_recc_h1n1` *int* - (binary) - H1N1 flu vaccine was recommended by doctor.
11. `doctor_recc_seasonal` *int* - (binary) - Seasonal flu vaccine was recommended by doctor.
12. `chronic_med_condition` *int* - (binary) - Has any of the following chronic medical conditions: asthma or an other lung condition, diabetes, a heart condition, a kidney condition, sickle cell anemia or other anemia, a neurological or neuromuscular condition, a liver condition, or a weakened immune system caused by a chronic illness or by medicines taken for a chronic illness.
13. `child_under_6_months` *int* - (binary) - Has regular close contact with a child under the age of six months.
14. `health_worker` *int* - (binary) - Is a healthcare worker.
15. `health_insurance` *int* - (binary) - Has health insurance.
16. `opinion_h1n1_vacc_effective` *int* - (categorical) - Respondent's opinion about H1N1 vaccine effectiveness.
    **Values:** 1 = Not at all effective; 2 = Not very effective; 3 = Don't know; 4 = Somewhat effective; 5 = Very effective.
17. `opinion_h1n1_risk` *int* - (categorical) - Respondent's opinion about risk of getting sick with H1N1 flu without vaccine.
    **Values:** 1 = Very Low; 2 = Somewhat low; 3 = Don't know; 4 = Somewhat high; 5 = Very high.
18. `opinion_h1n1_sick_from_vacc` *int* - (categorical) - Respondent's worry of getting sick from taking H1N1 vaccine.
    **Values:** 1 = Not at all worried; 2 = Not very worried; 3 = Don't know; 4 = Somewhat worried; 5 = Very worried.
19. `opinion_seas_vacc_effective` *int* - (categorical) - Respondent's opinion about seasonal flu vaccine effectiveness.
    **Values:** 1 = Not at all effective; 2 = Not very effective; 3 = Don't know; 4 = Somewhat effective; 5 = Very effective.
20. `opinion_seas_risk` *int* - (categorical) - Respondent's opinion about risk of getting sick with seasonal flu without vaccine.
    **Values:** 1 = Very Low; 2 = Somewhat low; 3 = Don't know; 4 = Somewhat high; 5 = Very high.
21. `opinion_seas_sick_from_vacc` *int* - (categorical) - Respondent's worry of getting sick from taking seasonal flu vaccine.
    **Values:** 1 = Not at all worried; 2 = Not very worried; 3 = Don't know; 4 = Somewhat worried; 5 = Very worried.
22. `age_group` - *label* - (categorical) - Age group of respondent.
23. `education` - *label* - (categorical) - Self-reported education level.
24. `race` - *label* - (categorical) - Race of respondent.
25. `sex` - *label* - (categorical) - Gender of respondent.
26. `income_poverty` - *label* - (categorical) - Household annual income of respondent with respect to 2008 Census poverty thresholds.
27. `marital_status` - *label* - (categorical) - Marital status of respondent.
28. `rent_or_own` - *label* - (categorical) - Housing situation of respondent.
29. `employment_status` - *label* - (categorical) - Employment status of respondent.
30. `hhs_geo_region` - *label* - (categorical) - Respondent's residence using a 10-region geographic classification defined by the U.S. Dept. of Health and Human Services. Values are represented as short random character strings.
31. `census_msa` - *label* - (categorical) - Respondent's residence within metropolitan statistical areas (MSA) as defined by the U.S. Census.
32. `household_adults` *int* - (categorical) - Number of other adults in household, top-coded to 3.
33. `household_children` *int* - (categorical) - Number of children in household, top-coded to 3.
34. `employment_industry` - Type of industry respondent is employed in. Values are represented as short random character strings.
35. `employment_occupation` - Type of occupation of respondent. Values are represented as short random character strings.
