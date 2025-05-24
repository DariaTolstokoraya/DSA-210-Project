# Project idea -- Digital & social contacts and their relation to subjective well-being and social exclusion in Switzerland
In this project, I will analyze how digital and social contacts within the family and workplace are related to subjective well-being and social exclusion in Switzerland. Switzerland was chosen due to its status of one of the wealthiest countries in the world and due to its high GDP per capita - $92,463 GDP (Richest Countries in the world 2024., n.d.). This wealth is closely connected to how people work (their work processes), their quality of life, and their overall happiness and level of subjective well-being. 

Living in such a prosperous country likely means that Swiss residents enjoy a high standard of living. Curious about this connection, I want to look at data from the European Social Survey (ESS) portal. I plan to explore happiness levels and examine factors such as work conditions and family life. The goal is to explore how digital and real-life social connections are related to the well-being of Swiss residents.

Source: Richest Countries in the World 2024. (n.d). URL: https://gfmag.com/data/richest-countries-in-the-world/

# Description of Dataset & Variables

The data for this study will be obtained from the European Social Survey (ESS), rounds 10 or 11. The dataset includes multiple variables that reflect different aspects of digital and social interactions and estimation of subjective well-being level. It is self-report data.
On this website it is possible to look at all the present data, read the desciption of the variables and download the data set - https://ess.sikt.no/en/datafile/242aaa39-3bbb-40f5-98bf-bfb1ce53d8ef

Nominal variable: “acchome” - This variables represent the ability of the respondent to access the internet from home

Ordinal variable 1: “sclact” - This variable represents answers of respondents to the question “Compared to other people of your age, how often would you say you take part in social activities?”.

Ordinal variable 2: “closepnt” - This variable represents answers of respondents to the question “Taking everything into consideration, how close do you feel to him/her?”.

Interval variable 1: “teamfeel” - This variable represents answers of respondents to the question “If you work in a team, how much do you feel like part of your team?”

Interval variable 2: “happy” - This variable represents answers of respondents to the question “Taking all things together, how happy would you say you are?”

Ratio variable: “ttminpnt” - This variable represents answers of respondents to the question “About how long would it take you to get to where your parents live, on average? Think of the way you would travel and of the time it would take door to door.”

During my future steps, I might remove some variables and add new ones that would be relevant for my topic. These six variables are related to the topic of “Digital and social contacts within family and workplace and its relation to subjective well-being and social exclusion”, so I would primarily focus on them. 

Working on the project, I realize that for regression analysis I will add some additional variables that are related to the social inclusion and exclusion domains to have ratio variables:
- “hhlipnt” - Parent lives in same household with a respondent (It has integer type)
- “colprop” - Proportion of colleagues based at the same location (It has integer type)

# Motivation to study this topic & Literature Review
Motivation to study this topic lies in several dimensions.

First of all, my personal interest and incentive to explore the country I would like to live in one day. The wealth and high standards of living of Switzerland make it a really attractive country to consider moving.

Second of all, the lack of studies on exploring Switzerland. There are a lot of literature on exploring relationships of subjective well-being and social exlusions with amount of social contacts a person has, but there were no detailed analysis of Switzerland case.

In the study titled “Technological Affluence and Subjective Well-Being” (Kavetsos, G., & Koutroumpis, P., 2011), a European pooled cross-sectional dataset was used, focusing specifically on internet access and ownership of electronic gadgets in relation to subjective well-being. In my research, I aim to go further by examining how online connections between family members and coworkers or bosses relate to an individual's subjective well-being. Additionally, the country sample used in this study indicates that there has been no similar analysis conducted for Switzerland. It means thet a research gap is detected :)
The responses were collected from 29 countries, including Austria, Belgium, Bulgaria, Croatia, Cyprus, Czech Republic, Denmark, Estonia, Finland, France, Germany, Greece, Hungary, Ireland, Italy, Latvia, Lithuania, Luxembourg, Malta, the Netherlands, Poland, Portugal, Romania, Slovakia, Slovenia, Spain, Sweden, Turkey, and the United Kingdom. But not for Switzerland.

Source: Kavetsos, G., & Koutroumpis, P. (2011). Technological affluence and subjective well-being. Journal of Economic Psychology, 32(5), 742–753.

