# MIST-4610-Group-8-Project-2
MIST4610.21482 Group - 8

# Team Members:
1. [Matteo Garza](https://github.com/matteo101man)
2. [Andrew Haynes](https://github.com/AH171717)
3. [Collin Ladina](https://github.com/CollinLadina)
4. [Abe Michael](https://github.com/abemichael12)

# Dataset Description

Our [dataset](https://catalog.data.gov/dataset/youth-tobacco-survey-yts-data) encompasses data from the Youth Tobacco Survey (YTS), focusing on tobacco use among youth across various U.S. states, spanning from 1999 to 2017. This dataset, accessible via the U.S. Government's Data.gov portal, has been cleaned to streamline the analysis process. It comprises 10,600 entries and includes key attributes such as the year of data collection, state identifiers, descriptions of tobacco-related behaviors, and demographic information, including gender and educational level of respondents. There are 31 total attributes.

The fields of the dataset detail the specific aspects of tobacco use being surveyed, such as "Cigarette Use (Youth)" or "Smokeless Tobacco Use (Youth)," along with responses categorized into types like "Ever" or "Frequent." The dataset includes robust sample sizes that indicate the scale of data collection for each point. With the dimensions available, we can analyze the correlation between demographic factors, geographical locations, and the prevalence of attitudes toward tobacco use among the youth. This facilitates a multifaceted analysis of trends over time and provides critical insights into effective public health strategies and educational efforts.

# Questions

## Question 1: Which states had the highest number of high school students who have tried tobacco products from 1999 to 2017?

The geospatial data visualization provided highlights the four U.S. states with the highest number of high school students who tried tobacco products from 1999 to 2017, which is crucial for identifying areas where public health interventions are most needed. This analysis is essential for understanding the effectiveness of tobacco control policies, comparing state-level data, and addressing the broader economic and public health implications of youth tobacco use. By exploring factors contributing to high usage rates, such as socioeconomic conditions and local regulations, and analyzing their long-term health impacts, stakeholders can develop targeted strategies to reduce smoking rates among adolescents, ultimately leading to improved health outcomes and reduced healthcare costs.

## Question 2: In those four states with the highest amount of Tobacco using students, how does cigarette use differ by gender and over time? 

The data visualization showing trends in cigarette use among high school students across four states over a decade invites questions about the changes in smoking rates and their correlation with gender. Investigating these trends is vital for assessing the impact of public health interventions and smoking prevention strategies targeted at young populations. By examining these patterns, stakeholders can identify whether male or female students are more responsive to such measures, providing insights that could tailor future efforts more effectively to each group.

Moreover, understanding the dynamics of teenage smoking in these states has significant social and economic implications. Reducing smoking rates among adolescents can lead to lower healthcare costs and improved quality of life in the long run. This analysis also highlights the need for continuous monitoring and adaptation of health policies to address the evolving landscape of youth smoking, ensuring that interventions remain effective against the backdrop of changing social norms and tobacco industry tactics. This comprehensive approach supports not just immediate public health goals but also broader societal benefits by fostering a healthier future generation.

# Manipulations
Our initial dataset contained an extraneous amount of different variables, many of which would not be useful for our analysis. This included variables like DisplayOrder, Stratification, SubMeasure, TopicType, TopicID, etc.

![image](https://github.com/AH171717/MIST-4610-Group-8-Project-2/assets/128336029/5db25c77-2b44-46c8-9970-035dc15292e7)

We opted to narrow it down to just 9 variables of interest we found for analysis, instead of the initial 31. The intent of this cleaned up CSV is for easy determinations regarding tobacco usage of the Youth across the United States. For further cleanup we manipulated variable names to be easier to understand under context, changing things like “Data_Value_Type”  to “Amount”, for example. 

![image](https://github.com/AH171717/MIST-4610-Group-8-Project-2/assets/128336029/6e1aee8e-d7f3-4d74-a09e-3abbba53a180)

As for Tableau manipulations, we created a calculated field called “Number of People” that would help us break the data down into actual population sizes. 

![image](https://github.com/AH171717/MIST-4610-Group-8-Project-2/assets/128336029/cfb304d1-11ba-42e0-bd34-4d55c5479717)

We used this concurrently with the TopicDescription variable, so we could filter out particulars like those among the amount and sample size that smoke cigarettes.

To get the Avg. Data Value used in the second visualization, we took the Data_Value column from our data and, in Tableau, we Averaged the values by State.

# Results

## Question 1 Visualization:
![image](https://github.com/AH171717/MIST-4610-Group-8-Project-2/assets/128336029/93da4826-4eb9-434b-8c71-61e6b8ae5063)


## Question 2 Visualization:
![image](https://github.com/AH171717/MIST-4610-Group-8-Project-2/assets/128336029/32328c1a-56df-47a8-a98f-aa462e0e1305)


# Analysis
In our first question, we aimed to utilize visualizations to uncover and narrate the story behind tobacco usage among high school students in the four states with the highest incidence from 1999 to 2017. The initial query involved locating the top four states with the highest number of high school students who have tried tobacco products, allowing us to be aware of areas where usage is prominent. This geospatial visualization shows that the states North Carolina, West Virginia, Missouri, and New Jersey are the areas with the highest amount of usage, indicating there are common underlying factors contributing to high tobacco usage among adolescents that span across the southeastern and mid-Atlantic regions.

In the 2nd question, the graph provided depicts the trend of cigarette usage among high school students over time, categorized by gender, in the previously listed four states. In our analysis, we created line graphs to depict the decline in cigarette use among high school students from 1999 to 2017 differentiated by gender. The data highlights a consistent decline in cigarette use, which can be indicative of the success of public health campaigns and stricter smoking regulations over this period. The visualization also shows that, initially, male students had higher usage rates than females, but by 2014, the gender gap in smoking rates had significantly narrowed, suggesting an effective response to anti-smoking measures across both genders. New Jersey has had the steepest decline in tobacco usage from around 62% to 16.5% throughout 18 years, which can be attributed to governmental policies being enacted by state and federal legislature like the New Jersey Smokefree Air Act of 2006 and Family Smoking Prevention and Tobacco Control Act of 2009, as well as the increase in tobacco sales tax over time. Missouri had the least decline in usage during this period which could potentially be attributed to the lower tobacco taxes than the national average. According to the CDC, “In 2011, Missouri had the lowest state cigarette excise tax in the United States, at $0.17 per pack” 
