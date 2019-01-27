# Alzheimer’s Analysis
### Introduction
#### About Dementia
Dementia is not a specific disease. It’s an overall term that describes a group of symptoms associated with a decline in memory or other thinking skills severe enough to reduce a person’s ability to perform everyday activities. Alzheimer’s disease accounts for 60 to 80 percent of cases. Vascular dementia, which occurs after a stroke, is the second most common dementia type. But there are many other conditions that can cause symptoms of dementia, including some that are reversible, such as thyroid problems and vitamin deficiencies.

Dementia is a general term for loss of memory and other mental abilities severe enough to interfere with daily life. It is caused by physical changes in the brain. Alzheimer's is the most common type of dementia, but there are many kinds.

### Alzheimer
- Alzheimer's is a type of dementia that causes problems with memory, thinking and behavior. Symptoms usually develop slowly and get worse over time, becoming severe enough to interfere with daily tasks. 


- Alzheimer's is not a normal part of aging. The greatest known risk factor is increasing age, and the majority of people with Alzheimer's are 65 and older. But Alzheimer's is not just a disease of old age. Approximately 200,000 Americans under the age of 65 have younger-onset Alzheimer’s disease (also known as early-onset Alzheimer’s). 


- Alzheimer's is the sixth leading cause of death in the United States. Those with Alzheimer's live an average of eight years after their symptoms become noticeable to others, but survival can range from four to 20 years, depending on age and other health conditions. 


- Alzheimer's has no current cure, but treatments for symptoms are available and research continues. Although current Alzheimer's treatments cannot stop Alzheimer's from progressing, they can temporarily slow the worsening of dementia symptoms and improve quality of life for those with Alzheimer's and their caregivers. Today, there is a worldwide effort under way to find better ways to treat the disease, delay its onset, and prevent it from developing.

### Understanding the data
> **Summary**: This set consists of a longitudinal collection of 150 subjects aged 60 to 96. Each subject was scanned on two or more visits, separated by at least one year for a total of 373 imaging sessions. For each subject, 3 or 4 individual T1-weighted MRI scans obtained in single scan sessions are included. The subjects are all right-handed and include both men and women. 72 of the subjects were characterized as nondemented throughout the study. 64 of the included subjects were characterized as demented at the time of their initial visits and remained so for subsequent scans, including 51 individuals with mild to moderate Alzheimer’s disease. Another 14 subjects were characterized as nondemented at the time of their initial visit and were subsequently characterized as demented at a later visit.

#### Dataset Description

- We will be using the longitudinal MRI data.
- The dataset consists of a longitudinal MRI data of 150 subjects aged 60 to 96.
- Each subject was scanned at least once.
- Everyone is right-handed.
- 72 of the subjects were grouped as 'Nondemented' throughout the study.
- 64 of the subjects were grouped as 'Demented' at the time of their initial visits and remained so throughout the study.
- 14 subjects were grouped as 'Nondemented' at the time of their initial visit and were subsequently characterized as 'Demented' at a later visit. These fall under the 'Converted' category.

| COL  | Description                         |
|------|-------------------------------------|
| EDUC | Years of Education                  |
| SES  | Socioeconomic Status                |
| MMSE | Mini Mental State Examination       |
| CDR  | Clinical Dementia Rating            |
| eTIV | Estimated Total Intracranial Volume |
| nWBV | Normalize Whole Brain Volume        |
| ASF  | Atlas Scaling Factor                |

### Mini–Mental State Examination (MMSE)
> The Mini–Mental State Examination (MMSE) or Folstein test is a 30-point questionnaire that is used extensively in clinical and research settings to measure cognitive impairment. It is commonly used in medicine and allied health to screen for dementia. It is also used to estimate the severity and progression of cognitive impairment and to follow the course of cognitive changes in an individual over time; thus making it an effective way to document an individual's response to treatment. The MMSE's purpose has been not, on its own, to provide a diagnosis for any particular nosological entity.
> - **Cognitive Impairment:** Cognitive impairment is when a person has trouble remembering, learning new things, concentrating, or making decisions that affect their everyday life. Cognitive impairment ranges from mild to severe.

