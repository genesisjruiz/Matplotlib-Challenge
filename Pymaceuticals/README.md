Module 5 Challenge: Data Visualization

In this assignment, I delved into real-world data visualization using Matplotlib. My responsibilities encompassed data analysis, creating visualizations, and summarizing the findings to evaluate the performance of Capomulin and other drug regimens in treating SCC.

GitHub:

Background

You've just joined Pymaceuticals, Inc., a new pharmaceutical company that specializes in anti-cancer medications. Recently, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.
As a senior data analyst at the company, you've been given access to the complete data from their most recent animal study. In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.
The executive team has tasked you with generating all of the tables and figures needed for the technical report of the clinical study. They have also asked you for a top-level summary of the study results.

Analysis Summary:

I began by combining and cleaning the mouse data and study results, removing one duplicate mouse and narrowing the study to 248 mice. The initial exploration involved generating two pie charts, one using Pandas and the other using pyplot, to visualize the distribution of female versus male mice. The results showed that male mice accounted for 51%, while female mice accounted for 49% of the study population.
Subsequently, I computed a summary statistics table that included the mean, median, variance, standard deviation, and standard error of the mean (SEM) of tumor volume for each treatment regimen. This analysis revealed that Capomulin and Ramicane had the smallest SEM, indicating a more precise estimate of the true mean tumor volume for these drug regimens.
Further exploration involved generating a bar plot displaying the total number of observed mouse time points associated with each drug regimen. The plot indicated that Capomulin and Ramicane had the most observed mouse time points. This larger dataset likely contributed to the smaller SEM, as a larger sample size leads to a more accurate estimation of the population mean.
I then created a dataframe, final_tumor_volumes, containing the last recorded tumor volume for each mouse under the selected treatment regimens. A subsequent box plot illustrated the distribution of tumor volume for each treatment group. Notably, Capomulin and Ramicane exhibited the smallest recorded tumor volumes at the final stage of treatment, with no outliers identified. Comparing the two regimens, Capomulin had a higher median tumor volume than Ramicane.
A line plot was generated to visualize the progression of tumor volume over time for a single mouse treated with Capomulin. The plot depicted a decreasing trend in tumor volume over time, suggesting a positive response to the treatment.
Lastly, a scatter plot was created to analyze the relationship between the average weight of mice under the Capomulin regimen and the corresponding average observed tumor volume. The correlation coefficient of 0.84 indicated a strong positive correlation between mouse weight and average tumor volume, providing valuable insights into their relationship within the context of the Capomulin regimen. However, it's essential to note that correlation does not imply causation, necessitating further analysis to establish causal relationships.


