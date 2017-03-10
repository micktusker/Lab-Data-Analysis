# Automation/Semi-automation of Lab Data Analysis

## Aim

To develop an automated semi-automated pipeline to aid with formatting, checking and analysis of laboratory assay data. As a starting point, we will develop it for CD38 data. The current system is manual, time-consuming, error-prone and relies on Excel.

## Plan
* Use Excel VBA code to format and annotate spreadsheets generated by lab software to create output spreadsheets
* Load the output spreadsheets into PostgreSQL
* Create R Shiny pages to retrieve and visualize the data stored in PostgreSQL


## Progress Update

* 2017-03-10: Created an Excel VBA class called "PlateMap" to generate a plate map lookup dictionary and to annotate a results spreadsheet. See its comments for further information.


## Next Steps

* Add a form to the current VBA code to allow users to define the input ranges and to run the code
* Go over the process with Nina on Tuesday 2017-03-14 to see if we can process one experiment.
* Agree on column names for output spreadsheets that can be used in PostgreSQL. We may need to store a mapping in the database of the database columns and table names to more detailed information that is meaningful to users.
