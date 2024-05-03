# PowerBI-Learning-Projects
Power BI dashboards that I have built during my learning process
# Case Study HR Analytics in Power BI
Firsly I create DimDate table using DAX. Then I im making sure that there are correct relationships connecting my fact and dimensions tables. Lastly using DAX I created measures that track Attrition Rate in % or track perfomance of invidual workers based on the ratings they got working in our company.
In this dashboard I dive into data about our workers in hypothetical company Atlas Labs. I made overview page with basic information about workers in our company. In the Demographics Page we look at demographic insights. Perfomance Tracker is page dedicated to track individual worker and his ratings. 
Attrition page is created for detailed look at Attrition Rate in our company. Overall this dashboard could be used to identify problems with workers leaving our company and the reasons for it.
# Report Design in Power BI
In this report I have been mainly focused on learning proper design techniques to enchance my report appearance. I created interactive storytelling report using bookmarks with buttons and charts that are only visible when we select the certain scenario (progressive disclosure). I also created customized theme and did a mobile layout with a bookmark navigator. 
# HealthCare Case Study 
For this case study, we will be working with a dataset that includes New York state-wide hospital discharge data for a year. Elective hip replacement surgery was the main reason for their hospital stay. The dataset is one single table with 30 columns Each row in the dataset represents a single inpatient stay, from their admission to discharge date. The health information in this dataset is not individually identifiable. This means the file does not contain personal health information.

In the first file - Case Study HealthCare.pbix I have built charts to generally find trends and correlations in data, therefore I could build a well designed dashboard. Of course I had to make advanced measures to really dig into insights that were hidden inside the data( Variance between Main Average LOS Days and invidual Average) - % Var Average LOS Days = 
VAR vAVG = [Average LOS Days]
VAR vAvgALL = CALCULATE([Average LOS Days],ALL())
RETURN
(vAVG-vAvgALL)/vAvgALL
for example this one up here. I also created new table - surgical_program_size_summary to summarize informations about hospitals and their personel using SUMMARIZECOLUMNS() functions.
### Insights after Case Study
After building this report I started process of making it look proffesional. I added company backgrounds, navigation buttons,changed colors of theme and charts, reshaped and resized charts, to make it look as appealing as it can be. Final product of my efforts is visible in the file - Case Study HealthCare Final Design.pbix 
In our quest to analyze efficiency in hospitals across New York State, we found the average cost per discharge for a hip replacement surgery was $21K, and that there was significant variability between hospital facilities. Our root cause analysis found that some attributes stood out over others to influence both cost and average LOS. Patients who had an extreme illness severity, and extreme or major mortality risk stood out as having the most significant impact on reduced efficiency. Also, hospitals located in New York City tended to have a higher cost and LOS overall, and lastly, that LOS was influenced by patient disposition to a skilled nursing home. These insights are very useful and will help HealthStat to inform improvement initiatives for their clients.
