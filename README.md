# Assignment 1: Data Profiling (EDA) Report – OULAD

**TTTC3213 Data Engineering**

| No. | Name | Matric No. |
|---|---|---|
| 1 | KHEW JUN YU | A216372 |
| 2 | SARAVANA A/L VISVANATHAN | A216453 |
| 3 | ABDUL HADEE BIN JAAPAR | A221505 |

## Scenario
The Open University wants to reduce student dropout. We profile and clean the Open University Learning Analytics Dataset (OULAD) to check which early signs in online activity and assessment results can be trusted to show students at risk of withdrawing or failing.

## Data source
- Open University Learning Analytics Dataset (OULAD), CC-BY 4.0
- https://analyse.kmi.open.ac.uk/open_dataset (also on Kaggle)
- Kuzilek J., Hlosta M., Zdrahal Z. (2017). *Open University Learning Analytics dataset.* Scientific Data 4:170171.

## How to run
1. Download the OULAD zip and unzip it.
2. Put these files in `data/oulad/` (same folder level as the notebook):
   `courses.csv`, `assessments.csv`, `studentInfo.csv`, `studentRegistration.csv`, `studentAssessment.csv`, `studentVle.csv`
3. Install the libraries if needed: `pip install pandas numpy matplotlib`
4. Open `oulad_eda.ipynb` and click **Run All**. It runs from top to bottom.

The data is not included in this repository: `studentVle.csv` is over GitHub's 100 MB limit, and `data/` is excluded by `.gitignore`.