The research "Always Available, Always Attached: A Relational Perspective on the Effects of Mobile Phones and Social Media on Subjective Well-Being" by Taylor & Bazarova is the closest to my work in terms of measurement focus. The aim of the researchers to address how interpersonal communication across various types media affects the subjective well-being (SWB) (Taylor, S. H., & Bazarova, N. N., 2021). Their study emphasizes digital contacts and happiness, but they focues on romantic relationships, involving one hundred fourteen romantic couples in long-term relationships recruited between January and March 2019. 
In my analysis I will not be limited by "romantic relationships" framework and plan to describe the situation on a more generelized level.

Source: Taylor, S. H., & Bazarova, N. N. (2021). Always Available, Always attached: A relational perspective on the effects of mobile phones and social media on Subjective Well-Being. Journal of Computer-Mediated Communication, 26(4), 187–206.

I also would like to analyze not only digital connection patterns but also real-life social connections and their relation to subjective well-being. In the study on social capital and subjective well-being (Hommerich, C., & Tiefenbach, T., 2017), researchers propose the concept of social affiliation, measuring the sense of belonging to a social group and being a respected and valued member of society. Relevant variables include feelings of being part of a team and participation in social activities compared to others of the same age, which relate to the sense of belonging. However, this study was conducted in Japan, whereas I aim to focus on Switzerland.

Source: Hommerich, C., & Tiefenbach, T. (2017). Analyzing the relationship between social capital and subjective well-being: The mediating role of social affiliation. Journal of Happiness Studies, 19(4), 1091–1114. https://doi.org/10.1007/s10902-017-9859-9

# Research question
My initial research question is "How digital and social contacts within family and workplace are related to subjective well-being and social exclusion?", and during my statistical analysis (chi square test, correlation and regression) I will still stick to it and try to find answer to this question.

For the Machine Learning models implemetation, I will try to focus on less subjective indicator, because it is hard to formalise hapiness. Though my data being all self-reported (meaning it is subjective), I came up to the conclusion that to minimize subjectivity, in this analysis I will replace traditional well-being measures with behavioral (more subjective in comparison to hapiness) indicators as:

1. Social engagement (sclact) as a proxy for isolation risk
2. Workplace integration (teamfeel) to detect exclusion patterns
   
Cluster analysis will identify high-risk groups based on these objectively measurable traits, while controlling for digital access (acchome) and geographic constraints (ttminpnt).

# Objectives of the research
1. Analyze the relationship between digital and social contacts with family members and colleques at work and subjective well-being and level of social inclusion estimation.
2. Identify key factors affecting happiness levels in Switzerland (i.g. whether access to digital communication tools, frequency of social interactions, and workplace dynamics are related to national well-being trends).

# Data Analysis
The analysis will consist of the following stages:
## 1. Data Cleaning and Filtering
I will remove the missing values, check whether I need to replace the missing values with the medians of the variables (so I would not worsen my outcome analysis), remove outliers.
During the data cleansing I have:
1) Removed invalid codes (e.g., 6666, 7777 for travel time / 7, 8, 9 for sclact - taking part into social activities variable / etc.).
2) Filtered ordinal variables (sclact, closepnt) to valid ranges (1–5) and make the corresponding scales.

## 2. Standardizing variable formats
During my variables adjustments, there were some varibles that had contradictory scales. So, for example, "1", as a report number, for 2 different variables could be either "Not at all" or "Much more than often". Such scale differentiation will not give me accurate results (as they supposed to mean the same for "1"; the correct scale would be that "1" stands for "Not at all" for one variable and "Much less than often" for another variable).

So I made sure that my variables' scales are the same, so I could get precise results and correct insights from data.

## 3. Exploratory Data Analysis:

### 3.1 Descriptive statistics (mean, median, mode) to describe key variables

During this step of working with data, I have such findings: 
1) 93% have internet access (acchome).
2) Most Swiss respondents (mean = 3 on 1-5 scale) reported social activity levels "about the same" as their peers. Only a small minority (15% of those without internet access) reported "much less" social activity.
3) High self-reported happiness (mean = 8.1/10) and team belonging (mean = 8.5/10), indicating strong workplace integration.
4) Most Swiss feel "very close" to their parents (tallest bar in distribution), Average travel time to parents is 173 minutes (~3 hours), median = 30 minutes.
5) Happiness scores showed:
Mean = 8.1
Median = 8.0
Mode = 8.0

