---
# National ACT Average Study Compared to US Public Universities ACT Percentiles
---


## Problem Statement
A national college preparatory program wants to investigate if public schools are generally accepting the students with average ACT scores. Since the program has no budget for the project they are asking to see if this is a line of questioning worthy of pursuing.


<br>
There are many factors that go into the admission process however the information gathered from this notebook could potentially work towards informing students on ther standing on a national level at public universities based on comparisons of average ACT scores.

<br>
This is to inform students that plan to apply in their own state If they should expect their scores to be advantages for public schools, however, being in-state applicant should give them a leg up on out-of-state applicants.

I will select which states are most participative and their respective public universities to explore this potential connection.

---
## Contents:
- [Problem Statement](#Problem-Statement)
- [Background](#Background)
- [Outside Research](#Outside-Research)
- [Chosen Data](#Chosen-Data)
- [Conclusions and Recommendations](#Conclusions-and-Recommendations)

---
## Background
In the United States highs schoolers typically take a standardized tests, SAT or ACT, to determine if they are college ready. It is typically required by universities and colleges to determine admission. There are many debates as to the credibility of these tests and their measure of "readiness" from grade point average to extra curriculars. In this notebook it is important to note that the maximum ACT score is 36. Additionally that note note different area of the US have different preferences.

## Outside Research
Important Note because I was only looking at data avaliable for 2017 to 2019 I wanted to potentiallly gather the average composite scores for the years 2020-2022 I summarized the results of my search in the table below with the location linked.


<br>
Table of Average ACT Scores from 2017 to 2021

|Year|*Source*|Average ACT Composite Score|
|---|---|---|
|2017|*ACT.Org [Source](https://www.act.org/content/dam/act/unsecured/documents/cccr2017/ACT_2017-Average_Scores_by_State.pdf)*|21.0|unk|
|2018|*ACT.Org [Source](https://www.act.org/content/dam/act/unsecured/documents/cccr2018/Average-Scores-by-State.pdf)*|20.8|unk|
|2019|*ACT.Org [Source](https://www.act.org/content/dam/act/secured/documents/cccr-2019/Average-Scores-by-State.pdf)*|20.7|unk|
|2020|*ACT.Org [Source](https://www.act.org/content/dam/act/unsecured/documents/2020/2020-Average-ACT-Scores-by-State.pdf)*|20.6|unk|
|2021|*ACT.Org [Source](https://www.act.org/content/dam/act/unsecured/documents/2021/2021-Average-ACT-Scores-by-State.pdf)*|20.7|unk|


<br>

Table of Test Policies at States of Interest

|State|*Source*|Required Test Type|
|---|---|---|
|Rhode Island|State Website [Source](http://www.ride.ri.gov/InstructionAssessment/Assessment/PSATandSAT.aspx#39491532-exemptions-from-testing)|SAT|
|New Hampshire|Governement Website [Source](https://www.education.nh.gov/sites/g/files/ehbemt326/files/inline-documents/nh_sat_school_day_faqs.pdf)|SAT|
|Michigan|Governement Website [Source](https://www.michigan.gov/documents/mde/Guide_to_State_Assessments_622260_7.pdf)|SAT|
|Delaware|Governement Website [Source](https://www.doe.k12.de.us/Page/2717)|SAT|
|Alabama|Governement Website [Source](https://www.alsde.edu/sec/sa/Pages/assessmentdetails.aspx?AssessmentName=ACT%20with%20Writing&navtext=ACT%20with%20Writing)|ACT|
|Kentucky|Governement Website [Source](https://education.ky.gov/AA/Assessments/Pages/ACT.aspx)|ACT|
|Louisiana|Governement Website [Source](https://www.louisianabelieves.com/measuringresults/assessments-for-high-schools)|ACT|
|Mississippi|Governement Website [Source](https://mdek12.org/OSA/ACT)|ACT|
|Montana|Governement Website [Source](http://opi.mt.gov/Leadership/Assessment-Accountability/MontCAS/Required-Assessments/ACT-With-Writing-FAQ)|ACT|
|Nevada|Governement Website [Source](http://www.doe.nv.gov/Assessments/College_Career_Readiness_Assessments_ACT/)|ACT|
|North Carolina|Governement Website [Source](https://www.dpi.nc.gov/districts-schools/federal-program-monitoring/every-student-succeeds-act-essa)|ACT|
|Utah|Governement Website [Source](https://www.schools.utah.gov/assessment/assessments)|ACT|
|Wisconsin|Governement Website [Source](https://dpi.wi.gov/assessment/act)|ACT|


---

## Chosen Data

* [`act_2017.csv`](./data/act_2017.csv): These are the ACT Scores by State for 2017
* [`act_2018.csv`](./data/act_2018.csv): These are the ACT Scores by State for 2018
* [`act_2019.csv`](./data/act_2019.csv): These are the ACT Scores by State for 2019
* [`sat_act_by_college.csv`](./data/sat_act_by_college.csv): Ranges of Accepted ACT & SAT Student Scores by Colleges for 2022


## Data Dictionary


The following is a summary of the features within various data sets that will be analyzed throughout this notebook.

|Feature|Type|Dataset|Description|
|---|---|---|---|
|state|*object*|act_17_to_19|This is the state within the US.|
|participation_17|*float*|act_17_to_19|This is the size of the high school population being tested in 2017.|
|composite_17|*float*|act_17_to_19|This is the average composite score for for high school 2017.|
|participation_18|*float*|act_17_to_19|This is the size of the high school population being tested in 2018.|
|composite_18|float|*act_17_to_19*|This is the average composite score for 2018.|
|participation_19|*float*|act_17_to_19|This is the size of the high school population being tested in 2019.|
|composite_19|*float*|act_17_to_19|This is the average composite score for 2019.|
|num_of_applicants|*int*|pub_act_prcntile_by_st_score|The number of university applicants that for each public state university.|
|acceptance_rate|*float*|pub_act_prcntile_by_st_score|The percentage of students accepted based on the number of applicants|
|tot_percentile25|*int*|pub_act_prcntile_by_st_score|The total 25% percentile, 25% of accepted students at public universities scored at or below on the listed composite score |
|tot_percentile75|*int*|pub_act_prcntile_by_st_score|The total 75% percentile, 75% of accepted students at public universities scored at or below on the listed composite score |
|pub_school_state|*object*|pub_act_prcntile_by_st_score|This is the state of each 4 year public university(duplicates within this column mean that multiple public school information avaliable for that school).|

---
## Conclusions and Recommendations
Based on my exploration of the data, the lower average percentile range for students accepted into public universities is higher than the national average ACT score in the US. This is too say that students interested in applying to public universities have to work to ensure they are performing higher than the ACT test taker in the US. So the safety schools(their in state public universities) they will be seeking to apply to will more than likely need to an average composite ACT score that is above the national anywhere from 2 to 7 points.More specifically summarizing this with values is that the 25th percentilea nd 75th percentilen respectively was found to be (22.9, 28.89). This range is just above the typical to national average,21.5, that I was able to gather fom my own data set and reasearch found online for in my National ACT Averages (Outside Research Section).

There are a fair amount of future recommendations to explore to determine if this conclusion can be truly determined:
- Gathering a more accurate dataset:
    - If a dataset contained various public universities per state and had measure of the average (50% percentile) of accected applicants then an accurate state/national level analysis could be determined.
- Explore the relationship of universities (accepts rates vs act score) follow the same trends as private?
- For those states that have favor or hold SAT policies for high school graduates what is that basis score?
 - For public universities what does the average composite score look like at a state level? Could then begin to advise local students looking to determine thir safety schools.


## Data Sources
* [`act_2017.csv`](./data/act_2017.csv): 2017 ACT Scores by State ([source](https://blog.prepscholar.com/act-scores-by-state-averages-highs-and-lows))
* [`act_2018.csv`](./data/act_2018.csv): 2018 ACT Scores by State ([source](https://blog.prepscholar.com/act-scores-by-state-averages-highs-and-lows))
* [`act_2019.csv`](./data/act_2019.csv): 2019 ACT Scores by State ([source](https://blog.prepscholar.com/act-scores-by-state-averages-highs-and-lows))
* [`sat_act_by_college.csv`](./data/sat_act_by_college.csv): Ranges of Accepted ACT & SAT Student Scores by Colleges ([source](https://www.compassprep.com/college-profiles/))
