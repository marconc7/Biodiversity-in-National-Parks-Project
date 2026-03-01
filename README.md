# Biodiversity in U.S. National Parks 🌿

## 📌 Project Overview

This project analyzes biodiversity data from the **U.S. National Park Service**, focusing on four specific parks: **Yellowstone, Yosemite, Bryce, and Great Smoky Mountains**. 

Using data-driven analysis, we aim to uncover patterns in species endangerment and determine if certain taxonomic groups face higher risks of extinction. By analyzing the different species along with their conservation status, we seek to provide insights into which species groups are at the greatest conservation risk. Specifically, this study evaluates the distribution of conservation statuses, tests the statistical significance of the association between the species category and its protection status, and identifies the most frequently observed species within each park.

## 🎯 Objectives

The main research questions we will seek to answer are the following:

* **Distribution Analysis:** Characterize the conservation status across 5,541 unique species.

* **Risk Assessment:** Identify which types of species (Mammals, Birds, etc.) are most likely to be endangered.

* **Statistical Significance:** Use Chi-Square testing to see if protection status is significantly linked to species category.

* **Observation Patterns:** Analyze over 3.3 million sightings to find the most common species in each park.



## 🗂️ Data Sources

Both `Observations.csv` and `Species_info.csv` was provided by [Codecademy.com](https://www.codecademy.com).

Note: The data for this project is *inspired* by real data, but is mostly fictional.


## 🛠️ Tech Stack & Libraries

* **Language:** Python 3

* **Data Manipulation:** `pandas`, `numpy`

* **Visualization:** `matplotlib`, `seaborn`

* **Statistical Analysis:** `scipy.stats` (specifically `chi2_contingency`)


## 📈 Data Processing & Methodology

The analysis followed a structured workflow to ensure data integrity:

1. **Data Cleaning:** Handled missing and duplicate values in both `observations` and `species_info` datasets.
2. **Feature Engineering:** Created an `is_protected` categorical variable to simplify the "at-risk" vs. "not-at-risk" comparison.
3. **Data Merging:** Combined the `species` and `observations` datasets to map sightings to specific conservation categories.
4. **Aggregation:** Pandas `groupby` and `crosstab` methods were used to aggregate data, which was then used as input to create visualizations.

## 📊 Key Findings & Insights

The project yielded several significant insights:

* **Biodiversity Balance:** Across all parks, plants dominate the landscape, accounting for 83% of all observations. Among animals, birds are the most frequently sighted (51%), followed by mammals (21%).

* **Protection Disparity:** Mammals (17.05%) and Birds (15.37%) have significantly higher protection rates compared to Plants (<2%).

* **Statistical Result:** A Chi-Square Test yielded a **p-value < 0.05**, confirming that the association between species category and protection status is statistically significant.

* **Most Observed:** The **Little Brown Bat** is a notable outlier—it is both highly observed across all parks and carries a protected conservation status.

* **Regional Leader:** Yellowstone National Park recorded the highest volume of sightings, totaling ~1.4 million observations.

> **Conclusion:** The data suggests that while plants make up the bulk of the National Park biomass, **animal species—specifically mammals and birds—require a disproportionate amount of conservation intervention**. The statistically significant disparity in protection rates confirms that conservation efforts are currently, and perhaps necessarily, focused on these high-risk animal categories.


## 🚀 How to Run the Project

1. Clone the repository:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git)

2. Ensure you have the observations.csv and species_info.csv files in the same directory as the notebook.

3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook Biodiversity-in-National-Parks-Project.ipynb


## Files in this Repository

* `observations.csv`: Data on species sightings at the four parks.

* `species_info.csv`: Taxonomic and conservation data for each species.

* `biodiversity_analysis.ipynb`: The full Python analysis and visualizations.

* `README.md`: Project summary and documentation.

