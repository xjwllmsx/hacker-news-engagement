# Engagement Analysis of Hacker News Posts

This project explores which kinds of [Hacker News](https://news.ycombinator.com/) submissions spark the most conversation and when authors should publish questions to maximize engagement. Using a historical snapshot of posts from the popular tech forum, we compare comment activity on Ask HN (questions) versus Show HN (project showcases) and identify the peak posting hours for lively discussion.

## Tech Stack

<div>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" title="Python" width="40" height="40" />&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/jupyter/jupyter-original.svg" title="Jupyter" width="40" height="40" />&nbsp;
</div>

## Contents

-   [Project Structure](#project-structure)
-   [Dataset](#dataset)
-   [View it Online](#view-it-online)
-   [Steps to Run](#steps-to-run)
-   [License](#license)

## Project Structure

```bash
hacker-news-engagement/
├── data/                 # Raw dataset (CSV)
│   └── hacker_news.csv
├── notebook/             # Jupyter Notebook with full analysis
│   └── hacker-news-posts.ipynb
├── .gitignore            # Lists ignored files for version control
├── pyproject.toml        # Dependency and project metadata
├── .python-version       # Defines Python version for virtual environments
├── uv.lock               # Lockfile for reproducible installs
└── README.md             # Project overview and setup instructions
```

## Dataset

The analysis relies on `hacker_news.csv`, a subset of the [Hacker News Posts dataset](https://www.kaggle.com/datasets/hacker-news/hacker-news-posts) originally published on [Kaggle](https://www.kaggle.com/). The CSV contains the submission title, author, Unix timestamp, number of comments, and other metadata for tens of thousands of posts between 2015 – 2017.

> **Note:** To keep the repository lightweight, only the filtered CSV used in this notebook is tracked. For a full refresh you can download the latest dataset from Kaggle and place it in the `data/` folder with the same filename.

## View it Online

Launch the notebook directly in your browser via Binder (no installation required):

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/xjwllmsx/hacker-news-engagement/HEAD?urlpath=%2Fdoc%2Ftree%2Fnotebook%2Fhacker-news-posts.ipynb)

## Steps to Run

Follow these steps to reproduce the analysis locally.

### 1. Clone the repository

```bash
git clone https://github.com/xjwllmws/hacker-news-engagement.git
cd hacker-news-engagement
```

### 2. Create and activate a virtual environment

```bash
uv venv          # create a virtual environment with uv
uv pip install -r requirements.txt  # or use pyproject.toml directly
```

### 3. Launch Jupyter Notebook

```bash
jupyter notebook notebook/hacker-news-posts.ipynb
```

## License

This repository is provided for educational purposes. The Hacker News dataset is redistributed under its original public‑domain terms; all analysis code and notebook content are released under the [MIT License](./LICENSE).
