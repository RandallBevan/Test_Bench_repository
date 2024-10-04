# Chess Prediction Using Machine Learning

# Proposal

## Intro + Background

Lately, there has been a lot of attention on forecasting the results of chess matches with the growing popularity of machine learning methods. Past studies, such as Aluna Riz’s research with LightGBM, have demonstrated how gradient boosting algorithms can effectively predict chess outcomes by analyzing player data and game-related characteristics [1]. This research furthers our knowledge that factors like player ratings, game length, and opening moves influence winning outcomes. 

In this project's dataset, obtained from [Kaggle](https://www.kaggle.com/datasets/datasnaek/chess), there are over 20,000 chess game records that include details such as player ratings, game outcomes, and time controls for each game played. The varied information available allows for an examination of gameplay dynamics and the meaning of ratings, furthering insight into the prediction of success or failure in competitive chess [2].

## Problem Definition

**Problem:** Finding the factors that most significantly impact the outcome of chess games, such as player experience/ranking, game duration, or opening strategies, and creating a model to predict game results.

**Motivation:** Through identifying the determinants of success and creating predictive models, chess enthusiasts, players, and coaches can benefit by analyzing game trends and utilizing prediction for strategic planning or personalized training.


## Methods

### Preprocessing
- **Data Cleaning:** Handle missing data, remove duplicates, and correct errors.
- **Outlier Handling & Feature Engineering:** Create interaction features, binning, and sample subsections of the dataset.
- **Data Transformation:** Normalize and apply log transformations if large values dominate.

### Machine Learning Methods
- **Random Forest:** Reason: group of decision trees, which makes it highly effective at handling complex, non-linear relationships in the data. It is also robust to overfitting because of its averaging nature, which makes it a strong candidate for chess prediction, where numerous features (e.g., moves, positions, strategies) interact in complex ways. It can handle categorical and numerical data well and often performs well without extensive parameter tuning.
- **Neural Networks:** Reason: Neural Networks, particularly deep learning models, are capable of learning highly complex patterns and making decisions based on features that might not be explicitly coded (e.g., intricate chess strategies). They are especially useful when provided with large datasets, which is common in chess with thousands of game records. NN models can handle non-linear and high-dimensional data effectively, making them suitable for a complex game like chess. [3]
- **Support Vector Machines (SVM):** SVMs are effective in high-dimensional spaces and are particularly useful when the decision boundary between classes (e.g., win, loss, draw) is complex. With the right kernel, SVMs can capture non-linear relationships in the data, which is essential for chess predictions. They also work well with smaller datasets compared to neural networks. [4]

## (Potential) Results + Discussion

In this project, we'll use accuracy, F1 score, and ROC-AUC to evaluate model performance. Accuracy provides a quick snapshot of overall correctness, F1 score balances precision and recall to handle imbalanced data, and ROC-AUC measures the model's ability to distinguish between outcomes. Our goals are to achieve high predictive accuracy while minimizing bias, ensuring fairness across player ratings and game outcomes. Ethical considerations include avoiding overfitting to specific player pools and ensuring data privacy. We expect Random Forest to perform well due to its robustness, while Neural Networks might excel with larger datasets. Overall, we anticipate discovering insights into the impact of openings and player ratings on game outcomes, contributing to more strategic chess analysis.

## References
[1] P. Aluna Rizzoli, “Predicting chess games results using lightgbm,” *Medium*, 16-Oct-2023. [Online]. Available: https://medium.com/@alunariz/predicting-chess-games-results-using-lightgbm-818f30b5a7c3. [Accessed: 02-Oct-2024].

[2] "Chess Game Dataset," Kaggle, [Online]. Available: https://www.kaggle.com/datasets/datasnaek/chess. [Accessed: 02-Oct-2024].

[3]V. Kumar, D. Singh, G. Bhardwaj and A. Bhatia, "Application of Neurological Networks in an AI for Chess Game," 2020 Research, Innovation, Knowledge Management and Technology Application for Business Sustainability (INBUSH), Greater Noida, India, 2020, pp. 125-130, doi: 10.1109/INBUSH46973.2020.9392188. keywords: {Technological innovation;Modulation;Games;Programming;Pattern recognition;Task analysis;Sustainable development;Neurological network;Reinforcement learning;Supervised;Unsupervised},

[4]N. L. T. Tra, P. T. Cong and N. D. Anh, "Design A Chess Movement Algorithm and Detect the Movement by Images Classification Using Support Vector Machine Classifier," 2018 4th International Conference on Green Technology and Sustainable Development (GTSD), Ho Chi Minh City, Vietnam, 2018, pp. 335-340, doi: 10.1109/GTSD.2018.8595604. keywords: {Robot kinematics;Support vector machines;Classification algorithms;Image processing;Artificial intelligence;Cameras;Chess program;Image processing;MATLAB;support vector machine},



## Contribution Table

| **Task Title**                    | **Task Owner**         |
|------------------------------------|------------------------|
| Project Team Composition           | All                    |
| Project Proposal                   | Fields Below           |
| Introduction & Background          | Randall                |
| Problem Definition                 | Randall                |
| Potential Dataset                  | Anay & Drew            |
| Methods                            | Anay & Drew            |
| Potential Results & Discussion     | Apollo & Nithil        |
| Gantt Chart                        | Drew                   |
| Video Recording                    | All                    |
| GitHub Page                        | Randall                |


## Gant Chart
https://gtvault-my.sharepoint.com/:x:/g/personal/ddagostino7_gatech_edu/EefHZ7und7ZEiZlgqVpmOr0B9ThaqGV_kqyBa7Izyc2oeg?e=4CRS5a
