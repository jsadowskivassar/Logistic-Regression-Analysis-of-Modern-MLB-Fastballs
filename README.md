# Missing Bats: A Logistic Regression Analysis of Modern MLB Fastballs

Link to paper: 

## Overview:
This repository contains a statistical analysis identifying the physical and contextual characteristics that make Major League Baseball fastballs difficult to hit. By analyzing MLB Statcast data, the project models swing-and-miss (whiff) probabilities to quantify pitcher deception and mathematically isolate the "Dead Zone".

## Statistical Approach
The predictive model was built using a binomial logistic regression on an isolated dataset of 6,448 swung-at fastballs.
* **Predictive Power:** The final adjusted model demonstrated strong predictive ability, achieving a Concordance Index (C-Index) of 0.71.
* **Handling Non-Linearity:** Implemented 2nd-degree polynomial coefficients to accurately model the non-linear, U-shaped relationships between whiff probability, effective velocity, and induced vertical break.
* **Multivariate Analysis:** Evaluated continuous physical metrics (velocity, horizontal/vertical break, spin deviation) alongside categorical contextual variables (13 standardized spatial zones, pitch counts, and platoon advantages)

## Key Findings
* **The "Dead Zone":** The non-linear modeling proved that fastballs with league-average velocity and average induced vertical break are severely punished by hitters. To consistently generate whiffs, pitchers must leverage outlier traits (e.g., extreme "high ride" or heavy sink).
* **Blueprint to Whiffs:** Pitches located in the upper shadow zones significantly increase whiff probabilities, while deploying fastballs in deeper counts (e.g., 2-2, 3-2) statistically decreases swing-and-miss rates.

## Repository Structure:

