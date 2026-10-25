Exoplanet Data Analysis

Overview

This project explores exoplanet data using Python, focusing on understanding planetary characteristics through exploratory data analysis (EDA) and data visualization.

The analysis investigates patterns, distributions, and relationships among available planetary features to better understand the properties of known exoplanets.

Objectives

* Explore and understand the exoplanet dataset.
* Inspect data quality and identify missing values.
* Analyze the distributions of planetary characteristics.
* Visualize relationships between relevant numerical features.
* Identify patterns and observations that could motivate further scientific investigation.

Technologies Used

* Python
* Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* Seaborn

The list above should include only libraries actually used in the notebook.

Dataset

The project uses an exoplanet dataset containing planetary measurements and related characteristics.

Dataset source: https://exoplanetarchive.ipac.caltech.edu/index.html

The dataset is used for exploratory analysis and visualization.

Methodology

1. Load the dataset into Python.
2. Inspect its structure, data types, and summary statistics.
3. Examine missing values and data quality.
4. Perform exploratory data analysis.
5. Create visualizations to investigate distributions and feature relationships.
6. Summarize the observations and identify potential directions for further analysis.

Results and Observations

The exploratory analysis investigates the following aspects of exoplanet data:

* Planetary mass and radius: Compared the mass–radius distributions of planets in the NASA and PHL datasets using logarithmic scatter plots to examine their physical characteristics.
* Planetary distance and temperature: Examined the distribution of exoplanet distances and analyzed the surface-temperature distribution available in the PHL dataset.
* Potential habitability: Applied rule-based filters using surface temperature (240–320 K), radius (0.5–2.5 Earth radii), and mass (0.1–10 Earth masses) to identify planets meeting the selected criteria.
* Earth Similarity Index: Calculated a custom similarity score using planetary radius and surface temperature to identify planets whose measured properties are closer to Earth’s under the selected formula.
* Feature relationships: Used a correlation heatmap to investigate relationships between mass, radius, distance, surface temperature, and stellar flux in the PHL dataset.

Interpretation and Limitations

The habitability filters identify candidates that satisfy the project’s selected numerical criteria; they do not establish that these planets are habitable or support life.

The calculated Earth Similarity Index is a simplified, project-specific score based on radius and surface temperature, not a comprehensive assessment of planetary habitability.

Include screenshots or saved visualizations if they help communicate the results.

How to Run

1. Clone this repository.
2. Install the required dependencies.
3. Open the Jupyter Notebook.
4. Run the notebook cells in order.

Example commands:

git clone https://exoplanetarchive.ipac.caltech.edu/docs/API_PS_columns.html?utm_source=chatgpt.com
cd PSCompPars.csv
pip install pandas numpy matplotlib seaborn jupyter
jupyter notebook

Replace the example repository details with your actual repository URL and name. Adjust the dependencies to match your notebook.

Limitations

This project focuses on exploratory data analysis. The observations are descriptive and do not establish that an exoplanet is habitable or supports life.

Future Improvements

* Investigate additional planetary and stellar characteristics.
* Explore statistical relationships between features.
* Develop a reproducible data preprocessing pipeline.
* Evaluate suitable machine learning approaches in a future extension.

Author

Swathya Kurra

GitHub: https://github.com/swathyakurra2-ops
