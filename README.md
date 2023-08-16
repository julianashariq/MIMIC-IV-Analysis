# NUS SPH6004 Advanced Statistical Learning Assignment 1

## Dataset Description
MIMIC database is a large, freely-available database comprising of de-identified health-related data of over forty thousand patients who stayed in critical care units at the Beth Israel Deaconess Medical Center. The database includes information such as demographics, vital sign measurements made at the bedside (~1 data point per hour), laboratory test results, procedures, medications, caregiver notes, imaging reports, and mortality (both in and out of hospital). MIMIC-IV verson 2.1 (released Nov 14 2022), is the latest version of the MIMIC dataset. 

You can read more about MIMIC-IV from the following resources:
- [The MIMIC-IV PhysioNet project page](https://physionet.org/content/mimiciv/2.2/)
- [The MIMIC-IV online documentation](https://mimic.mit.edu/)

To apply for access to the MIMIC-IV dataset, head over to the [MIMIC-IV page](https://mimic.mit.edu/docs/gettingstarted/) for instructions.

## Asssignment Objective
An extracted dataset of patients’ snapshot of health status at admission that comprises of many features/variables was used for this assignment.The main objective was to develop a strategy to select the right combination of features to build a predictor that estimates the patients’ chance of intubation in the Intensive Care Unit (ICU).

## Background
Endotracheal intubation is a common procedure in the ICU to protect a patient’s airway or provide invasive mechanical ventilation when a patient experiences respiratory failure. Intubation of ICU critically-ill patients is correlated with high complications and high mortality rate due to its emergent nature as compared to elective intubation. The timing to intubate is specific to the patient’s presenting condition and physicians in the ICU have to weigh the risks between intubating and delaying intubation, which is also associated with its own mortality and complication risks. Decision support systems such as predictive models to estimate the patients’ chances of intubation in the ICU may be of help in providing an early warning to physicians before the manifestation of respiratory distress or failure. Through this, potentially circumventing emergent intubation and its consequent high mortality and complication rates. The features included in the predictive model should be available during the early stages of admission in the ICU prior to any tests done due to deterioration of the patient condition. The features should also be easily obtainable and well-generalizable to ensure the usability of the model in various ICU settings.

## Files
- Preprocessing.ipynb details the dataset descriptive analysis and the data cleaning methods such as re-coding, handling missing values, removing outliers, feature scaling and balancing outcome class
- LR,_Tree_based_Models,_SVM.ipynb details the dimensionality reduction methods used (literature review, feature selection and regularization) as well as the predictive models (logistic regression, Decision Tree, Random Forest, AdaBoost, Extreme Gradient Boosting (XGBoost), and Support Vector Machine (SVM) linear and non-linear)
