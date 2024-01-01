# Sustainable Development-Goals
The trend of sustainable development goals (SDGs) over a period of 2000 - 2022

---
### TABLE OF CONTENT

1. [PROJECT OVERVIEW](#project-overview)
2. [DATA SOURCE](#data-source)
3. [TOOLS](#tools)
4. [DATA CLEANING AND PREPARATION](#data-cleaning-and-preparation)
5. [EXPLORATORY DATA ANALYSIS](#exploratory-data-analysis)
6. [DATA ANALYSIS](#data-analysis)
7. [FINDINGS](#findings)
8. [RECOMMENDATION](#recommendation)
9. [LIMITATION](#limitation)
10. [REFERENCE](#reference)
---

### PROJECT OVERVIEW

The project is on the analysis of dataset gotten from United Nations Sustainable Development Goals (SDGs) for 2000 to 2022 for various countries. The aim of the analysis is to identify the trends of the various SDGs for various countries.

### DATA SOURCE

The dataset used for this project was gotten from [Kaggle](https://www.kaggle.com/datasets/sazidthe1/sustainable-development-report) as at December 26, 2023.

### TOOLS

-	Microsoft Excel
-	Microsoft Power BI
-	Microsoft PowerPoint

### DATA CLEANING AND PREPARATION

Using Microsoft Excel, the data was cleaned by ensuring that there were no duplicates. Spelling checks were also performed on the fields for consistency. Blank-value check was done to ensure that there was no inappropriate blank cell.
The column headers were renamed to match the exact SDG goal that was represented. A new worksheet was created for the country code, country and flag URL of the country. The URL was gotten from [Country Flags](https://www.countryflags.com/). This was done by copying the distinct value of the country and country code from the original worksheet. Then, using power query in Excel, the flag URL column was gotten by:
-	Duplicating the country column
-	Renaming the column as flag URL
-	Lowercase for all the values
-	Replacing the space between two-worded countries with hyphen (e.g. burkina faso as burkina-faso)
-	Adding the prefix and suffix of the flag URL to the values.

### EXPLORATORY DATA ANALYSIS

The KPI asked during this project was the trend of various SDG goals over time.

### DATA ANALYSIS

Using Microsoft Power BI, a relationship was created in the model between the two worksheets, using one-to-many relationship for the country code and country. Measures were created for all the columns of the SDG goals using the template:
```
Measure = SUM(worksheet[‘goal column’])
```
A field parameter was created for all measures that was created. The dashboard background was designed in Microsoft PowerPoint, saved as a SVG file and imported into Power BI. 

### FINDINGS

It was observed that:
-	There was a relative increase in most of the trends over time for most the goals.
-	Some of the goals have a zero value which could be as a result of no values for that goal in that country.

### RECOMMENDATION

More support and enlightenment are needed in some of the countries to achieve the SDG goals. 

### LIMITATION

No noticeable limitations for this project.

### REFERENCE

[YouTube](www.youtube.com)

