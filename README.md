### Project Title
Hotel Booking Analysis and Forecasting using ML / AI

**Author**
Yu-Shen (Ethan) Tsao

#### Executive summary
This capstone project explores the use of machine learning to predict hotel booking cancellations, a critical business challenge that directly impacts revenue management, resource planning, and customer satisfaction. Using the Hotel Booking Demand dataset from Kaggle (~120,000 records), we developed and compared predictive models to determine whether a customer is likely to cancel their reservation prior to check-in.

After a thorough data cleaning and exploration phase, we applied two supervised learning algorithms: Logistic Regression and K-Nearest Neighbors (KNN). The models were evaluated based on accuracy, precision, recall, F1-score, and their ability to handle class imbalance.

While KNN achieved a higher overall accuracy (90.9%), it underperformed in identifying actual cancellations, with a recall of just 33% for the cancellation class. In contrast, Logistic Regression offered a more balanced and business-relevant outcome, correctly identifying 69% of actual cancellations and achieving a precision of 81%. This makes it a stronger candidate for production use in hotel operations.

Key predictors of cancellation included lead time, previous cancellations, deposit type, and booking channel. These insights not only enhance prediction accuracy but also offer valuable guidance for targeted marketing and overbooking strategies.

In conclusion, this project demonstrates that Logistic Regression is the more effective and actionable model for cancellation prediction in this context. Future work may include applying ensemble methods, addressing class imbalance with resampling techniques, and integrating the model into real-time booking systems to support operational decision-making.

#### Rationale
Why should anyone care about this question?
In the hospitality sector, booking cancellations present a significant challenge to operational efficiency and revenue optimization. The ability to accurately predict cancellations prior to guest check-in offers substantial strategic value to hotel management.
From a revenue management perspective, forecasting potential cancellations enables the implementation of dynamic overbooking strategies, minimizing the financial impact of unoccupied rooms. Operationally, it supports more accurate staffing, inventory planning, and resource allocation—ensuring that services are aligned with actual guest volume rather than inflated reservation numbers.

Moreover, early identification of high-risk bookings allows for proactive engagement with customers through targeted communications or retention incentives. This not only helps recover potential lost revenue but also enhances the overall guest experience.
By incorporating predictive analytics into booking workflows, hotel management can drive greater efficiency, mitigate risk, and make more informed decisions that directly support business goals and profitability.

#### Research Question
What are you trying to answer?
To what extent can we predict hotel booking cancellations prior to check-in using historical booking data, and what are the key factors that influence cancellation behavior?

Accurately predicting booking cancellations can help prevent revenue loss and improve operational efficiency for hotel businesses. My project goal is to evaluates two widely used machine learning models—Logistic Regression and K-Nearest Neighbors (KNN)—to determine which model provides more reliable predictions based on the available data.

#### Data Sources
What data will you use to answer you question?
Hotel booking demand(Kaggle)
https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand?resource=download&select=hotel_bookings.csv

This dataset provides booking information for both a city and a resort hotel. You'll find details such as when the booking was made, the duration of the stay, the number of guests (adults, children, or babies), and available parking spaces, among other relevant data. All personally identifying information has been removed.


#### Methodology
What methods are you using to answer the question?
1.	Obtain source data from Kaggle
2.	Analyze missing values in the columns, by replacing NaN value or dropping columns
3.	Drop and only keep relevant columns for the analysis
4.	Reduce cardinalities to reduce overfitting
5.	Covert categorial attributes to numeric values 
6.	Build Logistic Regression Model (LR)
7.	LR: Split data into Features and Targets
8.	LR: Split data into training (80%) and testing (20%)
9.	LR: Train Model
10.	LR: Predict and evaluate results
11.	Repeat the same process to build K-Nearest Neighbors (KNN)
12.	KNN: Split data into Features and Targets
13.	KNN: Split data into training (80%) and testing (20%)
14.	KNN: Train KNN Classifier
15.	KNN: Predict and evaluate results
16.	Evaluate and compare the results of Logistic Regression vs K-Nearest Neighbors models


#### Results
What did your research find?
In this project, both Logistic Regression and K-Nearest Neighbors (KNN) were evaluated to predict hotel booking cancellations using historical booking data.

KNN achieved a higher overall accuracy (90.9%) compared to Logistic Regression (82.4%). However, this accuracy is misleading due to class imbalance—most bookings are not canceled, which skews the performance of KNN.

Logistic Regression significantly outperformed KNN in identifying actual cancellations, achieving a precision of 0.81 and recall of 0.69 for the cancellation class, versus KNN’s much lower precision and recall of 0.33. The F1-score for cancellations was 0.74 for Logistic Regression, indicating a better balance between false positives and false negatives, compared to KNN’s 0.33.

From a business perspective, correctly identifying cancellations is critical to avoid lost revenue and optimize room management. Therefore, despite its lower overall accuracy, Logistic Regression is the preferred model due to its stronger performance on the minority (cancellation) class, better interpretability, and robustness to imbalanced data.

For model result comparison, please refer to document attached (Capstone Project ML Model Comparison)

#### Next steps
What suggestions do you have for next steps?
What suggestions do you have for next steps?
The logistic regression model has given a strong baseline, especially in interpretability. However, its linear nature may limit performance on more complex relationships. To improve recall for cancellations while maintaining overall performance, trying advanced models is a logical next step.
Model Options:
1.	Random Forest Classifier
2.	Gradient Boosting Classifier (from scikit-learn)

#### Outline of project

- [Link to notebook 1]()
- [Link to notebook 2]()
- [Link to notebook 3]()


##### Contact and Further Information
