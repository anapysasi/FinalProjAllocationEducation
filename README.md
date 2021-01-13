# Final Project: Allocation of Education Funds

## **DATA ENGINEERING PLATFORMS (MSCA 31012)**
**Team members: Fernando Forero, Christopher Hein, Meghan Rokas and Ana Pilar Ysasi Cillero**

**Autor: Ana Pilar Ysasi Cillero**

## General objective of the project:
1. End to end process of gathering, preparing and storing data in databases.
2. Collaborating with the team on business use case, data preparation and analysis.
3. Connecting to databases, analyzing the data and deriving valuable insights.
4. Creation of reports and dashboards based on the business case to communicate insights.

# Allocation of Education Funds
## Executive Summary:
• UNICEF is a non-profit organization serving children in more than 190 countries.

• The World Bank is an institution that provides both loans and grants to impoverished areas around the world.

• By collecting data from both of these sources, we will analyze the relationship between them on education levels.

• We will look into the World Bank’s past funding and UNICEF’s data on education rates to discover the connection between the allocation of World Bank investments to educational levels around the world.

## Business Use Case:
• There are 195 countries in the world, but a limited amount of money. How does the World Bank distribute its loans and grant? 

• Based on education levels worldwide, is the World Bank distributing its funds properly?

• We will analyze past World Bank education funding and compare it to UNICEF data to see if in years since the funding, education levels have risen in those countries.

• We will also study current education rates to make recommendations for future allocation of World Bank funds.

## Data Tools:
1. *Data Sources:* https://data.unicef.org/dv_index/ (Unicef data) & https://projects.worldbank.org/en/projects-operations/projects-list (World Bank data)
2. *Data Processing:* R, Python & OpenRefine
3. *Data Warehouse:* Google Drive & Google Cloud Platform
4. *Data Modeling:* Python & MySQL
5. *Data Visualization:* Tableau & PowerBI

## Data Modeling:
• Data was cleaned using R, Python, Excel & OpenRefine.

• After analyzing the databases we cleaned the redundant data in an iterative process.

• We redefined some attributes of the database in order to have the best normalization possible.

• We compiled the data from UNICEF and The World Bank into tables, forming an entity relationship model.

## Data Considerations:
• Primary keys were setted as integer (SMALLINT or TINYINT depending on the size of the table).

• Data was processed and cleaned locally.

• As we collected data from different databases, we had to cluster and unify both databases in order to have a unique final and coherent database; i.e. The World Bank sometimes listed their projects regionally, in order to work with a unified database we changed it by country.

• The two datasets are connected by country name keys in the region and countries table, respectively

## Insights
• Grants in education projects are very small compared to other segments within the bank (less than 10%).
• Grants represent 4% of the total amount invested in education by The World Bank.
• Correlation between total amount of investment and the average UNICEF indicators is very low (Total r-squared = 0.04).
• “Specific Investment Loans” is the main strategy used by The World Bank when providing loans to countries (More than double of the next strategy – “Development Policy Lending”)
• There is no clear relation between the indicators and the countries which are receiving the investments. Based on their attendance and completion rates, countries are receiving a disproportionate size of investment: countries with larger indicators are the ones receiving the most money.

## Recommendations
• The World Bank needs to utilize the data available to them to improve their decision making when determining where to allocate their funds.
• UNICEF’s education indicators should be referenced when determining where to invest, as the relation between investments and the indicator values are very low.
• Investments should be also analyzed at a country/region level to be able to guarantee that the bank is investing in regions with the most need. 
•  Based on the insights we’ve seen in the education trends world-wide, we see room for improvement. 
•  The UNICEF education dataset helped to unveil a disconnect in funding and education levels. Additional data from other sources would assist in this analysis.
•  We suggest the World Bank consider UNICEF’s (and other organization’s) databases and include them in their future decision making practices.
