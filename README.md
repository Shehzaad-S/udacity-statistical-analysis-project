## Data and Statistical Reasoning Project

### Project Description

This project explores factors associated with student academic performance using the Students Performance in Exams dataset. Using Python, Pandas, SciPy, Matplotlib, and Seaborn, the project demonstrates a reproducible statistical analysis workflow including data loading, descriptive statistics, exploratory data analysis (EDA), visualization, assumption testing, and hypothesis testing.

The primary objective of the analysis is to investigate whether math performance differs across parental education levels using a one-way ANOVA. In addition to hypothesis testing, the project evaluates statistical assumptions and examines both statistical and practical significance.

**What I Built:**

- Loaded and validated the Students Performance in Exams dataset.
- Performed descriptive statistical analysis on both numerical and categorical variables.
- Examined distributions of math, reading, and writing scores.
- Created visualizations to investigate score distributions and differences across parental education groups.
- Assessed ANOVA assumptions using distribution diagnostics, skewness, kurtosis, and Levene's Test for homogeneity of variance.
- Conducted a one-way ANOVA to evaluate differences in mathematics performance across parental education levels.
- Calculated eta-squared ($\eta^2$) to assess practical significance.
- Summarized key findings, limitations, and statistical considerations.

**Research Question**

_Do mathematics scores differ significantly across parental education levels?_

`Null Hypothesis (H0)`

The mean math score is equal across all parental education groups.

`Alternative Hypothesis (H1)`

At least one parental education group has a mean math score that differs from the others.

**Dataset:**

Students Performance in Exams

Source (Kaggle):

[Students Performance in Exams on Kaggle](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)

**File used:**

StudentsPerformance.csv

**Dataset Characteristics:**

1,000 observations
8 variables

Numerical variables:

- Math Score
- Reading Score
- Writing Score

Categorical variables:

- Gender
- Race/Ethnicity
- Parental Level of Education
- Lunch
- Test Preparation Course

**Bias Awareness and Limitations**

As with all observational datasets, the results should be interpreted with caution. While parental education was found to be associated with math performance, this does not establish a causal relationship.

Potential limitations include:

The dataset does not contain information on household income, school quality, geographic location, or student motivation.
Unmeasured confounding variables may influence student performance.
The dataset represents a specific population and may not generalize to all educational contexts.
Parental education explained only a small proportion of the variation in mathematics scores, indicating the presence of additional influential factors.

Care was taken throughout the project to avoid causal interpretations and to distinguish between statistical significance and practical significance.

**Future Statistical Extensions**

Several opportunities exist to extend this analysis:

`Two-Way ANOVA`

A useful extension would be a two-way ANOVA incorporating:

Parental Education Level
Lunch Status

This approach would allow investigation of:

The main effect of parental education.
The main effect of lunch status.
Potential interaction effects between socioeconomic indicators and educational background.

`Post-Hoc Analysis`

Future work could include Tukeys Honest Significant Difference (HSD) procedure to identify which parental education groups differ significantly from one another following the ANOVA.

`Multiple Regression`

A multiple regression model could evaluate the combined contribution of:

Parental education
Lunch status
Test preparation participation
Gender
Race/Ethnicity

to student mathematics performance.

**How to Run the Project:**

1. Clone the Repository

```Shell
git clone <repository-url>
```

```Shell
cd udacity-statistical-analysis-project

```

2. Create and Activate an Environment

Using Conda:

```Shell
conda env create -f environment.yml
```

```Shell
conda activate statistical-analysis
```

Using venv

```Shell
python -m venv statistical-analysis
```

Windows:

```Shell
statistical-analysis\Scripts\activate.bat
```

3. Install Dependencies

Python version:

```Plain Text

Python 3.11+
```

Using pip:

```Shell
pip install -r requirements.txt
```

Using Conda:

```Shell
conda env create -f environment.yml
```

4. Open the Notebook

Launch Jupyter:

```Shell

jupyter notebook
```

Open in code editor:

```Click
analysis.ipynb
```

Run all cells from top to bottom.

**Reproducibility:**

Generate the requirements file:

```Shell
pip freeze > requirements.txt
```

Generate the Conda environment specification:

```Shell
conda env export > environment.yml
```

The requirements.txt and environment.yml files are included in this repository to support reproducibility and environment recreation.
