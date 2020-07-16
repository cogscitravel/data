# Data from Rissman and Jacobs (2020)
## _submitted as a letter to Cognitive Science_

There are three files in this repository: `distances.tsv` and `responses.tsv`, which detail participant responses, and `questions.tsv` that provides a key to the question text.

Both files contain individual participant responses from a survey of nearly 500 cognitive scientists about their conference-related travel. Each dataset represents the reference data we used for generating all figures at the [paper's supplementary website](http://cogscitravel.github.io/survey/).

The data schema of each file is as follows:

_DISTANCES.TSV_:
```
ResponseId                      : Anonymized ID associated with each participant
Trip_Number                     : Trip number (1 to 8)
raw_response                    : What the respondent actually filled in, unchanged from the survey
units                           : Units (if the respondent specified)
distance_in_raw_response_units  : Numeric, miles/kilometers traveled
mode                            : Stated mode of transportation, if any (e.g. car)
likely_dominant_mode            : If multiple modes were provided (e.g. car and plane), 
                                  best guess about modality of longest single leg.
distance_in_kilometers          : Conversion of all miles-units responses into kilometers
```

_RESPONSES.TSV_:
```
ResponseId    : Anonymized ID associated with each participant
Finished      : Whether the participant completed the survey or not
RecordedDate  : What date the survey was completed
Question      : The text of the question the participant answered
Value         : The answer the participant provided (string column)
```

_QUESTIONS.TSV_:
Please see `questions.tsv` for plain English descriptions of the qualtrics headers.
* Those with numeric reponses * : `Q15_1, Q9_\*, Q12_\*, Q10_1, Q6_1, Q7_1, Q2, Q23`
* Those with character responses * : `Q16_\*, Q8, Q3, Q5, Q14`
