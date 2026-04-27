# Netflix Sales Database Analysis

# Project Objective
The main objective of this project is to:
- Analyze Netflix’s content distribution (Movies vs TV Shows)
- Identify trends in content addition over the years
- Understand genre popularity and audience targeting
- Explore global availability of content
- Build an interactive dashboard for business insights

# Business Problem
Streaming platforms like Netflix face challenges such as:
- What type of content should be produced more (Movies or TV Shows)?
- Which genres attract the most audience?
- In which countries is content most widely available?
- How has content growth changed over time?
- Which ratings dominate the platform?

Without proper analysis, content investment decisions can lead to low engagement and wasted resources.

# Solution (What This Project Does)
This project transforms raw Netflix data into actionable insights by:

- Cleaning and structuring messy data
- Creating relational datasets
- Building an interactive Power BI dashboard
- Providing visual insights for decision-making

# Tools Used
- Microsoft Excel – Data Cleaning & Preprocessing
- MySQL Workbench – Data Modeling & SQL Queries
- Power BI – Data Visualization & Dashboard

# Project Workflow

## Step 1: Data Cleaning in Excel
- Removed duplicates and handled missing values
- Used Text to Columns for splitting data
- Applied functions:
TRIM, LEFT, RIGHT, UNIQUE
SUM, AVERAGE, MIN, MAX
SUMIF, COUNTIFS, IF
VLOOKUP, XLOOKUP
- Created Pivot Tables for initial analysis

Separated columns:
- Cast
- Countries
- Directors
- Description
- Listed In (Genres)
- Title

Standardized column formats
Exported cleaned data to CSV format

## Step 2: Data Modeling in MySQL
Database Creation:

CREATE DATABASE netflix_data;

USE netflix_data;

Data Import:
- Import cleaned CSV into MySQL

Creating Relational Tables:

1. Cast Table
Converted multiple cast columns into rows using UNION
Created normalized table: netflix_cast

2. Countries Table
Extracted country-wise availability
Created table: countries_released

3. Directors Table
Structured director data
Created table: netflix_directors

4. Genres Table
Extracted categories (Listed In)
Created table: netflix_listed_in

These steps convert denormalized data → normalized relational structure

## Step 3: Power BI Dashboard

### Overview Dashboard

Includes:

- Shows Added by Date
Area chart showing growth of Movies vs TV Shows

- Shows by Rating
Stacked column chart of content ratings

- Top 10 Genres
Bar chart showing most popular categories

- Countries Available
Map visualization of global content distribution

### Single Title View Dashboard
- 🎬 Slicer (Movie/TV Show)
- 📅 Release Year KPI
- 🔞 Rating KPI
- 📝 Description Card
- 🎭 Listed In (Genres)
- 🎬 Directed By
- 👥 Cast Members
- 🌍 Country Map
- 📸 Dashboard Preview

### Overview Page

Single Title View Page
- 📈 Key Insights from Analysis
- 📊 Content Growth :
 Rapid increase in content after 2016
Movies dominate the platform compared to TV Shows
- 🎭 Genre Trends : 
Drama and International Movies are the most popular
Comedy also holds a strong share
- 🌍 Global Distribution : 
Content is highly concentrated in:
United States,
India
and United Kingdom
- 🔞 Ratings Analysis
Majority content falls under:
TV-MA and 
TV-14

# Business Recommendations
- Focus more on high-performing genres (Drama, International content)
- Expand content production in emerging markets
- Increase investment in TV Shows for long-term engagement
- Maintain balance of mature and family-friendly content
- Use historical trends to plan future releases

# Conclusion

This project demonstrates how raw data can be transformed into meaningful insights using:

- Data Cleaning (Excel)
- Data Modeling (MySQL)
- Data Visualization (Power BI)

It helps stakeholders make data-driven decisions in content strategy and audience targeting.
