# Project-Cycle3
## Video link
- https://youtu.be/76SYWb5QLOE
## Group Information
- Group number: 15
- Member names: 111370136 詹濬誌, 113370220 游子涵

## Dataset
- Raw data: `YRBS_2007.csv`
- Processed data used across notebooks:`yrbs_smoking_cleaned.csv`
## Selected Project Question & Extension
- **Core Research Question:** Is the proportion of current cigarette use different between male and female students?
- **Advanced Extension Question:** Do adolescent smokers exhibit a higher susceptibility to multi-substance use (alcohol and marijuana) compared to non-smokers? 
## Variables:
### 1. Demographic & Grouping Variable
- `WhatIsYourSex`: Biological sex of the respondent (Recoded to Male / Female).

### 2. Primary Behavioral Variables
- `CurrentCigaretteUse`: Primary response variable for gender difference analysis.
- `CurrentAlcoholUse`: Secondary substance use variable for extension analysis.
- `CurrentMarijuanaUse`: Secondary substance use variable for extension analysis.

### 3. Data Integrity & Logic-Check Variables (Ever Use Experience)
- `EverCigaretteUse`: Used to cross-verify and filter out contradictory smoking responses.
- `EverAlcoholUse`: Used to cross-verify and filter out contradictory alcohol consumption responses.
- `EverMarijuanaUse`: Used to cross-verify and filter out contradictory marijuana use responses.
## Key Methodology & Analytical Pipeline
1. **Data Cleaning & Logic Checking (`01_data.ipynb`):** Standardized raw survey values into binary behaviors and applied custom logic-checks to ensure data integrity.
2. **Statistical Inference & Hypothesis Testing (`02_inference.ipynb` & `03_behavior_variable.ipynb`):** Conducted Two-Sample Z-Tests to analyze gender differences in cigarette usage, as well as gender-stratified differences in alcohol and marijuana prevalence among smokers.
3. **Advanced Visualization (`04_interpretation.ipynb`):** Generated stratified conditional prevalence bar plots, 3-way Venn Diagrams, and UpSet Plots to capture the complex intersection patterns of polysubstance use.
## Final conclusion
- **Core Question:** Among the adolescent population surveyed in the YRBS 2007, there is a statistically significant difference in current smoking proportions between genders, with male students being significantly more likely to be current smokers than female students.
- **Extension Question:** The extension analysis strongly supports the behavioral clustering hypothesis. Smokers show a dramatically higher conditional prevalence of concurrent alcohol use (~86-88%) and marijuana use (~53-63%) compared to non-smokers. Furthermore, while male and female smokers show no significant difference in alcohol co-use, male smokers exhibit a significantly higher rate of marijuana involvement than female smokers.

