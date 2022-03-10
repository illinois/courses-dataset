
# University of Illinois' Course Catalog and Course Schedule

A collection of all courses offered by the University of Illinois.  Contains data from both **course catalog** data (describes the course and changes only after formal course revisions) and the **course schedule** (semester-specific offerings like the course meeting dates, time, instructors, etc).

Download the full CSV dataset files:

- [Spring 2022](https://raw.githubusercontent.com/illinois/courses-dataset/master/course-schedule/2022-sp.csv)
- [Fall 2021](https://raw.githubusercontent.com/illinois/courses-dataset/master/course-schedule/2021-fa.csv)
- [Spring 2021](https://raw.githubusercontent.com/illinois/courses-dataset/master/course-schedule/2021-sp.csv)
- [Fall 2020](https://raw.githubusercontent.com/illinois/courses-dataset/master/course-schedule/2020-fa.csv)
- [Spring 2020](https://raw.githubusercontent.com/illinois/courses-dataset/master/course-schedule/2020-sp.csv)
- [Fall 2019](https://raw.githubusercontent.com/illinois/courses-dataset/master/course-schedule/2019-fa.csv)


## Data Format

The first row of the CSV file contains column headers.  Every row after the first contains data.  The first 11 columns contain data about the course from the **course catalog** and the remaining rows are from the **course schedule**.


### Course Catalog Data Format

The data from the **course catalog** comprises of the first 11 columns of data:

| Year | Term | YearTerm | Subject | Number | Name  | Description | Credit Hours | Section Info | Degree Attributes | Schedule Information | ... |
| ---- | ---- | -------- | ------- | ------ | ----- | ----------- | ------------ | ------------ | ----------------- | -------------------- | --- |
| 2019 | Fall | 2019-fa  | AAS | 100 | Intro Asian American Studies | Interdisciplinary introduction to the basic concepts and approaches in Asian American Studies [...] | 3 hours. |  | Social & Beh Sci - Soc Sci, and Cultural Studies - US Minority course. | | ... |
| ... |
| 2019 | Fall | 2019-fa  | STAT | 107 | Data Science Discovery | Data Science Discovery is the intersection of statistics, computation, and real-world relevance [...] | 4 hours. | Same as CS 107 and IS 107. | Quantitative Reasoning I course. | | ... |
| ... |

### Course Schedule Data Format

The data form the **course schedule** is found in the last 13 columns: 

| ... | CRN | Section | Status Code | Part of Term | Section Status | Enrollment Status | Type | Start Time | End Time | Days of Week | Room | Building | Instructors |
| --------------------------- | --- | ------- | ----------- | ------------ | -------------- | ----------------- | ---- | ---------- | -------- | ------------ | ---- | -------- | ----------- |
| ... | 41758 | AD1 | A | 1 | A | Open | DIS | 9:00 AM | 9:50 AM | F | 329 | Gregory Hall | Boonsripaisal, S;Sharif, L |
| ... |
| ... | 71476 | AL1 | A | 1 | A | CrossListOpen | LEC | 12:00 PM | 12:50 PM | MWF | THEAT | Lincoln Hall | Fagen-Ulmschneider, W;Flanagan, K |
| ... | 71667 | AYA | A | 1 | A | CrossListOpen | LBD | 2:00 PM | 3:50 PM | W | 1038 | Foreign Languages Building | Zhou, W |
| ... |
 

## Data Source

Data was parsed from the course explorer API: https://courses.illinois.edu/cisdocs/explorer

See `script/` for the script used for parsing.
