# Hospital_Readmission_Risk_analysis

# <p align="center">Hospital Readmission Risk Analysis</p>
# <p align="center">![Pic](https://cdn-icons-png.flaticon.com/512/1802/1802511.png)</p>

## Business Problem: 
# Why Do Patients Come Back? A Hospital Readmission Story

Every hospital has a quiet worry: the patient who gets discharged, goes home, and returns a few weeks later. Readmissions are costly for hospitals and hard on patients. I wanted to find out who is most at risk of coming back.

## The Data
I worked with records from 130 US hospitals spanning 1999 to 2008, about 100,000 inpatient stays. Each row is one hospital visit: who the patient was, how long they stayed, what treatment they got, and whether they returned.

Data Source: [Diabetes 130-US Hospitals (UCI)](https://archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008)

## The Investigation
Using SQL, I asked a few simple questions:
- How often do patients actually return within 30 days?
- Does age or length of stay make a difference?
- Do patients with more prior visits come back more often?
- Which patients should hospitals prioritize for follow-up care?


## Findings
1. **Circulatory and diabetes diagnoses** had the **highest readmission rates** among all diagnosis categories, and both exceeded the average readmission rate.
2. Patients with **more prior inpatient visits** in the prior year showed a substantially elevated readmission risk, supporting prior-utilization as a strong predictive signal.
3. **Discharge disposition mattered significantly**. Patients discharged to certain facility types showed measurably different readmission rates than those discharged home.
4. Findings around **medication changes at discharge and A1C testing** during the stay both align with the original clinical research question this dataset was collected to investigate.

## Recommendations
- Focus discharge planning and follow-up on patients with the highest risk based on past hospital visits.
- Give extra care coordination to patients with heart/circulatory conditions and diabetes, given they have higher readmission rates.
- Review discharge processes at facilities with high readmission rates to find areas that could be improvedn-wide average
- Multi-table joins against ID-mapping reference tables to convert numeric codes into readable labels
