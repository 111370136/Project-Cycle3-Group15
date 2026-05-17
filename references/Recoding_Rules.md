# Recoding Rules
## Formal Behavior Variable
- **Raw Variable: `CurrentCigaretteUse`
- **Recoding used in this project:
    -`raw code 1` -> `smoker_binary = 0`
    -`raw codes 2 to 7` -> `smoker_binary = 1`
    -`Anything else or missing` -> `NA`

## Formal Grouping Variable
- **Raw Variable:** `WhatIsYourSex`
- **Recoding used** in this project:
    -`raw code 1` -> `Female`
    -`raw code 2` -> `Male`
    -`Anything else or missing` -> `NA`

## Logic-Check Variable
- **Raw Variable:** `EverCigaretteUse`
- **Cleaning Rule**
    -If a respondent answered `raw code 2` (No, never smoked) for `EverCigaretteUse` but was recorded as `smoker_binary = 1` (Current smoker) based on `CurrentCigaretteUse`, this is flagged as a logical contradiction.
    - **Action:** These contradictory responses are treated as invalid and are filtered out (`NA`) to ensure data integrity.
    
## Missing Data & Sample Size Summary
- **Handling Method:** Listwise Deletion. A case is dropped if it contains a missing value (`NA`) or logical inconsistency in any of the three target variables.