> Any score greater than or equal to 24 points (out of 30) indicates a normal cognition. Below this, scores can indicate severe (≤9 points), moderate (10–18 points) or mild (19–23 points) cognitive impairment. The raw score may also need to be corrected for educational attainment and age. That is, a maximal score of 30 points can never rule out dementia.


|   **Method**  |**Score**|  **Interpretation**                   |                   
|---------------|---------|--------------------------------------|
| Single Cutoff |   <24   |        Abnormal                      |
|     Range     |   <21   |  Increased Odds of Dementia          |
|               |   <25   |  Decreased Odds of Dementia          |
|   Education   |    21   |  Abnormal for 8th Grade Education    |
|               |   <23   |  Abnormal for High School Education  |
|               |   <24   |  Abnormal for College Education      |
|   Severity    |  24-30  |  No Cognitive Impairment             |
|               |  18-23  |  Mild Cognitive Impairment           |
|               |   0-17  |  Severe Cognitive Impairment         |

### Clinical Dementia Rating (CDR)
> The CDR is a 5-point scale used to characterize six domains of cognitive and functional performance applicable to Alzheimer disease and related dementias: Memory, Orientation, Judgment & Problem Solving, Community Affairs, Home & Hobbies, and Personal Care. The necessary information to make each rating is obtained through a semi-structured interview of the patient and a reliable informant or collateral source (e.g., family member).<br><br>
> The CDR table provides descriptive anchors that guide the clinician in making appropriate ratings based on interview data and clinical judgment. In addition to ratings for each domain, an overall CDR score may be calculated through the use of an algorithm. This score is useful for characterizing and tracking a patient's level of impairment/dementia:

| Score  | Description               |
|--------|---------------------------|
|    0   |        Normal             |
|    0.5 | Very Mild Dementia        | 
|    1   | Mild Dementia             |
|    2   | Moderate Dementia         |
|    3   | Severe Dementia           |=

###  Estimated Total Intracranial Volume(eTIV)
> Total intracranial volume (TIV/ICV) is an important covariate for volumetric analyses of the brain and brain regions, especially in the study of neurodegenerative diseases, where it can provide a proxy of maximum pre-morbid brain volume.<br><br>
> 1. > Unlike brain atrophy in the patients with AD, TIV did not vary over time. Mean TIV did not differ significantly between any of the subject groups. There was no association between TIV and age or age at symptom onset. The only significant predictor of TIV was sex. Men showed an approximately ∼12% larger eTIV than women. 

> 2. > We measured TIV with a semiautomated segmentation technique on T1- and T2-weighted MR images in 55 controls, 10 AD patients, and two persons at risk of familial AD. Whole-brain volumes also were measured and normalized with TIVs.

> 3. > The TIV normalization of cross-sectional brain volumes significantly reduced interindividual variation; the coefficient of variation (CV) was reduced from 10.0% to 6.0% in controls (P <.001). The TIVs measured on T1-weighted images had low variability (CV, 0.16%) and did not differ significantly from those measured on T2-weighted images (P =.16). The TIV normalization of serial brain-volume measurements reduced interimage differences caused by voxel-scaling variations (CV reduced from 1.3% to 0.5%, P =.002) in 10 controls and five AD patients.

### Atlas Scaling Factor   (ASF)
A unified approach for morphometric and functional data analysis in young, old, and demented adults using automated atlas-based head size normalization: reliability and validation against manual measurement of total intracranial volume.

Basically, total intracranial volume is found to correlate with the determinant of the transform matrix used to align an image with an atlas. The work demonstrates that a one-parameter scaling factor provides a reasonable TIV estimation
