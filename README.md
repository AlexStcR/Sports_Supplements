# Sports Supplements Effectiveness Analysis

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-1.3%2B-orange)
![Seaborn](https://img.shields.io/badge/Visualization-Seaborn-green)

This project analyzes a dataset of sports supplements to identify key trends and evidence-based recommendations. The analysis is performed using Python with the pandas, numpy, matplotlib, and seaborn libraries.

## Dataset

The dataset used for this analysis is `Sports_Supplements.csv`. It contains information on various sports supplements, including:

* Supplement name
* Alternative names
* Evidence level score
* Claimed improved aspect of fitness
* Fitness category
* And other related data

## How to Use

To replicate this analysis, follow these steps:

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/AlexStcR/Sports_Supplements.git
    cd Sports_Supplements
    ```

2.  **Install the required Python libraries:**

    ```bash
    pip install pandas numpy matplotlib seaborn
    ```

## Step-by-Step Analysis

The analysis is structured as follows:

1.  **Setup and Data Loading**

    * Import necessary libraries.
    * Load the dataset using `pandas.read_csv()`.
    * Perform initial inspection using `df.head()`, `df.info()`, and `df.describe()` to understand the data structure. 

2.  **Data Cleaning**

    * Check for missing values using `df.isnull().sum()`.
    * Clean column names by removing spaces and special characters. 
    * Convert the 'evidence\_level\_score' column to numeric. 
    * Clean and convert the '%\_positive\_studies/\_trials' column to numeric. 

3.  **Exploratory Data Analysis (EDA)**

    * Visualize the distribution of evidence levels. 
    * Identify the top supplements by the number of studies. 
    * Explore the relationship between evidence level and positive study percentage. 

4.  **Effectiveness Analysis**

    * Define criteria for supplement effectiveness. 
    * Filter the dataset to include only effective supplements. 
    * Group effective supplements by fitness category.

5.  **Detailed Analysis by Performance Type**

    * Analyze supplements for strength/power, endurance, and recovery. 
    * Identify the top 5 supplements in each category based on evidence level and positive study percentage. 

6.  **Visualization of Results**

    * Create visualizations to compare supplement effectiveness across categories.
    * Generate plots to highlight key findings.

7.  **Final Analysis and Recommendations**

    * Determine the most researched supplements. 
    * Identify supplements with the highest evidence scores.
    * Provide overall supplement recommendations based on the analysis.

## Key Findings

The analysis reveals several important insights:

* **Most Effective Supplements Overall:**
    * Creatine (strength/power)
    * Whey protein (muscle building/recovery) 
    * Caffeine (endurance) 
    * BCAAs (recovery) 
* **Evidence Strength:**
    * 15 supplements meet the effectiveness criteria (evidence level >= 4, >= 50% positive studies, >= 3 studies).
    * Creatine and whey protein have the highest evidence scores (6).
* **Category-Specific Recommendations:**
    * Strength: Creatine, whey protein, casein
    * Endurance: Caffeine, beetroot juice, baking soda [
    * Recovery: BCAAs, L-carnitine L-tartrate 
* **Most Scientifically Supported Supplements:**
    * Creatine (strength/power) 
    * Whey protein (muscle building/recovery) 
    * Caffeine (endurance)
    * BCAAs (recovery)

## Disclaimer

This analysis is based on the provided dataset and should not be considered medical advice. Always consult with a healthcare professional before starting any new supplement regimen.
