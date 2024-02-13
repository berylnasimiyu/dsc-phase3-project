# Water Wells Classification Project

Group 15 DSF-PT05
Members
1.Sophie Hare-Lead
2.James Kibunja
4.Beryl Wafula
5.John Nkakuyia
6.Daniel Murithi

## Project Overview
This project aims to address a classification problem related to water wells in Tanzania. The goal is to predict the condition of water wells, categorizing them as functional, non-functional, or in need of repair. The analysis and models developed in this project will assist stakeholders, such as NGOs or the Government of Tanzania, in identifying wells that require attention and maintenance.

## Business and Data Understanding
### Stakeholder Audience:
The primary stakeholders for this project are organizations involved in providing clean water access, including NGOs and the Government of Tanzania. The model's predictions will help prioritize well maintenance efforts and allocate resources effectively.

### Dataset Choice:
The dataset used for this analysis is a combination of two files: d.3.csv and d.1.csv. It contains various features related to water wells, such as pump type, installation date, and other relevant information. The dataset was chosen to address the specific needs of predicting well conditions.

### Target Variable:
status_group: The functionality status of the water pump (target variable). Categories may include "functional," "non-functional," or "functional needs repair."

**Overview:**

Tanzania, the largest country in East Africa with a population of approximately 59 million, grapples with challenges in providing clean water to its citizens. Approximately 47% of the population lacks access to clean drinking water, and many existing water points require repairs or have failed. The project's primary objective is to build a classifier for two key audiences:

1. **Government of Tanzania:**
   - Identify patterns in non-functional wells.
   - Understand factors influencing well failure to improve the construction of new wells.
   - Enhance the longevity and functionality of wells.

2. **Resource Allocation Optimization:**
   - Identify non-functional and in-need-of-repair wells to optimize resource allocation.
   - Maximize impact in providing clean water access.

**Objective:**

Tanzania faces water provision challenges due to issues with existing water points, with some wells needing repairs or failing entirely. The analysis aims to:
- Understand factors affecting well functionality (e.g., water source, well age, and the impact of public meetings).
- Determine the best payment mode for well maintenance.
- Utilize classification methods to identify effective strategies for improving well functionality. 

This analysis supports the Government Ministry of Water and NGOs in their efforts to ensure clean water access for Tanzanian communities.

**Data Understanding:**

Data was obtained from the Taarifa waterpoints dashboard which aggregates data from the Tanzania Ministry of Water. The data collected contains features related to water pumps such as geographic location, water quality, organizations that build and manage them, and population among others. The target feature is a 'status group with three possible values functional, non-functional, and functional-need-repairs.


**Age vs Functionality:**

The analysis explores the relationship between well age and functionality.

**Modeling:**

Three models were employed: XGBoost, LinearSVC, and RandomForest. XGBoost demonstrated the highest accuracy and precision, making it the chosen model.

**Evaluation:**

XGBoost emerged as the best-performing model, providing high accuracy and precision values.

**Findings:**

1. **Dependency on Groundwater:**
   - Groundwater plays a critical role in maintaining well functionality, serving as the primary water source for wells.

2. **Sustainability Measures:**
   - Exploring alternative methods such as rainwater harvesting and soil conservation is crucial to sustain more water in lakes, supporting overall water access.

3. **Payment Impact:**
   - Payment methods significantly influence well maintenance. Wells subjected to payment based on a bucket or monthly payments tend to be better maintained.

4. **Age as a Predictor:**
   - The age of wells proves to be a vital predictor of functionality. Newer wells generally have higher water supply and better overall condition.

5. **Public Meetings Influence:**
   - Public meetings play a substantial role in well functionality, with more than 50% of wells being functional when public meetings are held. This emphasizes the importance of community engagement.

6. **Model Recommendation:**
   - XGBoost emerged as the best-performing model, showcasing high accuracy and precision in predicting well functionality.

**Conclusion and Recommendations:**

- **Conclusion:**
  - Groundwater is vital for well functionality.
  - Payment methods, especially monthly or bucket-based, contribute to improved well maintenance.
  - Well age is a key factor, with newer wells generally in better condition.
  - Public meetings significantly impact well functionality.

- **Recommendations:**
  - Explore sustainable methods like rainwater harvesting and soil conservation.
  - Implement payment systems based on buckets or monthly payments for improved well maintenance.
  - Consider well age in planning and construction for better functionality.
  - Encourage and organize public meetings to enhance well functionality.
  - Establish designated inspections for pumps identified by the model.
  
**Future Work:**

- **Data Examination:**
  - Investigate missing or zero values in Population and GPS.
  - Explore binning highly cardinal columns for enhanced model performance.
  - Examine and address wells with static head values of 0.
