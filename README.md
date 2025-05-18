# A/B Testing for Landing Page Engagement
![image](https://github.com/user-attachments/assets/d23a9e05-2077-47ca-b2bf-875b453926c3)


This project performs an A/B test to determine which landing page (A or B) retains users for a longer duration, indicating higher engagement.

## Overview

This project performs an **A/B testing statistical analysis** to compare user engagement between two different landing pages — **Page A** and **Page B**. The goal is to identify which page leads to longer user interactions, using **exploratory data analysis (EDA)** and **statistical hypothesis testing** techniques.

If you're interested in data-driven decision-making, website optimization, or learning practical A/B testing using Python, this notebook is a valuable hands-on resource.


## Key Question

**Do users spend more time on Landing Page B compared to Landing Page A, suggesting higher engagement and better selling potential?**

## 🚀 Key Features

- ✅ Clean and structured **pandas-based data analysis**
- 📈 Visualizations using **Matplotlib** and **Seaborn**
- 📊 **Box plots, histograms, violin plots** for page comparison
- 🧪 **Hypothesis testing** using **t-tests** with SciPy
- ✅ Detects significant differences in page engagement
- 📦 Readable and reproducible Jupyter notebook

## 📁 Dataset

- **File Name:** `web_page_data.csv`
- **Source:** Kaggle (A/B Testing Dataset)
- **Columns:**
  - `Page`: Type of landing page (`PAGE A`, `PAGE B`)
  - `Time`: Time spent on the page (multiplied by 100 to convert to hundredths of seconds)

## Analysis

1.  **Data Loading and Exploration:**
    * Loads the data using Pandas.
    * Displays the first few rows to understand the data structure.
    * Converts the `Time` column from minutes to seconds for easier interpretation.
    * Examines data types and missing values.
    * Provides descriptive statistics of the `Time` column.

2.  **Visualizations:**
    * Box Plot – Compare distributions and outliers across pages.
    * Histogram with KDE – View the frequency distribution of engagement time.
    * Violin Plot – Detailed comparison of distribution shapes.

3.  **Statistical Analysis:**
    * **Normality Check:**
        * Uses the Shapiro-Wilk test to assess if the time spent on each page follows a normal distribution.
        * Visualizes the data with histograms and Q-Q plots to further inspect normality.
    * **Homogeneity of Variance Check:**
        * Applies Levene's test to determine if the variances of the two groups (Page A and Page B) are equal.
    * **Hypothesis Testing:**
        * Performs the Mann-Whitney U test (a non-parametric test) to compare the time spent on the two pages, as the data for Page A is not normally distributed.
        * States the null hypothesis (H0: There is no difference in time spent on Page A and Page B) and the alternative hypothesis (H1: Users spend more time on one page than the other).
        * Determines statistical significance based on the p-value.

## Findings

* **Descriptive Statistics:** Provides summary statistics (mean, standard deviation, etc.) for time spent on each page.
* **Normality Test Results:** Indicates whether the data for each page is normally distributed.
* **Variance Test Results:** Shows if the variances of the two groups are equal.
* **Mann-Whitney U Test Results:**
    * Reports the U statistic and p-value.
    * States whether the null hypothesis is rejected or not.
    * Interprets the practical significance of the findings in terms of user engagement.

## Conclusion

The analysis concludes whether there is a statistically significant difference in the time users spend on Landing Page A versus Landing Page B. It provides insights into which page design is more effective at engaging users, which can inform decisions about website design and marketing strategies.

## Repository Contents

* `a-b-testing-page-engagement-for-lan (1).ipynb`: Jupyter Notebook containing the analysis code.
* `web_page_data.csv`:  The dataset used for the A/B testing.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scipy (stats)

## Setup and Installation

1.  **Ensure you have Python installed (preferably Python 3.6 or later).**

2.  **Install the required libraries:**

    ```bash
    pip install numpy pandas matplotlib seaborn scipy
    ```

3.  **Clone the repository to your local machine.**

4.  **Navigate to the repository directory and open the Jupyter Notebook (`a-b-testing-page-engagement-for-lan (1).ipynb`) to run the analysis.**

## Usage

1.  Place the `web_page_data.csv` file in the same directory as the Jupyter Notebook.
2.  Open and run the Jupyter Notebook in your preferred environment (JupyterLab, Jupyter Notebook, VS Code with Jupyter extension, etc.).
3.  Follow the steps outlined in the notebook to reproduce the analysis and view the results.

## Author
[Lutfor Rahman Sohan]([url](https://www.linkedin.com/in/lutfor-rahman-sohan/))