### 3.2 Visualizations (histograms, bar plots, boxplots) to identify trends

These 2 steps help me to check the distributions, evaluate the normality of data distribution and make conclusions on what kind of tests I should use. And this step is also for making EDA and deriving insights from the data. In my descriptive table I included numerous values (mean, median, min, max, etc.). Here I want to report for "mean" results, because it shows us trends that people have in Switzerland. For the broader picture of the results you can look at the descriptive table in my .jpynb file.

I have got these results:
- On average people in Switzerland do have an access to the Internet, as 1 stands for "Have an access to Internet". So they have an ability to follow the news, stay up-to-dated, communicate with their family and friends via the Internet.
- On average people in Switzerland estimate their level of social activity is about the same as people of their age (as 3 stands for "About the same"). So Swiss people do not feel socially excluded on average.
- On average people in Switzerland feel pretty close to their parents, which is also a great indicator to judge whether Swiss people feel excluded from society and lack attention from their significant others. 
- On average people in Switzerland feel like they belong to a team, as the mean is pretty high (8.5) out of 10 scale. The same situation is for "happy" variable, as Swiss people tend to feel happy on average.
- On average people in Switzerland live 3 hours away (173.4 mins) from their parents, meaning that on average grown-up children and their parents live far apart.

Swiss residents generally enjoy high digital connectivity, social integration and emotional well-being. They report average social activity levels, strong family bonds (despite living ~3 hours from parents) and a sense of belonging in teams, alongside high self-reported happiness. These initial findings in EDA analysis suggest low perceived social exclusion in Switzerland.

## 4. Hypothesis formulation
During my data analysis, I have done 3 tests: Chi-Square Test, correlation analysis and regression. For each of the statistical tests I came up with the own hypothesis.

### 4.1. Hypothesis testing 1: Chi-square Test
H0: There is no association between the type of the area of living and ability to access the Internet from home

HA: There is association between the type of the area of living and ability to access the Internet from home

### Findings:
1) The chi-square test reveals a statistically significant association (p=0.032) between internet access and residential area in Switzerland, with rural farms showing the highest proportion of residents lacking internet access compared to urban areas.
   
2) Our p-value: 0.0317 is less than 0.05, meaning we reject the null hypothesis and state that these two categorical variables are not independently distributed, meaning there is an association between the type of the area of living and ability to access the Internet from home. It means people have different abilities to access the Internet from home in different types of areas they live in.

### 4.2. Hypothesis testing 2: Correlation analysis
This step will help me to examine whether they are relationships between my variables, and if there is, then evaluate the strength and direction of the relationship between two variables. Whether an increase or decrease in one variable is associated with an increase or decrease in another variable.

H0: There is no association between feeling like a part of a team (teamfeel) and being happy (happy)

H1: There is an association between feeling like a part of a team and being happy

### Pearson test revelaed that:
1) Weak but significant link between teamfeel and happy (correlation coefficient is 0.19, p-value < .001 - statistically significant result). So, each 1-point increase in team belonging predicts 0.19 higher happiness
  
2) Negligible correlations for ttminpnt (distance) and closepnt (closeness) with happiness (happy).

### Conslusion: We reject the H0 and accept H1, claiming we have an association between feeling like a part of a team and happiness level.

### 4.3. Hypothesis testing 3: Regression analysis
This step will help me to understand whether changes in one variable (the independent variable) are associated with changes in another variable (the dependent variable).

H0: There is no significant relation between feeling happy (outcome) and the team feeling (continious predictor)

HA: There is a significant relation between feeling happy (outcome) and the team feeling (continious predictor)

### Based on the regression results:
1) Swiss respondents with average team belonging, centered at 0, report high happiness, confirming overall life satisfaction.
   
2) The  regression line indicates each 1-point increase in team belonging (above the mean) predicts higher happiness.

3) Points are densely clustered near the mean (0 to +2 centered scores), suggesting most Swiss experience moderate-to-strong workplace integration. The wider spread at lower scores (-8 to -2) highlights greater happiness variability among those with below-average team belonging.

The regression model explained 4% of outcome variance (R² = 0.04). Both workplace integration (β = 0.14) and parental closeness (β = 0.11) showed small positive associations, while household composition demonstrated no meaningful relationship. The low R² suggests important predictors may be missing from the model.

