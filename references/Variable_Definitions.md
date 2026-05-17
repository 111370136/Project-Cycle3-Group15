# Variable Definitions
## Selected Behavior Variable
- **Variable Name:** `CurrentCigaretteUse`
- **What the variable measures:** The number of days the student smoked cigarettes during the past 30 days.
- **Recoding used in this project:**
    -`raw code 1` -> `smoker_binary = 0`
    -`raw codes 2 to 7` -> `smoker_binary = 1`
- **How missing or invalid values are handled:** Removed from the formal proportion analysis using listwise deletion.

## Selected Grouping Variable
- **Variable Name:** `WhatIsYourSex`
- **What the variable measures:** The biological sex of the student. 
- **Valid Codes:**
    - `1` = Female
    - `2` = Male
- **Recoding used in this project:**
    - `1` -> `Female`
    - `2` -> `Male`
- **How missing or invalid values are handled:** Removed from the analysis if the response is missing or invalid.

## Logic-Check Variable
- **Variable Name:** `EverCigaretteUse`
- **What the variable measures:** Whether the student has ever tried cigarette smoking, even one or two puffs.
- **Valid Codes:**
    - `1` = Yes
    - `2` = No
- **Data Cleaning Rule:** If a respondent answered `2` (No) for `EverCigaretteUse` but was recorded as `1` (Current smoker) in `CurrentCigaretteUse`, it is flagged as a logical contradiction and removed from the dataset.
- **How missing or invalid values are handled:** Removed from the analysis if the response is missing or invalid.
## Final Valid Sample Size
-**Total:** 13,025 students
-**Male Group (n_1):** 6,420 students
-**Female Group (n_2):** 6,605 students
