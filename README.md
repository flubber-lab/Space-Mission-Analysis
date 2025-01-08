# Space Missions Dataset Analysis

This repository contains an analysis of a dataset detailing various space missions, including their costs, durations, targets, and outcomes. The dataset provides insights into the success rates, fuel consumption, payload weights, and other key metrics of space missions.

## Dataset Overview

The dataset (`space_missions_dataset.csv`) contains the following columns:

- **Mission ID**: Unique identifier for each mission.
- **Mission Name**: Name of the mission.
- **Launch Date**: Date of the mission launch.
- **Target Type**: Type of target (e.g., Star, Exoplanet, Asteroid).
- **Target Name**: Name of the target (e.g., Mars, Titan, Betelgeuse).
- **Mission Type**: Type of mission (e.g., Colonization, Exploration, Mining).
- **Distance from Earth (light-years)**: Distance of the target from Earth.
- **Mission Duration (years)**: Duration of the mission.
- **Mission Cost (billion USD)**: Cost of the mission in billions of USD.
- **Scientific Yield (points)**: Scientific output of the mission.
- **Crew Size**: Number of crew members on the mission.
- **Mission Success (%)**: Success rate of the mission.
- **Fuel Consumption (tons)**: Fuel consumed during the mission.
- **Payload Weight (tons)**: Weight of the payload.
- **Launch Vehicle**: Vehicle used for the launch (e.g., SLS, Starship, Falcon Heavy).

## Analysis Performed

The following analyses were performed on the dataset:

1. **Descriptive Statistics**: Summary statistics for numerical and categorical columns.
2. **Trend Analysis**: Temporal trends in mission costs, durations, and success rates.
3. **Correlation Analysis**: Relationships between numerical variables (e.g., cost vs. scientific yield).
4. **Comparative Analysis**: Comparison of mission success rates by target and mission type.
5. **Cluster Analysis**: Grouping missions based on similar characteristics.
6. **Predictive Analysis**: Predicting mission success based on key features.
7. **Geospatial Analysis**: Analysis of missions based on distance from Earth.
8. **Cost-Benefit Analysis**: Calculating ROI for missions.
9. **Crew Size Analysis**: Relationship between crew size and mission success.
10. **Fuel and Payload Analysis**: Fuel efficiency and payload capacity.
11. **Target-Specific Analysis**: Popularity and difficulty of different targets.
12. **Mission Type Analysis**: Success rates and costs by mission type.
13. **Time Series Analysis**: Mission launch frequency over time.
14. **Anomaly Detection**: Identifying outliers in mission costs and success rates.
15. **Visualization**: Heatmaps, bar charts, line graphs, and pie charts.
16. **Hypothesis Testing**: Testing hypotheses about mission success factors.
17. **Network Analysis**: Relationships between missions and targets.
18. **Text Analysis**: Analyzing mission names and target names.
19. **Risk Analysis**: Identifying high-risk missions.
20. **Optimization Analysis**: Optimizing resource allocation for missions.

## Code

The analysis was performed using Python and the following libraries:

- **Pandas**: Data manipulation and analysis.
- **NumPy**: Numerical computations.
- **Matplotlib**: Basic plotting and visualization.
- **Seaborn**: Advanced statistical visualizations.
- **Scikit-learn**: Machine learning and predictive modeling.
- **NetworkX**: Network analysis.

### Example Code

```
python
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
```
# Load the dataset

`df = pd.read_csv('space_missions_dataset.csv')`

# Summary statistics
```
summary_stats = df.describe()
print(summary_stats)
```
# Correlation heatmap
```
numeric_columns = df.select_dtypes(include=['float64', 'int64']).columns
corr_matrix = df[numeric_columns].corr()
sns.heatmap(corr_matrix, annot=True, cmap='coolwarm')
plt.title('Correlation Matrix')
plt.show()
```
## Results

**Key findings from the analysis include:**

**Mission Cost Trends:** Mission costs have increased over time, with colonization missions being the most expensive.

**Success Rates:** Missions to closer targets (e.g., Mars) have higher success rates compared to distant targets (e.g., Betelgeuse).

**Fuel Efficiency:** Launch vehicles like Starship and Falcon Heavy demonstrate better fuel efficiency compared to SLS.

**ROI:** Mining missions tend to have the highest return on investment (ROI) in terms of scientific yield per cost.
