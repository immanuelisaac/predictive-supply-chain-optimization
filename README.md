# Supply Chain Optimization & Delivery Risk Prediction

##  Project Overview
In modern e-commerce and global trade, timely delivery is a critical driver of customer retention and operational profitability. This project provides an end-to-end data science approach to diagnosing, analyzing, and predicting supply chain inefficiencies. 

By transitioning from descriptive diagnostic analytics to predictive machine learning, this pipeline empowers business stakeholders to proactively mitigate delivery delays, optimize profitability, and enhance customer satisfaction.

##  Tech Stack
* **Language:** Python
* **Data Manipulation:** `pandas`, `numpy`
* **Data Visualization:** `matplotlib`, `seaborn`
* **Machine Learning:** `scikit-learn` (Random Forest)
* **Imbalanced Data Handling:** `imbalanced-learn` (SMOTE)

##  Key Features & Pipeline Steps
1. **Data Preprocessing & Cleaning:** * Removal of redundant columns and Personally Identifiable Information (PII).
   * Filtering of anomalous orders (e.g., canceled shipping).
   * Standardized datetime conversion.
2. **Feature Engineering:**
   * Calculation of exact `Delay` metrics and `Is_Delayed` boolean flags.
   * Extraction of temporal granularities (`order_month`, `order_day`, `order_hour`).
   * Categorization of `Profitability_Flag` (Profitable, Loss, Breakeven).
3. **Exploratory Data Analysis (EDA):**
   * Dynamic calculation of overarching Business KPIs (Total Profit, Total Loss due to delays, 90th percentile delay).
   * Multi-panel visualization of temporal friction points.
   * Region-specific categorical driver analysis to pinpoint exact logistics bottlenecks.
4. **Predictive Modeling:**
   * Frequency encoding for high-cardinality categorical variables.
   * Implementation of **SMOTE** to generate synthetic data, solving the inherent class imbalance of supply chain datasets.
   * Training and evaluation of a **Random Forest Classifier** to accurately predict `Late_delivery_risk`.

##  Installation & Setup
1. Clone the repository:
   ```bash
   git clone [https://github.com/immanuelisaac/predictive-supply-chain-optimization.git](https://github.com/immanuelisaac/predictive-supply-chain-optimization.git)
   cd predictive-supply-chain-optimization
