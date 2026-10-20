# ATP Match Performance Analysis & Training Resource Allocation

**ADS-505: Applied Data Science for Business**
**University of San Diego**
**Team 8: Ryan Salas and Meeki Mee**

## Project Overview
This project examines 22,883 ATP men's professional tennis matches from 2015–2023 to identify match-performance indicators associated with winning and support data-informed coaching and training-resource decisions.

Our intended stakeholder is the Director of Player Development. The analysis is a retrospective performance-auditing framework, not a pre-match prediction tool.

## Business Questions
- Which serve-performance indicators most strongly distinguish winners from losers?
- Can match statistics support consistent post-match reviews?
- How might coaching teams prioritize limited training resources?

## Data Source
Historical ATP match data covering 2015–2023, sourced from the public tennis dataset repository:
https://github.com/migumax/tennis_atp

## Methodology
1. Load and combine seasonal ATP match data.
2. Clean missing values and derive normalized match-performance indicators.
3. Explore serving statistics and winning outcomes.
4. Split the data chronologically: 2015–2020 training, 2021 validation, and 2022–2023 testing.
5. Compare a baseline, logistic regression, and random forest.
6. Evaluate accuracy, F1, ROC AUC, and court-surface performance.

## Main Findings
- First-serve points won: approximately 10.24 percentage-point winner advantage.
- Second-serve points won: approximately 10.84 percentage-point winner advantage.
- First serves in: approximately 1.80 percentage-point winner advantage.
- Logistic regression validation accuracy: 93.82%.
- Logistic regression final test accuracy: 93.13%.

These are observational relationships. Model performance does not prove that changing training routines will cause more match wins.

## How to Run
1. Download or clone this GitHub repository.
2. Install Python and Jupyter.
3. Install the dependencies using `pip install -r requirements.txt`.
4. Open `Team8_Final_Notebook.ipynb` in JupyterLab.
5. Ensure the ATP seasonal CSV files are accessible using the notebook's documented data-loading workflow.
6. Run the notebook cells in sequence and review the results.

## Repository Files
- `Team8_Final_Notebook.ipynb`: main analysis notebook.
- `requirements.txt`: Python dependencies.
- `.gitignore`: excluded temporary and raw-data files.
- `deliverables/`: final business reports and executive presentation.

## Team Contributions
**Ryan Salas:** Initial notebook development, data preparation, exploratory analysis, serve-performance indicators, visualizations, business interpretation, and project documentation.

**Meeki Mee:** Modeling workflows, baseline and machine-learning comparisons, evaluation metrics, validation and test analysis, model interpretation, and notebook updates.

Both team members should verify these descriptions against their actual contributions.

## Recommendations and Limitations
Pilot a coaching framework emphasizing first- and second-serve effectiveness, placement, and serve-plus-one execution. Evaluate results before implementing large-scale changes.

The framework uses completed-match statistics and cannot predict outcomes before a match. Observational associations do not establish causality.

## AI Assistance Disclosure
ChatGPT was used to assist with project development, code review, explanations, and documentation. All contributions should be reviewed, verified, and disclosed in accordance with course requirements.

## References
ATP dataset: https://github.com/migumax/tennis_atp

scikit-learn documentation: https://scikit-learn.org/stable/