# Limitations
One obvious limitation I can think of right now is that my analysis relies on self-reported survey data, which may include bias. It is a pretty common situation when it comes to self reporting, because people like to respond in a socially desirable way or they misunderstand the questions, for example.

However, there is nothing I can do to tackle this limitation, because I am working with existing data set and I can not change the formulations of the quiestions (to make them more understandable, for example) as well as control the survey process.

During further phases of the project, I formulated certain limitations I have faced with:

1) Self-report bias in social and well-being measures (I talked about it at the beggining)
2) Modest effect sizes for most correlations (r<0.2), I have found really small corelation coefficient, though some of them being statistically significant.
3) Hard to formalize subjective data. My initial research focus was on measuring hapiness level, but for the ML models implemetations I will shift my attention from subjective well-being levels to social engagement and workplace integration indicators.

# Overall conclusions for statistical analysis (2nd phase):

1) Workplace social integration (team belonging) emerges as the strongest predictor of happiness in Switzerland.
   
2) Closer parental ties show a slight positive association with happiness, suggesting potential cultural trade-offs between family obligations and personal well-being, so family ties are not that significant in determing well-being.
   
3) Physical distance from parents proves irrelevant to happiness or social bonds, challenging assumptions about geographic proximity's role in family relationships.

# Feature Engineering 
To uncover deeper behavioral patterns, enrich my data set and improve cluster differentiation, I engineered two new variables that quantify modern social dynamics. These features were specifically designed to:

1. Capture technology-mediated relationships in Swiss society
2. Measure the tension between professional and personal life
3. Serve as optimized inputs for machine learning algorithms

### 1. Digital Reliance Score

#### What I Did:
I created a binary variable called "digital_reliance" to identify individuals who likely depend on digital communication with their parents. This was done by:
- Calculating the median travel time to parents (ttminpnt)
- Marking as 1 those who:
* Live farther than the median distance and
* Have internet access at home (acchome = 1)
- All others were marked as 0

I did it for my ML models implementation to objectively measure a modern social behavior pattern among Swiss people: maintaining family ties digitally when physical visits are difficult.
This helps test whether digital communication compensates for distance in maintaining social connections (to be verified in clustering).

#### Prediction: 
Individuals with digital_reliance=1 will show higher sclact (level of participation in social activities) scores, suggesting that technology helps reduce isolation.

#### Findings:
Contrary to expectations, Cluster 1 ("Overworked Technology Users") with medium-high digital reliance (digital_reliance=0.63) reported the lowest social activity levels (sclact=2.15). Meanwhile, Cluster 2 ("Digitally-Balanced") with the highest digital reliance (0.76) showed moderate social activity (2.87), still below Cluster 0 ("Traditional Workers") with no digital reliance (sclact=3.40). So, Swiss people with the highest digital activity report the lowest level of participation in social activities.

### 2. Social-Work Balance Index

#### What I Did:
I constructed a continuous variable measuring the trade-off between social and work life by:
- Scaling teamfeel (workplace integration, original scale 0-10) to match sclact's range (1-6) using MinMax scaling.
- Subtracting scaled work integration from social activity frequency:
* social_work_balance = sclact - scaled(teamfeel)

I did it to quantify whether individuals prioritize social activities (sclact) over workplace relationships (teamfeel) or vice versa.

#### Prediction: 
Those with negative social_work_balance (work-focused) may report lower family closeness (closepnt).

#### Findings:
Cluster 1 (most work-focused, social_work_balance=-3.41) showed moderate family closeness (closepnt=3.69), only slightly lower than Cluster 0 (3.92) and Cluster 2 (3.45).

# Machine Learning implementation

For this analysis, I selected K-Means clustering as my primary method because it's particularly well-suited for datasets like mine with clear numerical features. K-Means works by grouping similar data points together while keeping different clusters as separate as possible, which aligns perfectly with my goal of identifying distinct patterns in social behaviors and digital reliance.

To ensure I choose the right number of clusters, I will use silhouette analysis. This method evaluates how well each data point fits within its assigned cluster compared to other clusters, giving a quality score between -1 and 1. Higher scores indicate better-defined clusters where points clearly belong to their assigned group rather than neighboring ones.

