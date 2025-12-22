# Replication Package: "What Makes an Agentic Pull Request Likely to be Accepted? Insights and Limitations From the Analysis of the AIDev Dataset"

## Repository Structure

- [`requirements.txt`](./requirements.txt): Dependencies for all analysis

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

Before continuing to analysis scripts, run the cells in the [`data_prep.ipynb`](./data_prep.ipynb) notebook to annotate the PR dataframe with additional columns (e.g. time to close, number of commits/reviews, etc.).

### 3. RQ1: Individual Factor Analysis

The analysis for RQ1 can be found in the [`rq1.ipynb`](./rq1.ipynb) notebook.

Running all cells will produce the findings presented in the paper.

### 4. RQ2: Case Study of Repository Subsets

The analysis for RQ1 can be found in the [`rq2.ipynb`](./rq2.ipynb) notebook.

Running all cells will produce the findings presented in the paper.
