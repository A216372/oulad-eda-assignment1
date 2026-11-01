# Assignment 1: Data Profiling (EDA) Report – OULAD

**TTTC3213 Data Engineering**

| No. | Name | Matric No. |
|---|---|---|
| 1 | KHEW JUN YU | A216372 |
| 2 | SARAVANA A/L VISVANATHAN | A216453 |
| 3 | ABDUL HADEE BIN JAAPAR | A221505 |

## Scenario
The Open University wants to reduce student withdrawal in its online courses. We profile and clean the Open University Learning Analytics Dataset (OULAD) to find **when** withdrawal warning signs first appear in students' online activity and early assessment submissions, and whether tutors can be alerted early **without unfairly targeting students by disability or background**.

## Data source
- Open University Learning Analytics Dataset (OULAD), CC-BY 4.0
- https://analyse.kmi.open.ac.uk/open_dataset (also on Kaggle)
- Kuzilek J., Hlosta M., Zdrahal Z. (2017). *Open University Learning Analytics dataset.* Scientific Data 4:170171.

## How to run
1. Download the OULAD zip and unzip it.
2. Put these files in `data/oulad/` (same folder level as the notebook):
   `courses.csv`, `assessments.csv`, `studentInfo.csv`, `studentRegistration.csv`, `studentAssessment.csv`, and `studentVle.csv`.
   The Kaggle copy splits `studentVle.csv` into parts (`studentVle_0.csv` to `studentVle_7.csv`). Put all the parts in the same folder and the notebook joins them automatically.
3. Install the libraries: `pip install -r requirements.txt`
4. Open `oulad_eda.ipynb` and click **Run All**. It runs from top to bottom. `studentVle` has about 10 million rows, so loading it takes about a minute.

The data is not included in this repository: `studentVle.csv` is over GitHub's 100 MB limit, and `data/` is excluded by `.gitignore`.

## What the notebook covers
1. Scenario
2. Data source
3. Data profiling and issue handling (missing values, outliers, duplicates, formats, data types, invalid values)
4. Diagnostic charts (7 charts, including withdrawal timing and weekly activity)
5. PII and bias risks
6. Conclusion
