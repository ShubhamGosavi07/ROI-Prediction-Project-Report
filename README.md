# ROI-Prediction-Project-Report

#### **Project Title**:  
**ROI Prediction in Social Media Advertising Campaigns**

---

#### **Introduction**:  
This project explores the application of data analytics and machine learning techniques to predict the Return on Investment (ROI) for social media advertising campaigns. By analyzing campaign data, such as conversion rates, acquisition costs, and engagement scores, we uncover insights to improve marketing strategies and optimize advertising efforts. The project also provides a framework for businesses to make data-driven decisions to maximize ROI.

---

#### **Dataset Description**:
The dataset consists of 300,000 records detailing advertising campaigns on various platforms. Key features include:
- **Campaign Information**: Campaign ID, Target Audience, Campaign Goal, Duration, Channel Used.
- **Performance Metrics**: Conversion Rate, Acquisition Cost, ROI (target variable).
- **Engagement Details**: Clicks, Impressions, Engagement Score.
- **Other Attributes**: Location, Language, Customer Segment, Company.

---

#### **Preprocessing Steps**:
1. **Cleaning**: Removed special characters (e.g., dollar signs) and converted columns like `Acquisition_Cost` to numeric values.
2. **Encoding**: Transformed categorical features (e.g., `Campaign_Goal`) into numeric formats for machine learning models.
3. **Normalization**: Scaled numerical features like `Clicks` and `Impressions` to ensure consistency.

---

#### **Exploratory Data Analysis (EDA)**:
- Analyzed ROI distributions across channels and campaign goals.
- Identified trends in conversion rates over time.
- Generated visualizations, including line plots, bar charts, and heatmaps, to illustrate key insights.

---

#### **Predictive Models**:
Three machine learning models were implemented to predict ROI:
1. **Random Forest Regressor**:
   - An ensemble learning method suitable for non-linear relationships.
   - Achieved the best performance among the models with an RMSE of 2.0.

2. **LSTM (Long Short-Term Memory)**:
   - Captured sequential dependencies in time-series data.
   - Suitable for campaigns with temporal patterns.

3. **Linear Regression**:
   - A baseline regression model assuming linear relationships.
   - Provided interpretable results but with higher error compared to other models.

---

#### **Evaluation Metrics**:
The models were evaluated using the following metrics:
- **Root Mean Squared Error (RMSE)**: Average magnitude of prediction errors.
- **Mean Absolute Error (MAE)**: Average absolute differences between predictions and actual values.
- **R² (Coefficient of Determination)**: Proportion of variance explained by the model.

| Model              | RMSE | MAE | R² Score |
|--------------------|------|-----|----------|
| Random Forest      | 2.00 | 1.59 | 0.33     |
| LSTM               | 2.10 | 1.45 | N/A      |
| Linear Regression  | 2.17 | 1.82 | 0.22     |

---

#### **Software and Tools**:
- **PySpark**: Large-scale data processing and machine learning.
- **Pandas, NumPy**: Data manipulation and preprocessing.
- **Seaborn, Matplotlib**: Visualization.
- **TensorFlow/Keras**: LSTM implementation.

---

#### **Conclusions and Recommendations**:
1. **Key Insights**:
   - Campaign goals and channels significantly impact ROI.
   - Targeting strategies need to be cost-effective for better ROI.

2. **Recommendations**:
   - Focus on high-performing channels like Pinterest and Instagram.
   - Use Random Forest for ROI prediction due to its robustness.
   - Explore deeper sequential patterns to enhance LSTM performance.

---

#### **References**:
Refer to the project report for detailed references, including libraries, methodologies, and dataset descriptions.

---

This README provides an overview of the project, its objectives, methods, and results. For detailed visualizations, analysis, and technical details, refer to the [project report](sandbox:/mnt/data/ROI_Prediction_Project_Report.pdf).
