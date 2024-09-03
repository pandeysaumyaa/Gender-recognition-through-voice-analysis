# Gender-recognition-through-voice-analysis

This project focuses on the development of a machine learning model for gender recognition based on voice samples. The process involves data extraction, transformation, and loading (ETL), followed by the application of several machine learning algorithms to determine the most accurate model for gender classification.

Project Overview

1. Data Preprocessing and ETL
The dataset consists of voice samples with various acoustic features. The initial step involves an ETL process:
- **Extraction**: Raw voice data is extracted from multiple sources.
- **Transformation**: The data is preprocessed to calculate key acoustic features, including mean frequency, median, skewness, kurtosis, and other relevant metrics.
- **Loading**: The transformed data is loaded into a structured format for analysis.

2. Feature Extraction
The following features were extracted and used for model training:
- Mean Frequency (meanfreq)
- Standard Deviation (sd)
- Median
- Q25, Q75 (quartiles)
- Interquartile Range (IQR)
- Skewness, Kurtosis
- Spectral Entropy (sp.ent), Spectral Flatness (sfm)
- Mode, Centroid
- Fundamental frequency (meanfun, minfun, maxfun)
- Dominant Frequency (meandom, mindom, maxdom)
- DfRange, Modulation Index (modindx)

 3. Machine Learning Models
Three machine learning algorithms were implemented and evaluated:
- **Random Forest**: A robust ensemble method that creates a 'forest' of decision trees.
- **Decision Tree**: A simple, interpretable model that splits the data based on feature values.
- **Naive Bayes**: A probabilistic classifier based on Bayes' theorem, assuming feature independence.

 4. Model Evaluation
The performance of each model was evaluated based on accuracy metrics. The Random Forest model achieved the highest accuracy among the three, making it the most effective for gender recognition in this dataset.

 Results
- Random Forest: Achieved the highest accuracy (mention the specific percentage if available).
- Decision Tree: Provided moderate accuracy, but was less effective than the Random Forest.
- Naive Bayes: Although fast and simple, it had the lowest accuracy compared to the other models.

Conclusion
The project demonstrates the effectiveness of the Random Forest algorithm in gender recognition based on voice features. The ETL process was crucial in preparing the data for analysis, ensuring that the models were trained on well-processed and relevant features.

 Dataset
The dataset used in this project can be obtained from [source link]. Ensure proper preprocessing before applying the machine learning models.

 Future Work
- Improve feature engineering to capture more nuanced aspects of voice data.
- Explore deep learning models for potentially better performance.
- Extend the project to include real-time gender recognition.

