# Population Project

## 1. Project Overview
This project is to analyze and understand population data using UN data.

### 1.1. Problem Statement
A not-for-profit organization is trying to find answers to the below question using UN population data.

1. Rural vs. Urban Population <br>
• World Rural Population % & World Urban Population %. <br>
• Change showing Rural vs. Urban Population % by Region (Continent). <br>
• Urban and rural population % by the country. <br>

2. Population <br>
• Total Population, Male & Female Population, and Sex Ration (Male/100 Female).<br>
• Population by Region (Continent).<br>
• Top 10 most populated countries. <br>

3. Life Expectancy <br>
• World Life Expectancy Rate, World Male & Female Life Expectancy Rate, World Fertility Rate, and Infant Mortality Rate.<br>
• Top 10 Country Life Expectancy. <br>

4. Migration <br>
• Total Refugees and Total Asylum Seekers. <br>
• Top 10 Countries – International Migration % of Population. <br>

5. Population Timeline <br>
• Total Population & % Difference from 2020 Population by country. <br>
• Population data from 1950 – 2100 by country. <br>

6. Total Births & Deaths <br>
• Chart showing side-by-side comparison of total births and deaths. <br>

7. % of City Population to Country <br>

### 1.2. Solution

1. Data Collection <br>
• Collect all the data from different sources. <br>

2. Data Transformation <br>
• Extract, transform, and load data using Power Query. <br>

3. Data Reporting <br>
• Load to Excel worksheet for reporting.<br>
• Load to Data Model (Power Pivot) to perform calculations. <br>

4. Data Analysis <br>
• Build relationships, perform calculated columns, or build measures using DAX. <br>
• Create Pivot Tables for reports. <br>

5. Data Automation <br>
• Create a macro that will refresh data. <br>
• Create a macro that will export data into a new workbook. <br>

6. Data Visualization <br>
• Build charts, graphs, and KPIs.<br>
• Build dashboards that consolidate all the information. <br>