As a secondary check, I employ hierarchical clustering (dendogram), which builds a tree-like structure showing how data points naturally group together at different levels of similarity. This approach is valuable because it doesn't require to specify the number of clusters in advance, serving as an independent way to verify the patterns found by K-Means.

This combination of methods that I chose, which are K-Means (for clear cluster definitions), silhouette analysis (for quality measurement), and hierarchical clustering (for natural pattern verification), gives confidence that my findings reflect genuine patterns in the data rather than arbitrary groupings. All techniques were implemented using standardized data to ensure fair comparisons between features measured on different scales.

## Clustering
After checking Elbow Method and Silhouette Score results, I came up with the optimal cluster number which is 3. Below I will report my interpretations of the graphs.

1. Elbow Method Plot
The curve flattens significantly after k=3. The "elbow" (optimal point) is at k=3 where the rate of inertia decrease slows down
So,  k=3 is likely the optimal number of clusters, as adding more clusters beyond this point yields diminishing returns.

2. Silhouette Score Plot
Higher values = better-defined clusters. Scores > 0.5 indicate reasonable structure
The highest score occurs at k=3 (~ >0.22). We also see pretty high indicator when it is 7 clusters. I will still chose to focus on 3 clusters, because 3 clusters are easier to interpret and act upon than 7.
So,  k=3 is likely the optimal number of clusters.

I want to explain my reasoning on cluster namings.

#### 1. Cluster 0: "Work-centric lifestyle"

##### Key Features:
- Lowest digital reliance (0.11)
- Extreme work-life imbalance (-2.18)
- Highest family closeness (3.92)

These individuals:
- Rarely use digital tools for family communication
- Prioritize work (very high teamfeel=9.15) but maintain strong family ties
- Represent traditional work-centric lifestyles

#### 2. Cluster 1: "Overworked Technology Users"

##### Key Features:
- Medium digital reliance (0.63)
- Worst work-life balance (-3.41)
- Lowest social activity (2.15)
  
These individuals:
- Use technology moderately but are consumed by work
- Show the most extreme work-life imbalance
- Sacrifice social activities (sclact is lowest)

#### 3. Cluster 2: "Digitally-Balanced"

##### Key Features:
- Highest digital reliance (0.76)
- Moderate work-life balance (-1.27)
- Balanced work integration (6.28)

These individuals:
- Are the most tech-dependent for social connections
- Maintain better work-life balance than Cluster 1
- Show moderate social activity despite high digital use

The visualization reveals three distinct social behavior profiles. On the left side of the plot, we find the Work-Centric Lifestyle cluster, positioned centrally along the vertical axis but distinctly left-leaning horizontally. These individuals exhibit the lowest digital reliance scores, combined with extremely high work focus (teamfeel ~9.15) and moderately active social lives. Their poor work-life balance scores suggest traditional workers who prioritize office jobs over digital socialization, maintaining in-person connections but struggling to harmonize professional and personal spheres.

Moving toward the middle-right section of the plot, slightly lower vertically, we encounter the Overworked Technology Users. This group presents a paradoxical profile: medium digital reliance coupled with the most extreme work-life imbalance (social_work_balance ~ -3.41) and the lowest recorded social activity. Their position indicates they utilize technology primarily for work purposes rather than social connection, becoming consumed by professional demands at the expense of personal relationships. This cluster exemplifies the "always-on" work culture enabled by partial digital adoption without compensatory social benefits.

The far right section hosts the Digitally-Balanced group, positioned at moderate heights along the vertical axis. These individuals demonstrate the highest digital reliance yet maintain the least negative work-life balance scores, achieving what appears to be sustainable integration of technology into their social and professional lives. Their moderate social activity levels suggest successful adaptation to digital tools without allowing work to dominate, representing a potentially optimal behavioral pattern in our increasingly connected world. The spatial separation between this cluster and the Overworked Technology Users is particularly telling, highlighting how similar technology adoption rates can yield dramatically different lifestyle outcomes depending on usage patterns and boundary-setting.

### K-Means Clustering

K-Means was selected as the clustering algorithm due to its computational efficiency and suitability for identifying spherical clusters in standardized data. The analysis used three clusters (validated through both the elbow method and silhouette scores). Principal Component Analysis (PCA) was integrated to visualize the high-dimensional data in two dimensions, with PC1 explaining 31.8% of variance (primarily capturing digital reliance, where right indicates high and left indicates low technology use) and PC2 explaining 22.5% of variance (reflecting work-life balance, with top representing socially active individuals and bottom representing work-focused individuals).

