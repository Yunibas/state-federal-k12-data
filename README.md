# TEA Reporting Data

## Comprehensive Report on Texas Public Schools

### Overview

The Comprehensive Report on Texas Public Schools describes the status of public education in Texas. The report provides information on a wide range of topics including: academic excellence indicators; state assessments; graduation and dropouts; grade-level retention; accountability ratings; curriculum; and charter schools.

[Web Page](https://tea.texas.gov/reports-and-data/school-performance/accountability-research/comprehensive-report-on-texas-public-schools)

### Files

Have not downloaded PDF files at this time.

### Notes

There is a ton of valuable data here. The problem is that it is only available in PDF format. Need to figure out how well this data can be parsed with a PDF "scraper".

Possible JavaScript libraries for parsing:

-  [pdf-parse](https://www.npmjs.com/package/pdf-parse)
-  [pdfreader](https://www.npmjs.com/package/pdfreader)

## Discipline Data

### Overview

The Discipline Data Products are downloadable reports and files. The statistics in these products are extracted or calculated from the data collected through the Public Education Information Management System (PEIMS). They are grouped into four categories:

-  Discipline Reports
-  Discipline Action Group Summary Reports
-  TAKS Assessment Reports for Students in Discipline Settings
-  STAAR Assessment Reports for Students in Discipline Settings

[Web Page](https://tea.texas.gov/reports-and-data/student-data/discipline-data-products/discipline-data-products-overview)

### Files

```text
<year>-<entity>_Discipline_Summaries.csv
2022-District_Discipline_Summaries.csv
```

### Notes

-  Available as summaries by school, district, region and state.
-  Includes school years 2018-2021 (3 years)
-  Data available as CSV
-  There are many unreported rows (value is "-999")
-  Data is divided into numerous categories thus multiple rows per entity (school, district, etc.)
-  District identifiers appear to be their State identifier (Federal identifier not included)
-  There are additional reports available that attempt to describe assessment results for students who have received disciplinary actions.

## Snapshot District Profiles

### Overview

Snapshot provides an overview of public education in Texas, at both the state and district levels, and includes almost 100 separate data elements to either browse or download. Snapshot also combines the data into summary tables based on specific characteristics, and its peer search function allows a user to group districts according to shared characteristics.

[Web Page](https://rptsvr1.tea.texas.gov/perfreport/snapshot/2020/index.html)

### Files
```
# Data file
<year>-District_Snapshot.csv

# Layout file
<year>-Snapshot_Layout.lyt
```

### Notes
- Data is only available at state and district granularity
- Data is available on a per school year from 1995-2020
- Export formats are Excel & comma-delimited
- Columns require descriptors to translate which can be downloaded as "layout" text file
- Report options are 1) district detail, 2) distribution stats, 3) summary tables
- Report includes:
  - Num schools
  - Num students
  - Demographic aggregates
  - Attendance Rates
  - Dropout Rates
  - Graduation Rates
  - Graduation Counts
  - STAAR outcome aggregates
  - College admissions
  - SAT averages
  - ACT averages
  - Staff FTE
  - Teacher FTE
  - Staff aggregates
  - Salary averages
  - Staff/Student ratios
  - Teacher aggregates
  - Tax/Student value
  - Tax rates
  - Revenue aggregates
  - Financials aggregates (assets, expenditures)
  - Disctrict size
  - Community type
  - Property wealth

## Campus and District Types
### Overview
The National Center for Education Statistics (NCES) has a classification system that categorizes campuses into categories based on population size and proximity to urban areas. NCES classifies campuses into twelve categories, composed of four basic types (City, Suburban, Town, and Rural) which are further differentiated by size (in the case of City and Suburban assignments) and proximity (in the case of Town and Rural assignments).

### Files
```
<year>-<entity>_NCES_Categories.xlsx
2020-School_NCES_Categories.xlsx
```

### Notes

-  Available by school or district
-  Includes school years 2007-2020
-  Data available as Excel file
-  Excel file contains summary sheet, data dictionary sheet, and data sheet
-  Data includes NCES identifiers but not State identifiers
-  Data describes community types and sizes (e.g. "Large City", "Remote Rural")

# NCES Reporting Data

## Common Core of Data (CCD)

### Overview
The primary purpose of the CCD is to provide basic information on public elementary and secondary schools, local education agencies (LEAs), and state education agencies (SEAs) for each state, the District of Columbia, and the outlying territories with a U.S. relationship.

[Web Page](https://nces.ed.gov/ccd/files.asp)

### Files
```text
<year>-<entity>_NCES_Directory.csv
2022-School_NCES_Directory.csv
```

### Notes

- Provides Federal identifiers and other metadata for all public districts and schools in the nation
- Data is available from 1985 to current
- Data can be downloaded by state, district, and school
- Once "Nonfiscal", "Level" and "School Year" is selected you will see a link for Flat and SAS Files under "Data File -> Directory"
- The download is a ZIP file containing a CSV and a SAS(?) formatted file
- The data contains only Federal identifiers (NCES ID) so there is no direct association identifier to link back to TEA identifiers