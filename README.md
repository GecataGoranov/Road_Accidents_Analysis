# **Most Dangerous Road Accidents**

A machine‑learning project analyzing factors contributing to the severity of road accidents in Great Britain. Through exploratory data analysis and five classifiers (Logistic Regression, Decision Trees, Random Forests, XGBoost, and CatBoost), this repository uncovers and ranks the most dangerous conditions leading to fatal, serious, or slight collisions.

## **Project Overview**

By leveraging five years of **STATS19** data, this project trains five classification models to predict accident severity (1 = Fatal, 2 = Serious, 3 = Slight) and identifies the most dangerous contributing factors.

## **Features**
- **Data Preparation**
  - Merge Accident, Vehicle, and Casualty tables.
  - Handle missing values and drop low-utility columns
  - Encode categorical features via scikit-learn pipelines
- **Exploratory Data Analysis (EDA)**
  - Distribution plots for severity classes.
  - Correlation heatmaps for numerical features.
  - Bar charts for categorical variables (weather, lighting, junction type).
- **Modeling and Evaluation**
  - Train and tune Logistic Regression, Decision Tree, Random Forest, XGBoost, CatBoost.
  - Evaluate via classification reports (precision, recall, F1).
  - Visualize confusion matrices and feature‑importance rankings.
 
  ## **Reproduction**

  In order to reproduce the results, you would first have to download the data [from this Google Drive folder](https://drive.google.com/drive/folders/1AY198qa8gk8iW87a_dNRdUgLBMoL2UQi?usp=drive_link) and place both folders separately in the root directory of the project.

  Experiments for every model are kept in separate notebooks in the `notebooks` directory

  ## **Conclusion**

  In the end, based on our findings, we can make the following conclusions:
1. Most of the accidents are not fatal and don't lead to injuries.
2. Bad weather conditions actually decrease the chances of an accident to be fatal
3. Most accidents happen in populated places
4. The worse the lighting, the worse the accident
5. People with stronger cars tend to drive them more dangerously
6. Young people tend to drive more dangerously
7. The most dangerous roads are the ones outside of populated places, excluding the motorways
8. Older people tend to be more likely to have a fatal outcode, when involved in an accident
9. Collisions, involving trucks are more dangerous
10. Turning on a fast road and overtaking are the most dangerous maneuvers

## **References**
1. Department for Transport. (n.d.). Road Safety Data: Accidents, Vehicles and Casualties. [Dataset]. UK Government. Retrieved from https://www.data.gov.uk/dataset/cb7ae6f0-4be6-4935-9277-47e5ce24a11f/road-safety-data
2.  Department for Transport. (2023). Reported road casualties in Great Britain: Annual report 2023. Retrieved from https://www.gov.uk/government/statistics/reported-road-casualties-great-britain-annual-report-2023
3.  Prokhorenkova, L., Gusev, G., Vorobev, A., Dorogush, A. V., & Gulin, A. (2018). CatBoost: unbiased boosting with categorical features. Advances in Neural Information Processing Systems, 31. Retrieved from https://arxiv.org/abs/1706.09516
4.  Chen, T., & Guestrin, C. (2016). XGBoost: A scalable tree boosting system. Proceedings of the 22nd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining, 785-794. Retrieved from https://doi.org/10.1145/2939672.2939785
