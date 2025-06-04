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

#### Data Sources
What data will you use to answer you question?

#### Methodology
What methods are you using to answer the question?

#### Results
What did your research find?

#### Next steps
What suggestions do you have for next steps?

#### Outline of project

- [Link to notebook 1]()
- [Link to notebook 2]()
- [Link to notebook 3]()


##### Contact and Further Information
