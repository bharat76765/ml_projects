# Bengaluru House Price Prediction (BHPP)

## Overview
**Day 90 of My Data Science Journey: Lessons from My First Full-Scale ML Project**

Welcome to my first full-scale machine learning project, where I take on the challenge of predicting house prices in Bengaluru using a rich dataset with plenty of complexity. From data cleaning and feature engineering to running various machine learning models, this project encapsulates my learning experience, applying the skills I’ve accumulated over my journey in data science.

This project has been both exciting and challenging, especially when working with messy, real-world data. I leveraged regression techniques and ensemble models to predict housing prices, all while improving my problem-solving and machine learning skills.

## Project Summary
This project tackles the **Bengaluru House Price Dataset**, which contains features like area type, availability, location, size, society, total square footage, bath, balcony, and price. My focus was on:
1. Keeping as much data as possible without making arbitrary exclusions.
2. Feature engineering to optimize the performance of models.
3. Protecting the target variable (price) from data leakage.
4. Solving the problem using regression learning methods.

Through the course of this project, I experienced both successes and setbacks, which are detailed below. 

## The Dataset
The dataset included columns that were tricky to handle: 
- **area_type**
- **availability**
- **location**
- **size**
- **society**
- **total_sqft**
- **bath**
- **balcony**
- **price**

The real challenges came from the `location`, `availability`, `society`, and `total_sqft` columns, which had missing values and inconsistencies. I spent considerable time filling in missing values, creating new features where necessary, and striking a balance between keeping as much data as possible and avoiding biases.

## The Process
### 1. Data Exploration:
The first step was to deeply explore the data to understand relationships between features and ensure data integrity. This included:
- Initial statistical summaries and visualizations to detect outliers.
- Correlation analysis to check relationships between variables.

**Key learnings**:
- Avoid rejecting data purely based on boxplots—outliers could contain valuable information.
- Feature engineering plays a major role in improving model performance.

### 2. Data Preprocessing:
This step involved:
- Filling in missing values and addressing inconsistencies.
- Engineering new features like `price_per_sqft` to give the models more context.

### 3. Model Building & Evaluation:
After cleaning the data, I implemented several machine learning models to predict house prices:

- **Simple Null Value Removal**: 
  After cleaning the dataset by removing null values, the model achieved an R² score of **0.74**, which was a good starting point.

- **Outlier Removal**: 
  Surprisingly, removing outliers gave me a **negative R² score**! This was an unexpected twist that demonstrated how sensitive the dataset is to different methods.

- **Advanced Outlier Removal and Feature Engineering**: 
  After performing more detailed feature engineering, the model gave an R² score of **0.54**. The effort here highlighted the challenges in balancing bias and variance in a complex dataset.

### 4. Applying Different Algorithms:
I applied a variety of algorithms to experiment and learn:

- **Polynomial Regression**: 
  This gave me an R² score of **0.67**. While it captured some non-linear relationships, it wasn’t the perfect fit.

- **Random Forest with GridSearchCV**: 
  Using Random Forest and tuning the model with GridSearchCV gave an R² score of **0.69**. Though I hoped for a higher score, the model performed relatively well compared to other methods. Overfitting was observed, but this is something I'll address in future iterations.

## Key Takeaways:
1. **Data Wrangling**: The challenges posed by missing values, outliers, and inconsistent data taught me the importance of cleaning and preprocessing.
2. **Model Comparison**: Through applying multiple models (Linear Regression, Polynomial Regression, and Random Forest), I realized that sometimes even simple models outperform complex ones if the data isn't properly treated.
3. **Patience and Perseverance**: The project tested my patience but also reinforced the importance of systematic problem-solving.
4. **Feature Engineering**: The more effort you put into understanding and manipulating features, the better your models will perform.

## Challenges Faced
The dataset presented various challenges, especially with columns like `society`, `location`, and `total_sqft`. Handling these inconsistencies while trying to retain as much useful data as possible took a lot of time and careful planning. Missing data in categorical fields and the continuous target variable required special attention to ensure the models weren't biased.

## Conclusion
Completing this project was a major milestone for me. It was a thrilling and challenging journey that tested my machine learning skills and my ability to handle real-world data. Although the R² scores weren’t as high as I initially hoped, I’ve learned invaluable lessons about data exploration, feature engineering, model tuning, and handling overfitting.

This project not only provided a hands-on experience in tackling real-world problems, but it also helped solidify my understanding of regression learning methods and ensemble techniques like Random Forest.

## Next Steps
In future iterations, I plan to:
- Tune the models more rigorously using techniques like cross-validation.
- Apply advanced algorithms such as **XGBoost** or **LightGBM** to improve prediction performance.
- Explore deeper feature engineering strategies to better capture the complexities of the dataset.

## Getting Started
### Prerequisites
The following libraries are required to run the project:
- Python 3.8+
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

Install them using:
```
pip install pandas numpy scikit-learn matplotlib seaborn
```

### Running the Project
1. Load the dataset `Bengaluru_House_Data.csv`.
2. Perform data cleaning and preprocessing, including handling missing values and outliers.
3. Apply regression models like Linear Regression, Polynomial Regression, and Random Forest.
4. Evaluate the models using R² scores and residual analysis.

## Acknowledgements
Thanks to the Kaggle community for providing the dataset and to the numerous online resources, including **ChatGPT and Gemini**, that helped me along the way.

---

**#Day_90**  
**#MachineLearning**  
**#DataScienceJourney**  
**#BengaluruHousePrices**  
**#RegressionLearning**  
**#OutlierRemoval**  
**#RandomForest**  
**#FeatureEngineering**  
**#FresherJourney**
