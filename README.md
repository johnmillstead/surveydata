# surveydata

My goal is to create an easy to read and understand database/graphic/report of our organization's annual report survey.

I am using this project to learn both Neo4j and Python.

Source Data: Annual employee survey completed in Survey Monkey.
Challenges: The survey uses complex skip logic, text fields, and non-standardized data input types. Also, the .csv from SV splits arrays into columns -- one for each available selection. For example one question asks what languages do you speak?  A drop-down list includes possible answers (ie, English, Spanish, French, etc.) but the .CSV has a column for English, a column for Spanish, etc.

My first step is to identify the data I want to track and then clean the data to remove erroneous data and blank spaces.

Our organization is comprised of 'associates' who travel and offer their services (ministry) around the world. Associates have different skillsets (specialty areas) where they minister.

Possible Nodes:

(Associate)
(Specialty)
(Country)
(Language)
(HealthCoverage)
(Organization)

Relationships

[SPEAKS LANGUAGE]
[SERVES_IN COUNTRY]
[SERVES_AT_ORGANIZATION]
[HAS_HEALTH_COVERAGE]
[SPECIALIZED_IN]

I will first create a clean employee table by exporting employee info (employee id, fund id, last, first) to a spreadsheet. I will use this table for the associate node.

I will then clean-up the SM data and add the employee id to the data.

I will attempt to learn OpenRefine to help clean the data.
