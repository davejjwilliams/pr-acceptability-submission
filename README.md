# Replication Package: "What Factors are Associated with Agentic Pull Request Acceptance? Initial Results from the AIDev Dataset"

## Repository Structure

- [`data_prep.ipynb`](./data_prep.ipynb): Notebook for dataset retrieval, annotation and filtering
- [`limitations_dataset.ipynb`](./limitations_dataset.ipynb): Notebook for analysis conducted in Section 3
- [`README.MD`](./README.md): This README file
- [`requirements.txt`](./requirements.txt): Dependencies for all analysis
- [`rq1.ipynb`](./rq1.ipynb): Notebook containing all analysis conducted for individual factor analysis in RQ1
- [`rq2_task_label_check.ipynb`](./rq2_task_label_check.ipynb): Notebook containing sanity check for task type label accuracy (used in RQ2 and discussed in threats to validity)
- [`rq2_task_labels_rater1.csv`](./rq2_task_labels_rater1.csv) & [`rq2_task_labels_rater2.csv`](./rq2_task_labels_rater2.csv): Independent manual labelling of task types for 300 agentic PR by two authors
- [`rq2.ipynb`](./rq2.ipynb): Notebook containing all analysis conducted for repository subset case studies in RQ2
- [`utils.py`](./utils.py): Util analysis functions used across both RQ1 and RQ2 analysis


## How to Reproduce Results

### 1. Setup

1. Create a virtual environment.

```bash
python -m venv venv
```

2. Load virtual environment.

Linux/MacOS:

```bash
source venv/bin/activate
```

Windows:

```bash
venv/Scripts/activate
```

3. Install dependencies.

```bash
pip install -r requirements.txt
```

### 2. Retrieve & Filter Dataset

Before continuing to the analysis scripts, run the cells in the [`data_prep.ipynb`](./data_prep.ipynb) notebook to annotate the PR dataframe with additional columns (e.g. time to close, number of commits/reviews, etc.).

### 3. RQ1: Individual Factor Analysis

The analysis for RQ1 can be found in the [`rq1.ipynb`](./rq1.ipynb) notebook.
You can reproduce all of the results presented in the paper under RQ1 by running the cells in this notebook.

### 4. RQ2: Case Study of Repository Subsets

The analysis for RQ1 can be found in the [`rq2.ipynb`](./rq2.ipynb) notebook.
You can reproduce all of the results presented in the paper under RQ2 by running the cells in this notebook.

### 5. Data and Ethical Limitations

The analysis for the numbers reported in Sections 4 and 5 can be found in the [`limitations_dataset.ipynb`](./limitations_dataset.ipynb) notebook.
Running all cells will produce the findings presented in the paper.
