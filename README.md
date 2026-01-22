# COVID-19 India Exploratory Data Analysis (EDA)

## Project Overview

This comprehensive Exploratory Data Analysis project investigates the COVID-19 pandemic's impact across India using the Our World in Data (OWID) dataset. The analysis encompasses temporal trends, state-wise distribution, vaccination coverage, mortality rates, and key patterns to understand the pandemic's progression throughout India.

The project demonstrates essential data analysis skills including data cleaning, statistical analysis, time-series analysis, data visualization, and insight extraction using popular Python libraries.

## Dataset Information

**Source**: Our World in Data (OWID) COVID-19 Dataset

**Dataset Details**:
- **Total Records**: Time-series data spanning the entire pandemic period in India
- **Key Variables**:
  - Total Cases: Cumulative confirmed COVID-19 cases
  - Daily New Cases: Daily new case counts
  - Total Deaths: Cumulative deaths due to COVID-19
  - Daily New Deaths: Daily mortality counts
  - People Vaccinated: Total population vaccinated (1st dose)
  - People Fully Vaccinated: Fully vaccinated population counts
  - Daily Vaccinations: Daily vaccination administration counts
  - Tests Conducted: Testing volume data
  - Case Fatality Rate (CFR): Mortality percentage of confirmed cases
  - Population Data: Demographics for per-capita calculations

**Data Time Period**: From initial outbreak through latest available data in OWID dataset

**Geographic Coverage**: India as a whole with state-level analysis capabilities

## Analysis Performed

### 1. Temporal Trends Analysis
- **Time-Series Visualization**: Plotting total cases, deaths, and vaccinations over time
- **Daily Case Trends**: Identifying peaks, valleys, and wave patterns
- **Trend Decomposition**: Separating trend, seasonality, and residual components
- **Moving Averages**: 7-day and 30-day rolling averages for smoothing noise

### 2. Case Progression Analysis
- **Growth Rate Analysis**: Computing daily percentage changes in cases
- **Acceleration/Deceleration Patterns**: Identifying phase shifts in pandemic trajectory
- **Peak Identification**: Locating first wave, second wave, and subsequent peaks
- **Case Doubling Time**: Calculating time required for cases to double

### 3. Mortality Analysis
- **Death Toll Trends**: Temporal patterns in mortality data
- **Case Fatality Rate (CFR)**: Calculating mortality percentage over time
- **Deaths vs Cases Correlation**: Understanding disease severity patterns
- **Age-adjusted Mortality**: Where available, analyzing by demographics

### 4. Vaccination Impact Analysis
- **Vaccination Coverage**: Percentage of population vaccinated over time
- **Vaccination Speed**: Daily vaccination administration trends
- **Vaccination Phases**: Identifying different vaccination campaign stages (Phase 1, 2, 3, etc.)
- **Vaccination vs Case Trends**: Analyzing correlation between vaccination and case trends
- **Fully Vaccinated Population**: Tracking completion of vaccination courses

### 5. Testing Analysis
- **Testing Volume Trends**: Daily test counts over time
- **Positivity Rate**: Cases as percentage of tests conducted
- **Testing Infrastructure**: Capacity and expansion timeline
- **Test-Case Correlation**: Understanding detection vs prevalence

### 6. Regional Analysis (If available)
- **State-wise Comparison**: Comparative analysis across states
- **Regional Disparities**: Identifying high-burden regions
- **Spatial Distribution**: Mapping case density and mortality patterns

### 7. Statistical Analysis
- **Descriptive Statistics**: Mean, median, standard deviation of key metrics
- **Correlation Analysis**: Relationships between variables
- **Distribution Analysis**: Normality tests and distribution fitting
- **Outlier Detection**: Identifying anomalous data points

## Key Findings

### Pandemic Waves
- **First Wave**: Initial outbreak with gradual rise followed by plateau
- **Second Wave**: Dramatic surge in cases with higher mortality rates
- **Subsequent Waves**: Omicron and other variants with different characteristics

### Testing & Detection
- Testing capacity increased significantly over time
- Positivity rates varied across different phases
- Testing played crucial role in case identification

### Vaccination Campaign
- Massive vaccination drive reached substantial population coverage
- Vaccination rollout improved case outcomes
- Different vaccine phases targeted different population segments

### Mortality Patterns
- Case fatality rates varied across different waves
- Mortality peaked during second wave
- Healthcare capacity constraints visible during peak periods

### Recovery & Trends
- Recovery rate improved over time with vaccination
- Healthcare interventions and protocols evolved
- Public health measures impact visible in trend inflections

## Technologies Used

**Programming Language**: Python 3.x

**Libraries**:
- **Pandas**: Data manipulation, cleaning, and aggregation
- **NumPy**: Numerical computations and statistical operations
- **Matplotlib**: Line plots, time-series visualizations, and basic charts
- **Seaborn**: Enhanced statistical visualizations and heatmaps
- **Plotly**: Interactive plots and dashboard-style visualizations (optional)
- **Scikit-learn**: Statistical analysis and data preprocessing
- **SciPy**: Advanced statistical testing and analysis

## Installation & Setup

### Prerequisites
- Python 3.7 or higher
- pip package manager
- Jupyter Notebook or JupyterLab

### Installation Steps

1. Clone this repository:
```bash
git clone https://github.com/souradeephowlader18-94/covid-india-EDA.git
cd covid-india-EDA
```

2. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install required packages:
```bash
pip install -r requirements.txt
```

