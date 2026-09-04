# Not All Barriers Are Visible: 1.2% Support in Lithuania

![Research question visual](https://github.com/Ramuneid/1.2-Support-in-Lithuania/blob/main/images/research-question-visual.png?raw=true)
<span style="font-size: 11px; font-family: 'Segoe Print', 'Bradley Hand', 'Comic Sans MS', cursive; color: #555;">Landing page of Power BI report, visual created with Gamma.app</span>

## Project Overview

This project explores the question:

**Who wins in the race for 1.2% support, and who is left behind?**

In Lithuania, **1.2% support** is a part of a resident's already paid income tax that they can allocate to an eligible organisation. The receivers are usually support beneficiaries such as NGOs, public institutions, community organisations, religious communities, schools, Lithuanian organisations abroad, or eligible artists.

The analysis is based on publicly available data from **2020-2024** and focuses on how 1.2% support is distributed among recipients, how this distribution has changed over time, and which organisations receive the most support.

## Project Aim

The aim of this project was twofold:

1. **To explore the distribution of 1.2% support in Lithuania**

   This analysis investigates who receives 1.2% support, how the support is distributed among recipients, and how the situation changed between 2020 and 2024.

2. **To practice and strengthen the full data analysis workflow, with a particular focus on exploring and applying Power BI capabilities**

   This project allowed me to apply skills in data extraction, data cleaning, transformation, modelling, exploratory data analysis, visualization, and publishing a Power BI report.

## Research Questions

The project is guided by the following questions:

- Who are the main recipients of 1.2% support in Lithuania?
- How is 1.2% support distributed among recipients?
- How has the distribution changed between 2020 and 2024?
- Are the biggest recipients becoming stronger over time?
- Who may be left behind in the competition for support?

## Data Sources

The analysis uses public data from **2020-2024**.

Data was collected using:

- Web scraping
- Power BI API connection to public sources

## Tools Used

- Power BI Desktop
- Power BI Service
- Power Query
- DAX
- Python
- Power BI API connection
- Power BI App

## Data Analysis Workflow

### 1. Goal Setting and Research Questions

The project started with defining the aim of the analysis and formulating key questions to guide the exploration.

### 2. Data Extraction

Data was extracted from public sources using web scraping and Power BI API connections.

The data connection was created in a way that allows updates to be reflected when changes are made in the original sources.

### 3. Data Cleaning and Transformation

The data was cleaned, transformed, and loaded using Power Query.

This included:

- Removing unnecessary columns
- Checking and changing data types
- Cleaning text values
- Handling missing or inconsistent values
- Preparing the data for analysis
- Combining data from multiple years

### 4. Data Modelling

The data was structured using a star-schema-based model, with fac_Parama as the central fact table containing support amounts, number of supporters, recipient identifiers, and year.
Supporting dimension tables provide additional context about:

- Support recipients and their characteristics
- Recipient contact and organisational information
- Municipality and population data
- Calendar
  
The model uses one-to-many relationships between dimension tables and the central fact table, allowing support data to be analysed across different years, recipients, organisation characteristics, and geographical areas.
A dedicated calendar table was created to support consistent time-based filtering and yearly comparisons.

Municipality population data was also integrated into the model, allowing support patterns to be explored in relation to the size and characteristics of different municipalities.
Separate measure tables were used to organise DAX calculations and keep the model easier to navigate and maintain. These include general KPIs as well as specialised calculations for the Top 10 recipients and supporter behaviour.

This structure supports interactive filtering and makes it possible to analyse the same support measures from multiple perspectives without duplicating the underlying data.

![Data Model](https://github.com/Ramuneid/1.2-Support-in-Lithuania/blob/main/images/DataModel.png?raw=true)

### 5. DAX Calculations

DAX formulas were used to enrich the dataset and create additional insights.

This included:

- Calculated columns
- Measures
- Ranking calculations
- Yearly comparisons
- Totals and percentage calculations

### 6. Exploratory Data Analysis

Exploratory data analysis was carried out to understand the structure, patterns, and changes in the data.

The analysis focused on:

- Distribution of support among recipients
- Top recipients by amount received
- Top recipients by number of supporters
- Changes over time
- Differences between large and smaller recipients

### 7. Report Design and Interactivity

Power BI visualizations were selected and adapted to make the report flexible and easy to explore.

The report includes:

- Relevant charts and visuals
- Slicers
- Tooltips
- Drill-through pages
- Interactive filtering
- Yearly comparison views

### 8. Publishing

The final report was published in Power BI Service and shared as a Power BI App.

## Key Findings

One of the main findings is that the **top 10 largest recipients** have grown over the five-year period, both in terms of:

- the amount of support received
- the number of people allocating support to them

This suggests that visibility, recognition, and existing reach may play an important role in the competition for 1.2% support.

Additional findings will be listed here:

- Finding 1
- Finding 2
- Finding 3
- Finding 4

## Project Status

This project is currently in progress.

The next steps include:

- Adding more findings
- Refining visualizations
- Improving report interactivity
- Publishing final screenshots or report links
- Updating this README with final conclusions

## How to View the Report

Power BI report link:

[Add your Power BI report or app link here]

## Author

Created by **Ramune Idzelyte**

Have a project where data, people, or impact matter? I would be happy to connect on LinkedIn.
