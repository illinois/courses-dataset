
# University of Illinois' Course Catalog and Course Schedule

A collection of all courses offered by the University of Illinois.  There are two datasets maintained:

1. The **course catalog** of all courses that may be offered at Illinois
2. The **course schedule** of courses actually offered in a specific term at Illinois

Download the full CSV dataset files:

1. [Download the full catalog as a single CSV file](https://raw.githubusercontent.com/illinois/course-catalog-dataset/master/course-catalog/2019-fa.csv), CSV file
2. Download the full course schedule as a single CSV file:
  - [Fall 2019 Schedule](https://raw.githubusercontent.com/illinois/course-catalog-dataset/master/course-schedule/2019-fa.csv), CSV file


## Data Format

The first row of the CSV file contains column headers.  Every row after the first contains data. 

### Course Catalog Data Format

The course **catalog** contains one row for each course:

| Year | Term | YearTerm | Subject | Number | Name  | Description | Credit Hours | Section Info | Degree Attributes | Schedule Information | 
| ---- | ---- | -------- | ------- | ------ | ----- | ----------- | ------------ | ------------ | ----------------- | -------------------- |
| 2019 | Fall | 2019-fa  | AAS | 100 | Intro Asian American Studies | Interdisciplinary introduction to the basic concepts and approaches in Asian American Studies [...] | 3 hours. |  | Social & Beh Sci - Soc Sci, and Cultural Studies - US Minority course. |  |
| ... |
| 2019 | Fall | 2019-fa  | STAT | 107 | Data Science Discovery | Data Science Discovery is the intersection of statistics, computation, and real-world relevance [...] | 4 hours. | Same as CS 107 and IS 107. | Quantitative Reasoning I course. | |
| ... |

### Course Schedule Data Format

The course **schedule** contains all data from the catalog for each section followed by data for each section of the course:

| ...ALL catalog data headers | CRN | Section | Status Code | Part of Term | Section Status | Enrollment Status | Type | Start Time | End Time | Days of Week | Room | Building | Instructors |
| --------------------------- | --- | ------- | ----------- | ------------ | -------------- | ----------------- | ---- | ---------- | -------- | ------------ | ---- | -------- | ----------- |
| ... (see catalog above) ... | 41758 | AD1 | A | 1 | A | Open | DIS | 9:00 AM | 9:50 AM | F | 329 | Gregory Hall | Boonsripaisal, S;Sharif, L |
| ... |
| ... (see catalog above) ... | 71476 | AL1 | A | 1 | A | CrossListOpen | LEC | 12:00 PM | 12:50 PM | MWF | THEAT | Lincoln Hall | Fagen-Ulmschneider, W;Flanagan, K |
| ... (see catalog above) ... | 71476 | AYA | A | 1 | A | CrossListOpen | LBD | 2:00 PM | 3:50 PM | W | 1038 | Foreign Languages Building | Zhou, W |
| ... |
 

## Data Source

Data was parsed from the course explorer API: https://courses.illinois.edu/cisdocs/explorer

See `script/` for the script used for parsing.