Three distinct clusters emerged:

- Traditional Socializers (left-center): Low digital use (0.11) with high work focus (9.15) but moderate social activity (3.40)
- Overworked Tech Users (bottom-center): Medium digital use (0.63) with extreme work imbalance (-3.41) and low socialization (2.15)
- Digitally-Balanced (far right): High digital use (0.76) with moderate balance (-1.27) and social activity (2.87)

### Hierarchical Clustering

For additional verification, I apply hierarchical clustering, which offers:
- No need to pre-specify cluster count, letting the data reveal natural groupings.
- Dendrogram visualization, illustrating how clusters merge at different similarity levels.
- Independent confirmation of K-Means results, ensuring methodological reliability.

#### Dendogram
Y-axis (Merge Distance): Shows the distance at which clusters were merged. Higher values mean more dissimilar clusters were combined.

X-axis: Represents individual data points (respondents in your case), though they're not labeled in your screenshot.

#### Agglomerative Clustering

This visualization shows three distinct clusters formed by agglomerative hierarchical clustering (Ward linkage) in a 2D PCA space, where PC1 (31.8% variance) and PC2 (22.5% variance) capture over half of the data's variability, indicating reasonably well-separated groups in this reduced dimension. 

#### Divisive Clustering (Top-Down)

This divisive clustering visualization shows four clusters (0.0 to 3.0) created through recursive binary splitting using K-Means, displayed in a 2D PCA space where PC1 explains 31.8% of the variance. The top-down approach reveals hierarchical structure, with clusters partially separated along PC1 but potentially overlapping due to the limited variance captured in this 2D view. Compared to your earlier agglomerative results (3 clusters), this method provides finer subdivisions at the cost of potential over-segmentation.

## Overall conclusions for ML models implimentations

The clustering analysis successfully identified three distinct behavioral profiles using K-Means, validated by silhouette scores and the elbow method. Hierarchical clustering independently confirmed these groupings. The clusters reveal meaningful patterns: traditional work-centric individuals, overworked technology users and digitally-balanced adapters. PCA visualization (PC1: 31.8%, PC2: 22.5%) highlighted clear separations along digital reliance and work-life balance axes. 

The divisive method split people into more groups, but some may be too small to be meaningful. The analysis shows that balancing tech use and personal life works best—the "digitally-balanced" group had the healthiest lifestyle.

Since all methods gave similar results, we can trust these findings. They clearly group people into different behavior types, which can help create tailored solutions. However, the 2D view might hide some details—looking at the original features could reveal more. In the end, the models did a great job identifying real-world social behavior patterns.

# Overall conclusions about project results

1. Most Swiss people report being very happy (8.1/10) and feeling connected at work (8.5/10). Nearly all (93%) have internet at home, though rural areas have slightly less access.
2. There main lifestyle types were found:
- Traditional workers: Prefer in-person contact, work-focused but with strong family ties
- Overloaded and stressed tech users: Use technology for work, struggle with work-life balance
- Tech-balanced: Use technology wisely while maintaining good life balance
Surprisingly, people who use technology more tend to socialize less in person. This suggests digital tools may be used more for work than social life.
3. Feeling like a part of a team at work matters more for happiness than how close you live to family. Every step up in workplace connections means slightly higher happiness. In our correlation analysis I have found that correlation coefficient is 0.19, p-value < .001 - statistically significant result). So, each 1-point increase in team belonging predicts 0.19 higher happiness.
4. K-Means & Hierarchical Clustering agreed on the 3 key groups.
5. PCA Visualization showed clear splits: PC1 = tech use (left=low, right=high), PC2 = work-life balance.
6. Divisive Clustering suggested finer subgroups, but 3 clusters were optimal for clear patterns.
  
These findings could help encourage healthy digital habits. The study shows how a wealthy, tech-savvy country like Switzerland balances digital life with personal well-being - lessons that could apply to similar nations.

In Switzerland, work relationships matter most for happiness. Technology helps, but needs to be balanced to avoid taking over personal life. The healthiest group uses technology moderately while keeping good work-life boundaries.