### Required Packages
```
pandas>=1.3.0
numpy>=1.21.0
matplotlib>=3.4.0
seaborn>=0.11.0
plotly>=5.0.0
scipy>=1.7.0
scikit-learn>=0.24.0
```

## Usage

### Running the Analysis

1. Open Jupyter Notebook:
```bash
jupyter notebook COVID19_EDA.ipynb
```

2. Run all cells or execute step-by-step:
   - Cell-by-cell execution recommended for learning
   - Each section contains markdown explanations
   - Visualizations display inline in notebook

### Notebook Structure

1. **Data Loading**: Import COVID-19 India dataset from OWID
2. **Data Cleaning**: Handle missing values, data type conversions, date parsing
3. **Exploratory Analysis**: Initial data exploration and summary statistics
4. **Temporal Analysis**: Time-series plots and trend analysis
5. **Comparative Analysis**: Cases vs Deaths vs Vaccinations
6. **Statistical Tests**: Correlation, distribution, and hypothesis testing
7. **Advanced Visualizations**: Interactive plots and comprehensive dashboards
8. **Key Insights**: Summary of findings and conclusions

### Customization

- Modify date ranges for specific analysis periods
- Filter for particular states (if state-level data available)
- Adjust visualization parameters in Matplotlib/Seaborn settings
- Change smoothing window sizes for moving averages
- Modify statistical test parameters

## File Structure

```
covid-india-EDA/
├── COVID19_EDA.ipynb          # Main analysis notebook
├── Daily_Insights_Summary.md  # Daily insights and summary
├── README.md                  # This file
├── data/                      # Data folder (if included)
│   └── covid_india.csv        # COVID-19 India dataset
└── requirements.txt           # Python dependencies
```

## Key Metrics & Calculations

### Case Fatality Rate (CFR)
```
CFR = (Total Deaths / Total Cases) × 100
```

### Recovery Rate
```
Recovery Rate = (Total Recovered / Total Cases) × 100
```

### Active Cases
```
Active Cases = Total Cases - Total Deaths - Total Recovered
```

### Vaccination Coverage
```
Vaccination % = (People Vaccinated / Total Population) × 100
```

### Daily Growth Rate
```
Growth Rate = ((Cases Today - Cases Yesterday) / Cases Yesterday) × 100
```

## Future Work & Improvements

### Data Enhancement
- Incorporate state-level data for regional analysis
- Add demographic breakdowns (age, gender)
- Include healthcare capacity metrics (hospital beds, ICU availability)
- Integrate genomic sequencing data for variant analysis

### Advanced Analysis
- Time-series forecasting using ARIMA or Prophet models
- Machine learning models for trend prediction
- Clustering analysis for identifying similar phases
- Anomaly detection in mortality and case data
- Sentiment analysis of public response (Twitter, media)

### Visualization Enhancements
- Interactive dashboards using Plotly or Dash
- Geographic heatmaps showing regional distribution
- Animated visualizations showing progression over time
- Comparative state/district level interactive maps

### Comparative Analysis
- India's response vs global comparisons
- Inter-state comparison metrics
- Urban vs rural analysis
- Pre-vaccination vs post-vaccination comparison

## Insights & Conclusions

1. **Wave Patterns**: India experienced distinct waves with varying characteristics and impacts
2. **Testing Scaling**: Rapid expansion of testing infrastructure enabled better case detection
3. **Vaccination Success**: Large-scale vaccination campaign reached significant population coverage
4. **Healthcare Response**: System adapted with surge capacity during peak periods
5. **Mortality Patterns**: Death rates correlated with healthcare capacity and variant characteristics
6. **Recovery**: Declining case trends visible in recent periods with improved interventions

## References & Data Sources

1. **Our World in Data (OWID)**: https://covid.ourworldindata.org/
   - Free, open-source dataset on COVID-19 pandemic
   - Regularly updated with latest available data
   - High-quality, curated from official sources

2. **Ministry of Health & Family Welfare, India**: https://www.mohfw.gov.in/
   - Official government COVID-19 dashboard
   - Real-time case statistics and vaccination data

3. **Johns Hopkins University CSSE**: https://github.com/CSSEGISandData/COVID-19
   - COVID-19 data repository
   - Widely used for pandemic research

4. **Python Data Science Libraries**:
   - Pandas Documentation: https://pandas.pydata.org/
   - Matplotlib: https://matplotlib.org/
   - Seaborn: https://seaborn.pydata.org/
   - SciPy: https://scipy.org/

## Learning Objectives Achieved

✓ Data cleaning and preprocessing with real-world dataset
✓ Time-series analysis and trend identification
✓ Statistical analysis and hypothesis testing
✓ Data visualization techniques and best practices
✓ Exploratory data analysis workflow
✓ Insight extraction and meaningful interpretation
✓ Documentation and presentation skills
✓ Version control and reproducible research

## Author

**Souradeep Howlader**
- GitHub: https://github.com/souradeephowlader18-94
- Project: COVID-19 India Exploratory Data Analysis
- Last Updated: 2024

## License

This project is open source and available under the MIT License.

## Acknowledgments

- Our World in Data for providing comprehensive COVID-19 dataset
- Python open-source community for excellent data science tools
- All contributors and healthcare workers fighting COVID-19
- Data enthusiasts and analysts sharing insights and methodologies

---

**Disclaimer**: This analysis is for educational and informational purposes. COVID-19 is a complex public health issue. For medical or policy decisions, please consult official health authorities and expert sources.
