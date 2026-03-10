# Energy Consumption Prediction Using Nonlinear Regression Models.


## 1. Dataset
Accurate prediction of building energy consumption is essential for improving energy efficiency, reducing operational costs, and supporting sustainable building management. Energy usage patterns are influenced by multiple factors including indoor temperature, humidity, weather conditions, and occupancy behavior. The dataset used in this study is the **Appliances Energy Prediction dataset introduced by Luis M. Candanedo et al. (2017)**, which contains 10-minute interval measurements of electricity consumption in a lowenergy house in Belgium, collected over approximately 4.5 months. Predictors include temperature and humidity from multiple rooms, weather data (outdoor temperature, wind speed, atmospheric pressure), and time-derived features (hour, day of week). Nonlinear regression approaches are necessary to capture these structured dependencies. </br></br>
**Target variable:** Appliances (energy consumed by appliances, in Wh, over 10 minutes)</br></br>
**Predictors:** Indoor and outdoor temperature, humidity, weather conditions, etc.</br></br>


## 2. Methods

### 2.1 Preprocessing choices
• **Missing values:** None detected.</br></br>
• **Outliers:** Shrinked using logarithm</br></br>
• **Feature scaling:** applied only for models sensitive to feature magnitude (Linear Regression, Polynomial Regression, SVR)</br></br>
• **Train/Test split:** 80/20</br></br>

### 2.2 Models selected
1. **Linear Regression.** Establishes lower bound performance. Assumes global linear
relationships.</br></br>
2. **Polynomial Regression.** Captures interaction and nonlinear relationships.</br></br>
3. **SVR.** Captures complex nonlinear relationships.</br></br>
4. **Gradient Boosting Regression.**</br></br>


## 3. References
• https://archive.ics.uci.edu/dataset/374/appliances+energy+prediction – Dataset.</br></br>
• https://scikit-learn.org/stable/api/index.html - guide for implementation of scikit functions.</br></br>
• https://seaborn.pydata.org/generated/seaborn.heatmap.html - creating a heatmap.</br></br>
