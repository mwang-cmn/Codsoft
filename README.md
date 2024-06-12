## Emergency Room - Patient Satisfaction Report in PowerBI

### Project Overview
In this project, I analysed data from an Emergency Room in a Hospital. The aim of this project is to gain insights on the satisfaction level of Patients who visited an Emergency room between August 2019 and October 2020. Operational analysis in healthcare facilities is crucial in ensuring that health systems run efficiently while delivering high quality and appropriate care. Solutions from the following insights highlight the areas to improve resource allocation and strategies to improve patient experience and overall satisfaction.

### Data Sources
The data used in this analysis can be found [here](https://github.com/mwang-cmn/Emergency-Room-Hospital-Dashboard/blob/main/Hospital%20ER.csv)
Here is a detailed description of the Hospital ER dataset

| Column Name            | Data Type | Description                                                    |
|------------------------|-----------|----------------------------------------------------------------|
| `date`                 | DATETIME  | The date and time when the patient visit occurred.             |
| `patient_id`           | VARCHAR   | A unique identifier for each patient.                          |
| `patient_gender`       | CHAR      | The gender of the patient. Values can include 'M' and 'F'.     |
| `patient_age`          | INT       | The age of the patient.                                        |
| `patient_sat_score`    | INT       | The patient satisfaction score, ranging from 1 to 10.          |
| `patient_first_initial`| CHAR      | The first initial of the patient's first name.                 |
| `patient_last_name`    | VARCHAR   | The last name of the patient.                                  |
| `patient_race`         | VARCHAR   | The race or ethnicity of the patient.                          |
| `patient_admin_flag`   | BOOLEAN   | Indicates whether the patient was admitted (TRUE) or not (FALSE). |
| `patient_waittime`     | INT       | The waiting time for the patient in minutes.                   |
| `department_referral`  | VARCHAR   | The department to which the patient was referred, if applicable. |

### Data Cleaning and Transformations
I cleaned the data in Power Query and created the following;
- Created measures - Admission rate(%),, Total Patients, Average Satisfaction Score, Average Waittime in minutes
- Created calculated columns - Time of Day, Time Slot, Date Hierarchy, Age Group, Age_Bucket
### Insights
- During the period, the Emergency room had 9,216 patients visits and the overall Average Satisfaction Score was 5.47 out of 10. Only 50% of total patients were admitted to the hospital for further medical attention.
- During patient visits, the waiting time before a patient could see a practitioner was 35 minutes on average. Additionally, 34% of the total visits occurred during late night hours ie 11PM and 6AM, While only 16% of visits occurred during evening hours i.e. 6PM - 10PM. 
- The overall average satisfaction for male patients was 5.03 while female patients' stood at 4.96. Male patients ranked the renal department the lowest at 4.5, while female patients ranked the Physiotherapy department the lowest at 5.29. 
- Walk in Patients, without departmental refferals, and Patients who visited the renal department, ranked the Emergency room the lowest at 5.4 and 5.3, respectfully.
- The Average satisfaction was relatively uniform across all age-groups.
[View PowerBI file here](https://github.com/mwang-cmn/Emergency-Room-Hospital-Dashboard/blob/main/Healthcare%20-%20Dashboard.pbix)

### Recommendations
1. Reduce Waiting Times
   - The average waiting time before patients can see a practitioner is 35 minutes. Consider streamlining processes, optimizing triage, and allocating resources efficiently to reduce waiting times.
   - Implement strategies such as fast-track lanes for less severe cases or using technology (e.g., appointment scheduling apps) to manage patient flow effectively.

2. Improve Late-Night Services
   - Since 34% of visits occur during late-night hours (11 PM to 6 AM), focus on maintaining high-quality services during these times by ensuring adequate staffing, maintain cleanliness, and providing timely care even during off-peak hours to enhance patient satisfaction.

3. Department-Specific Interventions
Address department-specific satisfaction issues:
   - For male patients, improve satisfaction in the renal department (average score of 4.5). Investigate reasons for dissatisfaction and implement changes.
   - For female patients, address concerns in the Physiotherapy department (average score of 5.29). Enhance communication, comfort, and personalized care.

[Preview of Dashboard](![snap](https://github.com/mwang-cmn/Emergency-Room-Hospital-Dashboard/assets/73072045/a03117bf-324a-4578-a482-48fe9f42beaa))


