# Replication Package: "What Makes an Agentic Pull Request Likely to be Accepted? Insights and Limitations From the Analysis of the AIDev Dataset"

## Repository Structure

- [`data_prep.ipynb`](./data_prep.ipynb): Notebook for dataset annotation and filtering
- [`limitations_guidelines.ipynb`](./limitations_guidelines.ipynb): Notebook for analysis conducted in Section 3
- [`README.MD`](./README.md): This README file
- [`requirements.txt`](./requirements.txt): Dependencies for all analysis
- [`rq1.ipynb`](./rq1.ipynb): Notebook containing all analysis conducted for individual factor analysis in RQ1
- [`rq2.ipynb`](./rq2.ipynb): Notebook containing all analysis conducted for per-repository case studies in RQ2
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

The analysis for the numbers reported in Section 3 can be found in the [`limitations_guidelines.ipynb`](./limitations_guidelines.ipynb) notebook.
Running all cells will produce the findings presented in the paper.
