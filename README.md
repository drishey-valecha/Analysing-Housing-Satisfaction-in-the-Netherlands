**Title**

The following is the title of the housing satisfaction project in the Netherlands: “Analysing Housing Satisfaction in the Netherlands 🇳🇱: Data-Driven Insights for Urban Policy and Development (CBS StatLine Dataset)”.

**Project Overview**

In this project, I have analysed **housing satisfaction in the Netherlands** using the open government data provided by **CBS (Centraal Bureau voor de Statistiek)**. This repository demonstrates my skills in data analysis, predictive modelling, and visualisation, with a focus on the factors that affect housing satisfaction among Dutch residents. By employing machine learning models like Logistic Regression, Random Forest, and XGBoost, I have identified key drivers of satisfaction, including dwelling characteristics, environment quality, and tenant vs. owner status. The project is a step towards understanding public opinion and providing actionable insights for urban housing improvements.

**Data Source**

- Dataset: CBS StatLine Housing Satisfaction
- API Link: CBS API Housing Satisfaction

**Dataset Overview**

1) Total records: 591,360 (housing satisfaction and environment satisfaction).
2) Records in this project with a focus on housing satisfaction: 295,680.
3) Features: 8
4) Target variable (SatisfactionWithCurrentDwelling_1):
  - **0** --> Unhappy residents.
  - **1** --> Happy residents.
5) Feature categories:
  - *Categorical Features*: OwnerTenant, DwellingCharacteristics, Margins, Regions, and Periods.
  - *Numerical Features*: ID, SatisfactionWithCurrentDwelling_1, and SatisfactionWithLivingEnvironment_2.
6) The dataset contains various attributes about housing satisfaction, such as:
  - *Satisfaction with House*: Evaluates how satisfied residents are with their dwelling.
  - *Satisfaction with Environment*: Assesses how satisfied they are with their neighbourhood, amenities, and overall living conditions.
  - *Dwelling Characteristics*: Includes property value, dwelling size, age, and whether it has outdoor space.
  - *Ownership Type: Whether the resident is a homeowner or a tenant.
7) Key observations:
  - Most people in the Netherlands report being highly satisfied with both their homes and environments.
  - However, a small portion of residents, especially tenants, report dissatisfaction.
  - Smaller dwellings, older constructions, and a lack of outdoor space are strongly correlated with dissatisfaction.

**Methodology**

1) **Data Collection & Preprocessing**
- *API Integration*: Used both **requests** and **cbsodata** Python packages to fetch live data from the CBS StatLine API.
- *Data Cleaning*: Cleaned and preprocessed the dataset, handled missing values, categorised features, and encoded variables.

2) **Modelling**
- *Logistic Regression*: To predict satisfaction levels based on various features.
- *Random Forest*: A powerful model to analyse feature importance.
- *XGBoost*: Tuned for accuracy to improve performance, particularly for classifying dissatisfied residents.

**Key Findings**

1) *Environment & Dwelling Satisfaction Correlation*: Residents who are satisfied with their environment are more likely to be satisfied with their dwelling.
2) *Tenant Dissatisfaction*: Tenants, particularly those renting from housing corporations, exhibit higher dissatisfaction levels.
3) *Building Quality*: Newer homes (built after 2001) tend to have higher satisfaction rates, with gardens and more space also contributing positively.
4) *Urban vs. Rural*: Residents in more densely populated areas like Amsterdam and North Holland report more dissatisfaction.

**Observations from the Model Results**

1) *Logistic Regression*:
- Accuracy: 85%
- Key Insights: Ownership type and environment satisfaction are strong predictors of dwelling satisfaction.

2) *Random Forest*:
- Accuracy: 87%
- Key Insights: The model is computationally intensive but highlights the importance of dwelling characteristics (e.g., number of rooms, age of the property).

3) *XGBoost*:
- Accuracy: 91%
- Key Insights: The tuned model outperforms others with faster prediction times and higher precision for detecting dissatisfied residents.

**Visualisations**

1) *Histograms*
2) *Box Plots*
3) *Pie Charts*

**Conclusion and Insights**

The XGBoost model reveals that smaller, older, and low-value dwellings, especially those without private outdoor space, are strongly associated with resident dissatisfaction. Furthermore, **dissatisfaction appears to have increased significantly in recent years**, peaking in 2024. This trend may reflect **growing concerns over housing quality, affordability, and density in Dutch urban areas**.

1) *Policy Recommendations*: Focus on improving the quality of public housing, particularly for tenants renting from housing corporations.
2) *Key Drivers of Satisfaction*: Dwelling characteristics such as having a garden, more space, and newer constructions are major factors. Satisfaction with the environment is the strongest positive predictor of overall satisfaction.
3) *Urbanisation Challenges*: Urban areas like Amsterdam show more dissatisfaction, possibly due to housing pressure and affordability concerns.

**Disclaimer**

- This project utilises the Dutch open government data provided by **CBS (Centraal Bureau voor de Statistiek)**.
- **I do not own the dataset**. It is being used purely for educational purposes to support my learning in the field of data science and analysis.
- I would like to acknowledge **CBS (Centraal Bureau voor de Statistiek)** for their willingness to make the data accessible and open to sharing for analysis.

**Link to License**

This dataset is licensed under the **CC BY 4.0 License**.