### 1.3. Flowchart
![image](https://user-images.githubusercontent.com/99619460/184936590-6624cd63-acc4-43fb-8d4f-85459ef08b9e.png)

## 2. Data Collection

Data is collected from the below sources.

1. Population Growth Rate in Urban Areas & Capital Cities - https://data.un.org/ 

2. Population, Surface Area and Density - https://data.un.org/

3. Population Growth, Fertility and Mortality Indicators - https://data.un.org/

4. International Migrants and Refugees - https://data.un.org/

5. Total population by sex, annually from 1950 to 2100 - https://population.un.org/wpp/Download/Standard/CSV/

6. Several indicators in 5-year periods, from 1950-1955 to 2095-2100 - https://population.un.org/wpp/Download/Standard/CSV/

7. UN World Locations - https://population.un.org/wpp/Download/Metadata/Documentation/

8. List of Most Populated Cities in the World - https://worldpopulationreview.com/world-cities

### 3. Data Transformation

There are three steps within data cleaning which are all performed using Power Query in Excel.

![image](https://user-images.githubusercontent.com/99619460/184939989-ab3f6ba3-3ecf-431c-bfce-c96f6d4a2bde.png)

#### 3.1. Extract Query

In this section, data is extracted from all different sources. Basic transformation steps are performed such as removing columns, filtering rows, changing data types, etc.

All the files are getting loaded to Power Query. Each files corresponds to Power Query name.

![image](https://user-images.githubusercontent.com/99619460/184940144-8b871aa7-1d45-48bb-b2d3-e59b28f397f2.png)

M Script - https://github.com/Data-Practitioner/Population-Project/blob/main/data_transformation/extract_query

#### 3.2. Transform Query

In this section, data is extracted from all extract queries. Advance transformation steps are performed such as merging, pivoting, changing text, adding custom columns, conditional logic, etc.

All Extract Queries are converted to Transform Queries to clean data. Each Extract Query corresponds to its Transform Query.

![image](https://user-images.githubusercontent.com/99619460/184940417-b151f344-de9f-423e-8258-36d6e3a0495d.png)

M Script - https://github.com/Data-Practitioner/Population-Project/blob/main/data_transformation/transform_query

#### 3.3. Load Query

In this section, data is extracted from all transform queries. Additional transformation steps are performed such as merging, reorganizing columns, etc. All these queries are loaded into data model for building relationship and calculating measures.

All Transform Queries are converted to Load Queries to merge and load queries into worksheet for reporting.

![image](https://user-images.githubusercontent.com/99619460/184940497-d631348c-a093-4b2f-9617-88acaf81712f.png)

M Script - https://github.com/Data-Practitioner/Population-Project/blob/main/data_transformation/load_query

### 4. Data Reporting

All the Load Queries is loaded to Excel worksheet for reporting (raw data). Also, loaded to Data Model (Power Pivot sheet) to perform calculation.

![image](https://user-images.githubusercontent.com/99619460/184940699-736c8dd8-2733-4419-bc7e-3512bdb99862.png)

### 5. Data Analysis

#### 5.1. Building Relationship

The below visual shows only 4 tables are part of the data model, and others are standalone tables. The data model helps to load, retrieve, and analyze extensive amounts of data which is crucial for Excel to load quickly.

![image](https://user-images.githubusercontent.com/99619460/184940913-117e3a05-c3a9-4f4b-a964-8b70ec4bf5d8.png)

#### 5.2. DAX

Below, measures are calculated using DAX in Power Pivot All these measures are used for building reports in the Pivot table.

DAX Code - https://github.com/Data-Practitioner/Population-Project/blob/main/data_analysis/dax

#### 5.3. Pivot Table

All the Power Pivot sheets are loaded into Excel worksheets to build Pivot Tables.

Each Power Pivot sheet corresponds to Excel worksheet which has Pivot Tables.

![image](https://user-images.githubusercontent.com/99619460/184941142-68f6b770-7dcd-49b2-8e6c-8f1bce9578b7.png)

### 6. Data Automation

Using VBA, data will refresh and exported into a new workbook. 

#### 6.1. Data Refresh 

**Example 1**

The macro in the below screenshot will refresh data based on the region that is selected.

![image](https://user-images.githubusercontent.com/99619460/184941389-ceed884a-eb25-4abe-835e-86af0c4b5647.png)

VBA Code - https://github.com/Data-Practitioner/Population-Project/blob/main/data_automation/data_refresh_1

**Example 2**

The macro in the below screenshot will refresh data based on the country that is selected.

![image](https://user-images.githubusercontent.com/99619460/184941808-fba28921-d74b-4e4e-ac97-042470dbd202.png)

VBA Code - https://github.com/Data-Practitioner/Population-Project/blob/main/data_automation/data_refresh_2

#### 6.2. Data Export 

**Example 1**

The macro in the below screenshot will export data into new workbook.

![image](https://user-images.githubusercontent.com/99619460/184942136-e35c7fb8-bc6c-489d-b5eb-09a51d5cc9a6.png)

VBA Code - https://github.com/Data-Practitioner/Population-Project/blob/main/data_automation/data_export_1

**Example 2**

The macro in the below screenshot will export data into new workbook.

![image](https://user-images.githubusercontent.com/99619460/184942216-73b7a332-771f-4b6d-a6d6-b0ca56891df6.png)

VBA Code - https://github.com/Data-Practitioner/Population-Project/blob/main/data_automation/data_export_2

### 7. Data Visualization

All the Pivot Table and raw data in the worksheet is transformed into charts, graphs,and KPI’s to build dashboard.

![image](https://user-images.githubusercontent.com/99619460/184942401-3fe282e2-47a6-4901-927e-e7e986efa6c3.png)

All the dashboards are combined into one master dashboard.

![image](https://user-images.githubusercontent.com/99619460/184942483-5296f196-0b3b-43f5-907d-d8b1175d80c9.png)

### Conclusion

1. Rural vs. Urban Population <br>
• World Rural Population % & World Urban Population %. <br>
• Change showing Rural vs. Urban Population % by Region (Continent). <br>
• Urban and rural population % by the country. <br>

All the points are addressed in DB – PopUrban&CapitalCities sheet.

![image](https://user-images.githubusercontent.com/99619460/184942894-e7ccf8ae-2076-4dce-b655-0e1f481c358b.png)

2. Population <br>
• Total Population, Male & Female Population, and Sex Ration (Male/100 Female). <br>
• Population by Region (Continent). <br>
• Top 10 most populated countries. <br>

All the points are addressed in DB – PopSurfaceArea&Density sheet.

![image](https://user-images.githubusercontent.com/99619460/184943028-18639879-04e1-4f71-8353-2339f943fbbe.png)

3. Population <br>
• Total Population, Male & Female Population, and Sex Ration (Male/100 Female). <br>
• Population by Region (Continent). <br>
• Top 10 most populated countries. <br>

All the points are addressed in DB – PopSurfaceArea&Density sheet.

![image](https://user-images.githubusercontent.com/99619460/184943149-4a27a563-f10c-4ca8-95fe-6947d120155d.png)


4. Migration <br>
• Total Refugees and Total Asylum Seekers.  <br>
• Top 10 Countries – International Migration % of Population.  <br>

All the points are addressed in DB – Migrants&Refugees sheet.

![image](https://user-images.githubusercontent.com/99619460/184943291-34308e0e-bd8f-4849-a0de-06fb693c9962.png)

5. Population Timeline <br>
• Total Population & % Difference from 2020 Population by country. <br>
• Population data from 1950 – 2100 by country. <br>

All the points are addressed in DB – TotalPopBySex sheet.

![image](https://user-images.githubusercontent.com/99619460/184943389-eafd9375-2751-41d1-a09a-58dd56a23cf2.png)

6. Total Births & Deaths <br>
• Chart showing side-by-side comparison of total births and deaths. <br>

All the points are addressed in DB – PopIndicators sheet.

![image](https://user-images.githubusercontent.com/99619460/184943482-2d71f946-4293-40f4-a295-aaccf8ae20c6.png)

7. % of City Population to Country.

All the points are addressed in DB – MaxPopCitiesInWorld sheet.

![image](https://user-images.githubusercontent.com/99619460/184943532-0ef6c3b6-c99d-406e-adeb-5822961d1710.png)



