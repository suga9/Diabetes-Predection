# Diabetes Prediction 🩺

## Overview
Diabetes is a chronic health condition that affects how your body turns food into energy. This project aims to predict the onset of diabetes based on diagnostic measures.

## Types of Diabetes
There are two main types of diabetes:

### Type I Diabetes
Type 1 Diabetes occurs when your immune system mistakenly attacks and destroys the insulin-producing cells in your pancreas. This results in little to no insulin production, leading to high blood sugar levels. It is usually diagnosed in children and young adults and requires lifelong insulin therapy for management.

**Key Point:** In Type 1, the pancreas produces no or low insulin.

### Type II Diabetes
In Type 2 Diabetes, your body either resists the effects of insulin or doesn't produce enough insulin to maintain normal glucose levels. This is the most common type of diabetes and is often associated with lifestyle factors such as obesity, lack of physical activity, and unhealthy eating habits. It can often be managed with lifestyle changes, oral medications, and insulin therapy if needed.

**Key Point:** In Type 2, body cells respond poorly or do not absorb enough sugar.

**In this project,** 
our primary focus is on Type 2 Diabetes. The dataset we are utilizing encompasses a variety of metrics specifically related to Type 2 Diabetes. This will enable us to delve deeper into the nuances of this condition and potentially uncover meaningful patterns and insights.


## How Is Diabetes Diagnosed?

| Test | Value for Diagnosis |
| --- | --- |
| Fasting Plasma Glucose | ≥ 126 mg/dL |
| Oral Glucose Tolerance | ≥ 200 mg/dL |
| Glycated Hemoglobin (A1C) | ≥ 6.5% |

## Dataset:
https://data.mendeley.com/datasets/wj9rwkp9c2/1 Rashid, Ahlam (2020), “Diabetes Dataset”, Mendeley Data, V1, doi: 10.17632/wj9rwkp9c2.1

The data consist of medical information, laboratory analysis… etc. The data that have been entered initially into the system are: No. of Patient, Sugar Level
Blood, Age, Gender, Creatinine ratio(Cr), Body Mass Index (BMI), Urea, Cholesterol (Chol), Fasting lipid profile, including total, LDL, VLDL, Triglycerides(TG) and 
HDL Cholesterol , HBA1C, Class (the patient's diabetes disease class may be Diabetic, Non-Diabetic, or Predict-Diabetic).

## Sample Dataset:

**df = pd.read_csv('/content/file_downloaded')
df**

|index|ID|No\_Pation|Gender|AGE|Urea|Cr|HbA1c|Chol|TG|HDL|LDL|VLDL|BMI|CLASS|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|0|502|17975|F|50|4\.7|46|4\.9|4\.2|0\.9|2\.4|1\.4|0\.5|24\.0|N|
|1|735|34221|M|26|4\.5|62|4\.9|3\.7|1\.4|1\.1|2\.1|0\.6|23\.0|N|
|2|420|47975|F|50|4\.7|46|4\.9|4\.2|0\.9|2\.4|1\.4|0\.5|24\.0|N|
|3|680|87656|F|50|4\.7|46|4\.9|4\.2|0\.9|2\.4|1\.4|0\.5|24\.0|N|
|4|504|34223|M|33|7\.1|46|4\.9|4\.9|1\.0|0\.8|2\.0|0\.4|21\.0|N|
|5|634|34224|F|45|2\.3|24|4\.0|2\.9|1\.0|1\.0|1\.5|0\.4|21\.0|N|
|6|721|34225|F|50|2\.0|50|4\.0|3\.6|1\.3|0\.9|2\.1|0\.6|24\.0|N|
|7|421|34227|M|48|4\.7|47|4\.0|2\.9|0\.8|0\.9|1\.6|0\.4|24\.0|N|
|8|670|34229|M|43|2\.6|67|4\.0|3\.8|0\.9|2\.4|3\.7|1\.0|21\.0|N|
|9|759|34230|F|32|3\.6|28|4\.0|3\.8|2\.0|2\.4|3\.8|1\.0|24\.0|N|
|10|636|34231|F|31|4\.4|55|4\.2|3\.6|0\.7|1\.7|1\.6|0\.3|23\.0|N|

## Dataset Description

**df.info()**

- Class: `pandas.core.frame.DataFrame`
- Range Index: 1000 entries from 0 to 999
- Total Columns: 14
    - Data types: float64(8), int64(4), object(2)
- Memory Usage: 109.5+ KB
  

The dataset used in this project has the following structure:

| # | Column | Non-Null Count | Dtype |
| --- | --- | --- | --- |
| 0 | ID | 1000 non-null | int64 |
| 1 | No_Pation | 1000 non-null | int64 |
| 2 | Gender | 1000 non-null | object |
| 3 | AGE | 1000 non-null | int64 |
| 4 | Urea | 1000 non-null | float64 |
| 5 | Cr | 1000 non-null | int64 |
| 6 | HbA1c | 1000 non-null | float64 |
| 7 | Chol | 1000 non-null | float64 |
| 8 | TG | 1000 non-null | float64 |
| 9 | HDL | 1000 non-null | float64 |
| 10 | LDL | 1000 non-null | float64 |
| 11 | VLDL | 1000 non-null | float64 |
| 12 | BMI | 1000 non-null | float64 |
| 13 | CLASS | 1000 non-null | object |

Each row in the dataset represents a patient, and each column is a different feature related to the patient's health metrics or demographic information.



