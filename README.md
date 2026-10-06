# DecodeLabs AI Project 2: Student Performance Classification

This beginner-friendly project uses Logistic Regression to classify a student's result as `Pass` or `Fail` from study hours, attendance, assignments, and previous score.

## Project Structure

```text
AI_Project_2/
├── data/
│   └── student_classification_dataset.csv
├── notebooks/
│   └── classification_model.ipynb
├── README.md
└── requirements.txt
```

## Requirements

- Python 3.9 or later
- Jupyter Notebook

## Setup

Open a terminal in the `AI_Project_2` folder and install the required packages:

```bash
python -m pip install -r requirements.txt
```

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open `notebooks/classification_model.ipynb` and run the cells from top to bottom. The notebook reads the dataset using a path relative to the notebook, so keep the project structure intact.

## What the Notebook Does

1. Loads and inspects the CSV dataset.
2. Separates the four input features from the `result` target.
3. Splits the records into training and test sets, keeping the class proportions with stratification.
4. Trains a Logistic Regression classifier.
5. Evaluates test predictions with accuracy, a confusion matrix, and a classification report.
6. Predicts the result for one example student.

## Dataset Columns

| Column | Meaning | Role |
| --- | --- | --- |
| `study_hours` | Hours spent studying | Feature |
| `attendance` | Attendance percentage | Feature |
| `assignments` | Assignments completed | Feature |
| `previous_score` | Previous assessment score | Feature |
| `result` | `Pass` or `Fail` | Target |

## Important Note

The included dataset has only 30 records, so its test metrics are illustrative and can vary with different data. This model is for learning and demonstration only; it should not be used to make real academic decisions about students.
