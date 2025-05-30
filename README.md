# Data Analytics Portfolio
<a href="JCassner_Data_Analyst.docx" download>Resume</a>
## About Me
#### Detail-oriented and motivated data analyst with hands-on experience in data cleaning, exploration, and visualization using real-world datasets. Skilled in transforming raw data into actionable insights through clear visual storytelling and interactive dashboards. Proficient in SQL, Python, R, and business intelligence tools such as Tableau. Strong communicator with a track record of cross-functional collaboration and iterative problem-solving. Passionate about uncovering trends and patterns to support data-informed decision-making in dynamic, fast-paced environments.

## Education 👨🏻‍🎓
* M.S., Data Analytics - Franklin University (_May 2025_)
* B.S., Biology - Ohio Northern University (_May 2007_)

## Certifications 🏅
* **Machine Learning with Python** (_August 2024_)
  * Developed skills in basic data analytics methods, supervised and unsupervised machine learning algorithms, evaluating model performances, clustering methods, diagnostic and predictive analytics and natural language processing; Able to apply appropriate machine learning and data mining methods to solve real-world problems; Demonstrated knowledge and skills in using Python programming to support fact-based decision making
* **Data Visualization with Tableau** (_December 2024_)
  * Demonstrated data visualization skills through the completion of various projects utilizing Tableau; Able to connect, prepare, explore and analyze the data and build powerful visualizations and dashboards in Tableau; Developed skills to create effective data stories using Tableau features, and presentation skills to communicate their products to non-technical audiences
* **Data Mining with R** (_December 2024_)
  * Developed skills in exploratory data analysis and various data mining methods, including regression, classification, clustering, association rule mining, time series forecasting, and text mining; Able to apply appropriate data mining methods to solve scenario-based real-world business problems; Demonstrated knowledge and skills in using RStudio for data visualization and reporting to support fact-based decision-making


## Projects 🛠️
### Machine Learning
[SkyMart Data Cleaning & EDA](https://colab.research.google.com/drive/10U9YVvh9neSB3jiR-X5TOwu2pF_vyzG5#scrollTo=HFRqDX5rmwIY)

[SkyMart Sales Predictive Modeling](https://colab.research.google.com/drive/1Qr5fHEcdC1lomarmXOTromuZdZML6Cmk#scrollTo=ZzKAQtOGEDaZ)

<a href="SkyMart_Final_Report.docx" download>SkyMart Final Report</a>

Description: SkyMart is a leader in the United States retail business sector with over 45 stores nationwide and sought to uncover valuable insights from newly gathered data relating to their business performance. Their main goal was to develop a predictive model to best forecast future sales of their company while also pulling insights of individual store's sales performance, deciphering seasonal fluctuations to improve inventory preparedness, and determining if external factors have a major effect on overall sales. Key steps in delivering on SkyMart's requests involved an in-depth data wrangling & cleaning, exploratory data analysis (EDA), data modeling, and evaluation. 
* **Data Wrangling & Cleaning**: Datasets were procured through a Kaggle library and combined to facilitate target and feature inclusion. Datatypes were transformed into more usable types (e.g., date fields changed to datetime and parsed, binary fields encoded appropriately), feature engineering was performed to combine similar features, and null values were investigated and imputed.
* **EDA**: Univariate analysis of all features revealed skewed distributions of some, which were transformed via natural log and boxcox transformations to best prepare the data for linear regression implemntation. Bivariate analysis of relationships between predictor features and the target was then performed and resulted in the knowledge that their relationship was not strongly linear. Potential use of non-linear models was noted due to that finding. Store performances were determined by analyzing store sales figures over time to pinpoint high- and low-performing stores. Seasonality was determined by decomposing sales figures over time and revealing late-year spikes and early-year lulls.
* **Data Modeling**: The dataset was split into 70% training and 30% testing sets and both were standardized to account for different measurement scales. Each model investigated was evaluated on its coefficient of determination (R2 value), root mean squared error (RMSE), and plotting residuals. A multiple linear regression  including all predictor features was first performed and yielded very subpar results, confirming the lack of linearity of the data. Pivoting to non-linear models, a polynomial regression was then conducted which yielded slightly better metrics (R2: 0.385; RMSE: $442,143) but far from preferred outcomes. More complex non-linear models were needed and so decision tree, random forest, and XGBoost were then investigated. Each of these three models were tuned to their best hyperparameters, their least valuable features were recursively eliminated, and then each tuned model was fitted onto their preferred features.
* **Evaluation**: Based on the metrics of R2 value, RMSE, and plotting residuals with the consideration given to computing time, it was determined that XGBoost was the best model to recommend for future use with this dataset. Its R2 value was 0.975, its RMSE was $88,829, its residual plot was the least variable, and it did not overly tax the computing system. Future work was also determined and communicated back to SkyMart.

---

### Tableau Visualization
[Undergraduate School Selection Tool](https://public.tableau.com/app/profile/justin.cassner/viz/UndergraduateSchoolSelectionTool/Dashboard1)

Description: Deciding on a undergraduate school to attend is a very common pain point for graduationg high school seniors. I sought to develop a streamlined dashboard to assist those seeking higher education in answering pertinent questions they have. I utilized data from the U.S. Department of Education's National Center for Education Statistics (NCES) to accomplish this. Topics explored included the cost impact of staying in the state of residence or going out of state, the size of the typical freshman class as it can directly affect the student, and which placement test was most commonly submitted so the student can begin preparation for that. Visualizations range from comparable lists, bar graphs, and proportional symbol mapping and all are capbable of user refinement to assist in honing down their choices. 

---

### R Modeling
[Effect of COVID-19 Lockdown on Common Well-Being Search Terms](https://github.com/user-attachments/files/18431560/COVID-19.Lockdown.Effect.on.Search.Terms.docx)

Description: I investigated time series data on common well-being search terms, such as boredom, divorce, sadness, and stress, and their relation to the timing of the United States COVID-19 lockdown. Time series plots were first created in R spanning two different years over 3 states to visualize the layout of the data. A regression model was then able to be utilized by using the fixed effects ordinary least squares technique on the panel data. Lastly, running a clustering analysis on each search term by day reveals any significance of their changes between the two years after the lockdown timing. 
