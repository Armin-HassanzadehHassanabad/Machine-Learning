Heart Disease Data Analysis

This project explores the Kaggle Heart Disease dataset through thorough preprocessing, exploratory data analysis (EDA), outlier handling, imputation, and a supervised learning model using Random Forests.

Overview

The notebook includes:

    Data Summarization: Using summarytools, dtale, and klib for fast overview and correlation insight.

    EDA: Distribution plots and box plots to study feature behavior, skewness, and potential outliers.

    Outlier Detection & Treatment: IQR and Z-score-based filtering; outliers replaced with NaN and handled appropriately.

    Missing Data Imputation: Strategy includes conditional median/mode replacement and KNN imputation based on percentage of missingness.

    Data Cleaning: Removal of duplicates, consistent type casting, and imputation logic to retain sample integrity.

    Feature Engineering: Detection of categorical and continuous variables for downstream modeling.

    Modeling: Pipeline includes train-test split, feature scaling, and fitting a tuned RandomForestClassifier.

Techniques Used

    Visualization: matplotlib, seaborn, klib for EDA and multivariate exploration.

    Imputation: Conditional strategies + KNNImputer for high-missing features.

    Outlier Handling: Domain-aware thresholds using IQR/Z-score.

    Model: Random Forest with depth, split, and leaf control for regularization.


Performance

    The trained RandomForestClassifier achieves a test accuracy of:
      (pred1 == y_test).mean()  # Final evaluation score
      
Requirements
      
      pip install pandas numpy seaborn matplotlib sklearn dtale klib summarytools

Remarks

      This project emphasizes disciplined preprocessing and data integrity before applying any model. 
      Feature curation, cleaning, and proper handling of missing values contribute significantly to stable model generalization.
