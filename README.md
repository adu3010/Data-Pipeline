# Data-Pipeline

# 🌐 Universal Data Pipeline

A modular and extensible **data pipeline framework** that covers the entire lifecycle of data preparation and analysis — from **ETL** (Extract, Transform, Load) to **Exploratory Data Analysis**, **Visualizations**, **Feature Engineering**, and generating a **Final Report**.

This project is designed to help **data analysts, scientists, and ML engineers** streamline workflows by providing a clean, reusable structure.

---

## 🚀 Features
- **ETL (Extract → Transform → Load)**  
  - `extract_data()`, `transform_data()`, `load_data()`

- **Exploratory Data Analysis (EDA)**  
  - `exploratory_analysis()`, `find_high_correlations()`

- **Visualization**  
  - `create_overview_dashboard()`  
  - `create_distribution_plots()`  
  - `create_correlation_heatmap()`  
  - `create_missing_values_plot()`  
  - `create_feature_importance_plot()`

- **Feature Engineering**  
  - `auto_detect_target()`  
  - `encode_categorical_features()`  
  - `scale_numerical_features()`  
  - `create_derived_features()`  
  - `remove_correlated_features()`  
  - `handle_outliers()`

- **Final Report**  
  - `generate_final_report()`

---

## 📊 Flowchart

Below is a high-level flow of the pipeline:

```mermaid
flowchart TD
    A[ETL] --> B[extract_data()]
    B --> C[transform_data()]
    C --> D[load_data()]
    D --> E[exploratory_analysis()]
    E --> F[find_high_correlations()]
    D --> G[create_visualizations()]
    G --> G1[overview]
    G --> G2[distribution]
    G --> G3[heatmap]
    G --> G4[missing values]
    G --> G5[feature importance]
    D --> H[feature_engineering()]
    H --> H1[auto_detect_target()]
    H1 --> H2[encode_categorical_features()]
    H2 --> H3[scale_numerical_features()]
    H3 --> H4[create_derived_features()]
    H4 --> H5[remove_correlated_features()]
    H5 --> H6[handle_outliers()]
    E --> Z[generate_final_report()]
    G --> Z
    H --> Z
    D --> Z
