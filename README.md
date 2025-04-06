# Electric Vehicle Charging Station Optimization

## Project Overview

The goal of this project is to optimize the operation of electric vehicle (EV) charging stations by analyzing user behavior, enhancing infrastructure efficiency, and forecasting energy demand. The study covers two real charging sites near Burbank (CA), using data from 2018–2021.

We explore clustering of user sessions, define actionable KPIs, and build predictive models to support better decision-making and dynamic pricing strategies.

---

## Data Description

- **Charging Sessions Dataset** — 63,883 cleaned entries from two sites (private and public).
- **Weather Data** — merged from public sources for enhanced modeling.
- Features include connection times, kWh delivered, session durations, user inputs, and more.

---

## Key Steps

1. **Data Cleaning**: Removed duplicates, fixed inconsistent timestamps, unpacked JSON fields.
2. **Feature Engineering**: Created features for session duration, energy per hour, temporal patterns.
3. **Clustering**:
   - Used PCA to reduce dimensionality.
   - Evaluated K-Means and Agglomerative Clustering.
   - Identified 4 user groups:
     - *New Regular Consumers*
     - *First and Flexible*
     - *Charging Professionals*
     - *First Fast Public Users*
4. **Prediction Models**:
   - Compared a linear regression vs. a simple neural network.
   - Forecasted hourly energy demand with minimal performance difference between models.

---

## KPIs Proposed

- **Utilization Rate**
- **kWh Delivered per Hour**
- **Charging Time**
- **Parking Time**

Interactive visualizations and widgets were implemented to explore these KPIs over time and across locations.

---

## Conclusions

- **Best clustering** was achieved with 4 K-Means clusters.
- **Linear regression model** is preferred for prediction due to explainability and similar performance.
- **Utilization improvements** possible without infrastructure expansion.
- Recommending:
  - Dynamic pricing based on demand.
  - Incentives to reduce idle parking.
  - Monitoring behavioral shifts (e.g., remote work).
  - Differentiated strategies for public vs. private sites.

---

## Appendix

Includes visualizations of:
- Charging session patterns
- Site comparisons
- Cluster distributions
- Prediction model performance

---

*This project was completed as part of the Analytics and Applications M.Sc. course at the University of Cologne.*
