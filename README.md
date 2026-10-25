Exoplanet Data Analysis

Exploratory data analysis (EDA) of exoplanet properties using Python, Pandas and Matplotlib/Seaborn.

Overview
This project cleans and combines two public exoplanet catalogs and explores how planet mass, radius, distance and temperature are distributed and related. It is descriptive analysis only; it does not use machine learning.

Data sources
- NASA Exoplanet Archive (Planetary Systems Composite Parameters): https://exoplanetarchive.ipac.caltech.edu/ (file: PSCompPars.csv)
- Planetary Habitability Laboratory, Habitable Worlds Catalog: https://phl.upr.edu/hwc/data (file: HWC_exoplanet.csv)

What I did
- Loaded both datasets, renamed and standardised selected columns, and handled missing values in the planetary measurements
- Compared planet mass and radius on logarithmic scatter plots for both catalogs
- Examined the distribution of exoplanet distances and surface temperatures
- Generated descriptive statistics and a correlation heatmap (mass, radius, distance, surface temperature, stellar flux)
- Applied rule-based filters (surface temperature 240-320 K, radius 0.5-2.5 Earth radii, mass 0.1-10 Earth masses) to identify candidates
- Calculated a simplified Earth-similarity score using only planet radius and surface temperature
- Merged records that appear in both datasets

Limitations
- The filters show which planets meet my chosen numerical criteria. They do not show that any planet is habitable or supports life.
- The similarity score uses only two properties, so it is much simpler than published Earth-similarity indices.
- Some surface temperatures in the PHL catalog are estimates from models, not direct measurements.

How to run
1. Clone the repository:
   git clone https://github.com/swathyakurra2-ops/exoplanet-habitability-analysis.git
2. Go into the folder:
   cd exoplanet-habitability-analysis
3. Install the libraries:
   pip install pandas numpy matplotlib seaborn jupyter
4. Start Jupyter and open exoplanets.ipynb:
   jupyter notebook
5. Run the cells in order.

Possible future work
- Add more planetary and stellar properties
- Test how sensitive the results are to the filter thresholds
- Build a reproducible cleaning pipeline

Author
Swathya Kurra - https://github.com/swathyakurra2-ops
