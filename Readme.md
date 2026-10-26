# HanuAI ML Assessment — Task 2: Advanced EDA and Text Mining

## Project Overview

This project performs Exploratory Data Analysis (EDA) and text mining on vehicle complaint and repair records. The objective is to identify recurring complaint patterns, extract useful issue and repair-action tags, group similar narratives, and provide actionable insights for stakeholders.

## Objectives

- Inspect dataset structure, data types, missing values, and duplicate records.
- Analyze complaint categories and numerical features using descriptive statistics and visualizations.
- Extract symptom, cause-related, issue, and repair-action tags from text narratives using rule-based keyword matching.
- Apply TF-IDF vectorization and KMeans clustering to explore similar complaint and repair narratives.
- Prepare stakeholder recommendations based on the observed patterns.

## Technology Stack

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Structure

```text
HanuAI_ML_Assignment/
├── data/
│   └── Hanuai_task2_assignment.csv
├── notebooks/
│   └── task2_eda_text_mining.ipynb
├── outputs/
│   ├── HanuAI_Task2_Analyzed.csv
│   ├── HanuAI_Task2_Repair_Summary.csv
│   └── HanuAI_Task2_Tag_Summary.csv
├── reports/
│   └── HanuAI_Task2_Stakeholder_Report.docx
├── README.md
└── requirements.txt
```

## Methodology

1. **Data inspection and cleaning:** Examine schema, data types, missing values, duplicate records, and data integrity.
2. **Exploratory analysis:** Summarize complaint categories and numerical features and visualize important distributions.
3. **Text mining:** Extract issue, symptom, cause-related, and repair-action tags from available narratives using keyword-based rules.
4. **Text clustering:** Convert combined narratives into TF-IDF features and use KMeans to identify exploratory groups of similar records.
5. **Export and reporting:** Save the analyzed dataset and tag summaries as CSV files and prepare a stakeholder report.

## Key Findings

- The dataset contains 1,000 vehicle complaint records.
- The three most frequent complaint categories account for 79.4% of all records.
- Blank/black screen is the most frequent extracted symptom tag.
- Radio replacement and programming are prominent repair-action tags.
- Five exploratory text clusters were generated to investigate recurring narrative patterns.

## Output Files

- **HanuAI_Task2_Analyzed.csv:** Analyzed records and extracted tags.
- **HanuAI_Task2_Tag_Summary.csv:** Combined frequency summary of extracted tags.
- **HanuAI_Task2_Repair_Summary.csv:** Frequency summary of repair actions.
- **HanuAI_Task2_Stakeholder_Report.docx:** Findings, limitations, and recommendations.

## How to Run

1. Install Python 3.10 or a compatible version.
2. Clone or download this repository.
3. Open a terminal in the project directory.
4. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

5. Open the notebook:

   ```bash
   jupyter notebook notebooks/task2_eda_text_mining.ipynb
   ```

6. Run the notebook cells in order. Ensure the source dataset is available in the `data/` directory.

## Limitations

The extracted tags are based on keyword-matching rules and may not capture every possible expression. The KMeans clusters represent textual similarity, not verified engineering root causes. Further validation against repair records and technical investigations would improve reliability.

## Conclusion

This project demonstrates how EDA, rule-based text mining, and unsupervised clustering can help organize vehicle complaint data and support further investigation of recurring issues.
