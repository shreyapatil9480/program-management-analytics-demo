# Project Management Analytics

This repository contains a **synthetic project management dataset** and an accompanying Jupyter notebook for exploratory data analysis (EDA) and predictive modeling.  It is designed to demonstrate analytical skills relevant to **business analysts**, **program managers**, and **data analysts**.

## Dataset Overview

The dataset (`project_management_dataset.csv`) simulates 500 projects with realistic attributes:

| Column | Description |
| --- | --- |
| `Project_ID` | Unique identifier for each project |
| `Start_Date` | Project start date (YYYY‑MM‑DD) |
| `End_Date` | Project end date (YYYY‑MM‑DD) |
| `Planned_Duration` | Planned project duration (days) |
| `Actual_Duration` | Actual project duration (days) |
| `Budget_kUSD` | Planned budget (thousands of USD) |
| `Spent_kUSD` | Actual spend (thousands of USD) |
| `Team_Size` | Number of people assigned to the project |
| `Complexity` | Complexity rating (1–10) |
| `Stakeholder_Engagement` | Stakeholder engagement rating (1–10) |
| `Risk_Level` | Risk level (1–10) |
| `Success` | Binary indicator of project success (1 = on time and within budget with manageable risk; 0 = otherwise) |

The data generation process introduces relationships between variables (e.g., greater complexity increases risk; overruns in duration or spending reduce the chance of success) to mirror real‑world project dynamics.

## Analysis Notebook

The Jupyter notebook (`analysis.ipynb`) demonstrates how to:

1. **Load and inspect the dataset** using `pandas`.
2. **Summarize the data** and check for missing values.
3. **Visualize distributions and relationships** with `matplotlib` and `seaborn`, including histograms, correlation heatmaps, and boxplots.
4. **Build predictive models** with `scikit‑learn`:
   - A **classification model** (logistic regression) to predict project success.
   - A **regression model** (linear regression) to estimate actual project duration.
5. **Evaluate model performance** using accuracy, confusion matrices, mean absolute error (MAE), and R² scores.

The notebook provides increasing levels of difficulty by progressing from simple descriptive statistics to more advanced predictive modeling tasks.



   ```bash
   python -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```

3. Launch Jupyter Notebook:

   ```bash
   jupyter notebook analysis.ipynb
   ```

4. Explore the notebook cells sequentially.  Each section explains the purpose of the analysis and the code used to achieve it.

## Dependencies

Dependencies are listed in `requirements.txt` and include:

- `pandas` – data manipulation
- `numpy` – numerical computations
- `matplotlib` and `seaborn` – visualization
- `scikit‑learn` – machine learning algorithms and evaluation

## Contributing

This repository is intended as a self‑contained demonstration project.  Feel free to fork the repo, experiment with different models or visualizations, or extend the dataset.  Pull requests are welcome.

## License

This project is released under the [MIT License](LICENSE) (if you decide to include a license).  As the data is synthetic, it is free to use for any purpose.
## Getting Started

1. **Clone or download** this repository.
2. Install dependencies:
