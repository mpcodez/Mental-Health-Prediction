# Mental Health and Socioeconomic Status Analysis

## Authors  
- Medha Pappula  
- Kade Yen  

## Class  
- Machine Learning 1  

## Instructor  
- Dr. Yilmaz  

## Project Overview  
This project investigates the impact of socioeconomic factors on mental health outcomes among adults in the United States. Using the 2023 National Health Interview Survey (NHIS) dataset from the CDC, we analyze key socioeconomic attributes and their correlation with mental health conditions. Our goal is to provide insights that can guide policy interventions and resource allocation.

## Research Question  
**What specific socioeconomic factors among adults in the United States have a profound impact on mental health outcomes?**  

## Dataset  
- **Source:** [2023 National Health Interview Survey (NHIS)](https://www.cdc.gov/nchs/nhis/2023nhis.htm)  
- **Size:** 29,522 rows, 647 attributes  
- **Relevant Attributes:**  
  - PHQ41_A, PHQ42_A, PHQ43_A, PHQ44_A (Brief Mental Health Assessment)  
  - Various socioeconomic indicators (education level, income, employment status, etc.)

## Preprocessing Pipeline  
1. **Removing Irrelevant Attributes:**  
   - Discarded ~550-600 attributes to improve correlation and model efficiency.  
   - Maintained ~336 key attributes.  

2. **Handling Missing Data:**  
   - Removed attributes with >70% missing values.  
   - Replaced missing values with default values using Weka’s ReplaceMissingWithUserConstant feature.  

3. **Feature Engineering (Class Attribute Creation):**  
   - Combined PHQ41_A, PHQ42_A, PHQ43_A, and PHQ44_A to create a mental health classification label.  
   - Applied thresholding and averaging to categorize mental health status.  

4. **Normalization:**  
   - Adjusted skewed numeric attributes by dividing values by their max range.  

## Methodology  
- **Data Cleaning & Processing:** Pandas, Weka  
- **Model Training:** Machine Learning classification on engineered attributes  
- **Tools Used:**  
  - Python (Pandas, NumPy)  
  - Weka for attribute selection and missing value handling  

## How to Use  
1. **Download the latest NHIS dataset from [CDC](https://www.cdc.gov/nchs/nhis/2023nhis.htm).**  
2. **Preprocess the data using the same pipeline outlined above.**  

## Additional Resources  
- **Final Research Paper:** [paper.pdf](./finalReport.pdf)  
- **Presentation Slides:** [slides.pdf](./slides.pdf)  
