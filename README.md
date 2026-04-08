# Health-Impact-Analysis-of-Smoking-Power-Bi-dashboard-
This is a Smoking Health Risk Analysis dashboard, built in Power BI with an interactive anatomical navigation panel on the left side. It analyses health data for 310 total patients, examining the relationship between smoking behaviour and organ-level health outcomes across five body systems: Heart, Human Body (general), Kidney, Liver, and Lungs. The dashboard tracks smoking status distribution, smoking duration, and daily intake by age group, cholesterol and hypertension risk, and smoking patterns by gender. This is a clinical or public health analytics tool designed to support medical researchers, health policymakers, or wellness programme designers in understanding how smoking impacts specific organs across different demographic groups.


[![Smoking Health Analysis](https://cdnb.artstation.com/p/assets/images/images/018/539/303/large/anatomy-for-sculptors-12028814-825746584191159-7396937415402469624-o.jpg?1559754582)](https://cdnb.artstation.com/p/assets/images/images/018/539/303/large/anatomy-for-sculptors-12028814-825746584191159-7396937415402469624-o.jpg?1559754582)

## Data Cleaning Steps
1. Patient record deduplication — Each of the 310 patients was confirmed to have a unique patient ID. 
2. Smoking status standardisation — Fields contained inconsistent entries such as "ex-smoker", "quit", "non-smoker", and "passive smoker". These were collapsed into exactly three categories — "Never", "Current", and "Former".
3. Age banding — Continuous age values were grouped into six uniform bands: 18–28, 29–38, 39–48, 49–58, 59–68, and 69+. 
4. Cholesterol and hypertension risk classification — Raw cholesterol readings (in mg/dL) and blood pressure values were classified into "High", "Normal", and "Low" risk categories using standard clinical thresholds.
5. Gender field encoding — Gender was standardised to a binary "Female" / "Male" classification, and any non-standard entries (e.g., blanks, "Unknown", or free-text) were   excluded from the data set
6. Smoking duration and daily intake cleaning — Numeric fields for daily cigarette intake and years of smoking duration were reviewed for implausible values
7. Null and missing value treatment — Key clinical fields (BMI, cholesterol, blood pressure, smoking status) were checked for nulls and deleted.
8. Organ damage state assignment — Each patient's relevant organ health records were classified into "Damaged" or "Healthy" states based on clinical markers (e.g., elevated liver enzymes for liver damage, reduced FEV1 for lung damage, coronary artery indicators for heart damage). 



## Key Performance Indicators (KPIs)
-- Total patients

-- Average age

-- Average BMI

-- Never smoked

-- Current smokers

-- Former smokers

-- Organ views available

-- Health state toggle

-- Age groups tracked

-- Gender breakdown


## Obersavtions

-- Nearly 60% of patients have a smoking history: Current (30.32%) and former smokers (29.35%) together represent 59.67% of the 310-patient cohort. Only 40.32% have never smoked, meaning the majority carry smoking-related health risk — either active or residual.

-- Average BMI of 29.3 sits at the overweight boundary: A BMI of 29.3 is just below the clinical obesity threshold of 30. Combined with a smoking history in nearly 60% of patients, this cohort faces compounded cardiovascular and metabolic risk factors simultaneously.

-- Smoking duration and intake peaks in the 18–28 age group: The line chart for smoking duration and daily intake across age groups shows a dramatic upswing for the 18–28 cohort. Older groups (59–68, 49–58) show lower or declining values, suggesting either cessation trends or survivor bias among older patients.

-- High cholesterol and hypertension are present across all age groups: The stacked bar chart shows High, Low, and Normal cholesterol/hypertension risk across all six age bands (18–28 through 69+). The "High" category (orange) is consistently present in every band, with no age group showing predominantly "Normal" status.

-- Males dominate the "Current" and "Former" smoker categories: In the smoking status by gender chart, the dark blue (Male) segment is visibly larger than the light blue (Female) for both "Current" and "Former" status. "Never" smokers appear more gender-balanced, suggesting male patients in this cohort have significantly higher smoking exposure.

-- Never smokers form the largest single group at 40.32%: The "Never" category at 40.32% provides a meaningful control baseline for comparison against current and former smokers. This group is expected to show lower organ damage rates, lower cholesterol risk, and healthier BMI distributions when filtered.

-- Former smokers at 29.35% remain a significant at-risk group: Former smokers are nearly as large a group as current smokers (29.35% vs 30.32%). Research consistently shows residual cardiovascular, pulmonary, and hepatic risk persists years after cessation; this group should not be treated as low-risk in clinical planning.


## Conclusion
The Smoking Health Risk Analysis dashboard presents a clinically sobering picture of a 310-patient cohort where nearly 60% carry an active or historical smoking burden. The average age of 54.6 and average BMI of 29.3 place this population at elevated baseline risk even before smoking history is factored in. The data confirms that smoking-related harm in this cohort is not isolated to a single organ system; the dashboard's organ navigation across Heart, Kidney, Liver, Lungs, and full Body implies systemic damage patterns. The youngest age group (18–28) shows the highest smoking duration and daily intake values, a deeply concerning trend suggesting the most aggressive smoking behaviour is occurring in the youngest patients, which will translate into compounded organ damage risk over the coming decades. 

## Recommendations
1. Prioritise cessation interventions for the 18–28 age group immediately. The spike in smoking duration and daily intake among the youngest cohort is the single most urgent finding in this dashboard. Young-onset heavy smoking produces dramatically worse long-term organ outcomes than late-onset smoking. Targeted school, campus, and community cessation programmes, including pharmacological support (varenicline, NRT), behavioural therapy, and digital health apps, should be directed at this demographic as a first priority.
2. Do not treat former smokers as low-risk patients. With 29.35% of the cohort former smokers, and their risk profile nearly matching that of current smokers in absolute terms, clinical protocols should include regular screening for lung function, liver enzymes, cardiac markers, and kidney function in all ex-smokers, not just active ones. 
3. Address the dual risk of high BMI and smoking in combination. An average BMI of 29.3 alongside a 59.67% smoking history rate means a large proportion of these patients face simultaneous cardiovascular, metabolic, and pulmonary risk factors. Integrated care pathways combining smoking cessation support with weight management counselling, dietary intervention, and physical activity programmes would be more effective than treating each condition in isolation.
4. Deploy gender-targeted smoking cessation programmes. Since males dominate the current and former smoker categories, male-specific cessation strategies — such as workplace programmes, men's health campaigns, or GP-led brief interventions should be developed. Female smoking patterns in this cohort appear lower but should still be monitored, particularly given the specific risks smoking poses for female cardiovascular and reproductive health.
 
