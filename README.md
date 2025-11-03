# Data Sensitivity Classification
I developed an AI tool that analyzes a dataset and assesses the data sensitivity of each column. You can customize the classification policy to suit your needs. The process enables your organization to categorize data more quickly and effectively—with transparent AI-based reasoning behind each decision. The underlying LLM is Google’s [gemini-2.5-flash](https://deepmind.google/models/gemini/flash/).

The output is generated as an Excel spreadsheet containing each column name, its classification, and the reason for that classification—plus a summary tab showing counts per category.

# Raw Data Preview
I used a data faker to generate synthetic data:
<img width="1684" height="191" alt="synthetic user records" src="https://github.com/user-attachments/assets/5d9e57c6-f3aa-4379-a6fc-77f7e75fca55" />


# Outputs
Each data column is categorized and reasoning for each classification is given.
<img width="1365" height="269" alt="classification results" src="https://github.com/user-attachments/assets/06f2eb8e-c49a-4e5e-8d6f-4492faf4bb23" />
<img width="288" height="149" alt="classification summary" src="https://github.com/user-attachments/assets/ede14a9a-1a81-468a-868e-b662fb676380" />

# Evaluation
Velocity: 3 seconds to output generation. Accurate run time depends on the volume of data. For a dataset with 50 rows 9 columns, took 3s. For 500 rows and 122 columns took 30s.


Consistency: CV = 0.031

Coefficient of Variation (CV) = (Standard Deviation) ÷ (Mean)
Lower CV → higher consistency.

Value: Spent < CA$0.3 on ~10 runs of the demo notebook

