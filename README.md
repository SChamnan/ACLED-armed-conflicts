# Analyzing Armed Conflict Using ACLED Dataset
A Tableau dashboard created to analyze conflicts in 75 countries in 8 regions of the world. For interative dashboard, click [here](https://public.tableau.com/app/profile/chamnan.suon/viz/DSDA2015DashboardPresentation/Dashboard2). Datasource used to develop this dashboard comes from ACLED website.

Overall view of the dashboard on Tableau

Figure 1.
![image](https://github.com/user-attachments/assets/48bdd715-d4d0-40be-bfe0-6ea7c645d50a)

## Objectives
To answer the following questions
- What are the total number if conflict and fatalities between 2017 and 2018 in the covered regions?
- How many fatalities occurred in each region? And which region has the most fatalities?
- What are the conflict types and which one has resulted in the most fatalities?
- What are the 5 countries with the most fatalities?

## Datasource and Data Clearning
Dataset is obtained from Armed Conflict Location and Event Data (ACLED), an inititative focused on collecting, analyzing, and mapping crisis events through disaggregate data. Below are bullet points describing how the dataset is processed and cleaned:
- Total of 22 fields and 143,853 rows are downloaded to a csv file
- Used Data cleaning function on GoogleSheet to handle missing and duplicate data
- Removed unneeded fields
- Detected and deleted over 13k duplicate rows
- Used Tableau built-in feature to change `event_date` data type from string to date type
After data cleaning process, I have a nice and clean dataset of 15 fields and 130,212 rows ready to be used.

#### Field Names and Descriptions
- `region` 8 regions (Western Africa, Northern Africa, Middle Africa, Southern Africa, Eastern Africa, Middle East, Southern Asia, and South-Eastern Asia)
- `fatalities` total deaths in each conflict
- `event_date` date of when a conflict happened
- `conflict_type` 6 types of conflicts (Battle-No changes in territory, Battle-Government regains territory, Battle-Non-state party overtakes territory, Remote violence, violence against civilians, and riots/protests)
- `country` countries in covered regions

## Using and Describing the Dashboard
The upper part of the dashboard (see figure 2.) shows title and a brief description of the datasource. Moreover, it describes a high level of data such as regions, countries, and timeframe being analyzed. Futhermore, we see basic statistics showing total countries, total conflicts and total fatalities. Each red dot on the map represents an event and, if you hover over on the map, region name, country name, exact location of the event, and total fatalities are displayed on each dot. Both the left and right side provides the total fatalties in each region. To see how many conflicts and fatalities occurred per month in each region, hover over each mini graph.

Figure 2.
![image](https://github.com/user-attachments/assets/734a5175-93a4-43a5-896b-29376e65e6e7)

The bottom part of the dashboard (see figure 3.) displays two bar graphs and summary section. On the left side, the bar graph shows top conflict types based on total fatalities. As we can note, 'battle with no changes in territory' appears to have the most fatalities. If you hover over the bar, a small pop-up list will appear explaining the total fatalities and listing top countries under this conflict type (see figure 4.)

Figure 3.
![image](https://github.com/user-attachments/assets/77bbfbbc-08ab-4963-9867-94104e665805)

Figure 4.
![image](https://github.com/user-attachments/assets/f69aa098-f1f3-4508-b13b-ff0385881065)

The bar graph on the right side displays the top 5 countries with the most fatalities. Similarly, if one hovers over each bar, a small pop-up view will appear with a table describing each conflict (See Figure 5.)

Figure 5.
![image](https://github.com/user-attachments/assets/8bcf4010-c614-4981-9c6e-3ec955cbf33c)


## Findings and Insights
Between 2017 and 2018, almost 60% of total fatalities occurred in the Middle East region, making it the least safe region among those analyzed here. Moreover, we learned that over 160,000 fatalities happened in Syria, Afghanistan, and Iraq, with over 40% of the fatalities happening in Syria alone. This made Syria the most dangerous country compared to other 74 countries in this dataset. With regards to the conflict type, a total of 128,082 fatalities were caused by 'battle with no changes in territory,' making it the type of conflict to result in the most fatalities. These numbers and figures show how wars and political conflicts cause hundreds of thousands of deaths each year.

## Challenges
I would like to compare the trends of fatalities over time, perhaps in a recent year, to see which countries have decreased theeir number of fatalities. However, to download ACLED datasets, I need an access key which is not available for general users.



