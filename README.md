# Project idea
In this project, I will analyze how digital and social contacts within the family and workplace are related to subjective well-being and social exclusion in Switzerland. Switzerland was chosen due to its status being one of the wealthiest countries in the world and due to its high GDP per capita - $92,463 GDP per Capita (Richest Countries in the world 2024., n.d.). This wealth is closely connected to how people work (their work processes), their quality of life, and their overall happiness and level of subjective well-being. Living in such a prosperous country likely means that Swiss residents enjoy a high standard of living. Curious about this connection, I want to look at data from the European Social Survey (ESS) portal. I plan to explore happiness levels and examine factors such as work conditions and family life. The goal is to explore how digital and real-life social connections are related to the well-being of Swiss residents.

Source: Richest Countries in the World 2024. (n.d). URL: https://gfmag.com/data/richest-countries-in-the-world/

# Description of Dataset

The data for this study will be obtained from the European Social Survey (ESS), rounds 10 or 11. The dataset includes multiple variables that reflect different aspects of digital and social interactions and estimation of subjective well-being level. It is self-report data.
On this website it is possible to look at all the present data, read the desciption of the variables and download the data set - https://ess.sikt.no/en/datafile/242aaa39-3bbb-40f5-98bf-bfb1ce53d8ef

Nominal variable: “acchome” - This variables represent the ability of the respondent to access the internet from home

Ordinal variable 1: “sclact” - This variable represents answers of respondents to the question “Compared to other people of your age, how often would you say you take part in social activities?”.

Ordinal variable 2: “closepnt” - This variable represents answers of respondents to the question “Taking everything into consideration, how close do you feel to him/her?”.

Interval variable 1: “teamfeel” - This variable represents answers of respondents to the question “If you work in a team, how much do you feel like part of your team?”

Interval variable 2: “happy” - This variable represents answers of respondents to the question “Taking all things together, how happy would you say you are?”

Ratio variable: “ttminpnt” - This variable represents answers of respondents to the question “About how long would it take you to get to where your parents live, on average? Think of the way you would travel and of the time it would take door to door.”

During my future steps, I might remove some variables and add new ones that would be relevant for my topic. These six variables are related to the topic of “Digital and social contacts within family and workplace and its relation to subjective well-being and social exclusion”, so I would primarily focus on them. 

# Motivation to study this topic
Motivation to study this topic lies in several dimensions.

First of all, my personal interest and incentive to explore the country I would like to live in one day. The wealth and high standards of living of Switzerland make it a really attractive country to consider moving.

Second of all, the lack of studies on exploring Switzerland. There are a lot of literature on exploring relationships of subjective well-being and social exlusions with amount of social contacts a person has, but there were no detailed analysis of Switzerland situation.

In the study titled “Technological Affluence and Subjective Well-Being” (Kavetsos, G., & Koutroumpis, P., 2011), a European pooled cross-sectional dataset was used, focusing specifically on internet access and ownership of electronic gadgets in relation to subjective well-being. In my research, I aim to go further by examining how online connections between family members and coworkers or bosses relate to an individual's subjective well-being. Additionally, the country sample used in this study indicates that there has been no similar analysis conducted for Switzerland. It means thet a research gap is detected :)
The responses were collected from 29 countries, including Austria, Belgium, Bulgaria, Croatia, Cyprus, Czech Republic, Denmark, Estonia, Finland, France, Germany, Greece, Hungary, Ireland, Italy, Latvia, Lithuania, Luxembourg, Malta, the Netherlands, Poland, Portugal, Romania, Slovakia, Slovenia, Spain, Sweden, Turkey, and the United Kingdom. But not for Switzerland.

Source: Kavetsos, G., & Koutroumpis, P. (2011). Technological affluence and subjective well-being. Journal of Economic Psychology, 32(5), 742–753.

The research "Always Available, Always Attached: A Relational Perspective on the Effects of Mobile Phones and Social Media on Subjective Well-Being" by Taylor & Bazarova is the closest to my work in terms of measurement focus. The aim of the researchers to address how interpersonal communication across various types media affects the subjective well-being (SWB) (Taylor, S. H., & Bazarova, N. N., 2021). Their study emphasizes digital contacts and happiness, but they focues on romantic relationships, involving one hundred fourteen romantic couples in long-term relationships recruited between January and March 2019. 
In my analysis I will not be limited by "romantic relationships" framework and plan to describe the situation on a more generelazible level.

Source: Taylor, S. H., & Bazarova, N. N. (2021). Always Available, Always attached: A relational perspective on the effects of mobile phones and social media on Subjective Well-Being. Journal of Computer-Mediated Communication, 26(4), 187–206.

I also would like to analyze not only digital connection patterns but also real-life social connections and their relation to subjective well-being. In the study on social capital and subjective well-being (Hommerich, C., & Tiefenbach, T., 2017), researchers propose the concept of social affiliation, measuring the sense of belonging to a social group and being a respected and valued member of society. Relevant variables include feelings of being part of a team and participation in social activities compared to others of the same age, which relate to the sense of belonging. However, this study was conducted in Japan, whereas I aim to focus on Switzerland.

Source: Hommerich, C., & Tiefenbach, T. (2017). Analyzing the relationship between social capital and subjective well-being: The mediating role of social affiliation. Journal of Happiness Studies, 19(4), 1091–1114. https://doi.org/10.1007/s10902-017-9859-9

# Research question
How digital and social contacts within family and workplace are related to subjective well-being and social exclusion?

# Objectives of the research
1. Analyze the relationship between digital and social contacts with family members and colleques at work and subjective well-being and level of social inclusion estimation.
2. Identify key factors affecting happiness levels in Switzerland (i.g. whether access to digital communication tools, frequency of social interactions, and workplace dynamics are related to national well-being trends).

# Data Analysis
The analysis will consist of the following stages:
1. Data Cleaning and Filtering
I will remove the missing values, check whether I need to replace the missing values with the medians of the variables (so I would not worsen my outcome analysis), remove outliers.
2. Standardizing variable formats
I will make sure that my variables' scales are the same, so I could get accurate results.
3. Exploratory Data Analysis:

3.1 Descriptive statistics (mean, median, mode) to describe key variables

3.2 Visualizations (histograms, bar plots, boxplots) to identify trends

These 2 steps help me to check the distributions, evaluate the normality of data distribution and make conclusions on what kind of tests I should use (for example, should I use parametric or non-parametric ANOVA).

4. Hypothesis formulation
5. Hypothesis testing 1: Correlation analysis
This step will help me to examine whether they are relationships between my variables, and if there is, then evaluate the strength and direction of the relationship between two variables. Whether an increase or decrease in one variable is associated with an increase or decrease in another variable.
6. Hypothesis testing 2: Regression analysis
This step will help me to understand whether changes in one variable (the independent variable) are associated with changes in another variable (the dependent variable). Frankly speaking, it allows us to understand how one variable depends on another and to quantify the strength and nature of this relationship.

For this moment of project development I find it hard to understand what type of machine learning techniques can be applied for my data set. Probably at the future stages it will become more obvious for me. 

# Hypothesis
For each type of tests the hypothesis will be formulated separately.

# Limitations
One obvious limitation I can think of right now is that my analysis relies on self-reported survey data, which may include bias. It is a pretty common situation when it comes to self reporting, because people like to respond in a socially desirable way or they misunderstand the questions, for example.


However, there is nothing I can do to tackle this limitation, because I am working with existing data set and I can not change the formulations of the quiestions (to make them more understandable, for example) as well as control the survey process.
