# Data Dictionary

This data dictionary describes the variables used in the credit portfolio analysis.

The original dataset is confidential and is not included in the public GitHub repository. The variable names below are included to explain the structure of the analysis.

| Variable | Type | Description | Used in analysis |
|---|---|---|---|
| `loan_id` | Categorical or identifier | Anonymised unique loan identifier. | Used for record tracking and risk ranking. |
| `loan_amount` | Numeric | Amount borrowed by the customer. | Used in EDA, visualisation, hypothesis testing, correlation, and regression. |
| `loan_term` | Categorical | Duration or tenor of the loan. | Used to compare loan amount and default rate across loan terms. |
| `is_bad` | Numeric binary | Outcome variable. `1` indicates defaulted or bad loan, `0` indicates repaid or good loan. | Main dependent variable for default and repayment analysis. |
| `gender` | Categorical | Applicant gender as recorded in the anonymised dataset. | Used for portfolio segmentation. |
| `most_recent_credit_date` | Date | Most recent credit activity date. | Used as the required date variable and checked during cleaning. |
| `dependants` | Numeric | Number of dependants recorded for the applicant. | Reviewed during data preparation. |
| `income` | Numeric | Applicant income. | Used as an applicant characteristic in correlation and regression. |
| `application_channel` | Categorical | Channel through which the application was submitted. | Used in visualisation, chi-square testing, and regression. |
| `current_dpd` | Numeric | Current days past due. | Used as a loan performance variable. |
| `max_dpd` | Numeric | Maximum days past due. | Used as a loan performance variable. |
| `has_gps` | Categorical or binary | Indicates whether GPS data was available. | Used as a predictor in regression. |
| `credit_score` | Numeric | Applicant credit score. | Used in correlation analysis, credit score bands, and regression. |
| `repayment_status` | Derived categorical | Derived from `is_bad`. Values are `Repaid` and `Defaulted`. | Used for interpretation and visualisation. |
| `repayment_good` | Derived numeric binary | Derived from `is_bad`. `1` means repaid, `0` means defaulted. | Dependent variable for logistic regression. |
| `log_loan_amount` | Derived numeric | Log-transformed loan amount created to reduce skewness. | Used in hypothesis testing and visualisation. |
| `credit_score_band` | Derived categorical | Credit score divided into five bands. | Used for risk segmentation and visualisation. |

## Confidentiality statement

The original dataset is not included because it is internal organisational data. The public repository includes only this data dictionary and a dummy sample structure file.
