# Heavy Machinery Predictive Maintenance Model ⚙️

**Interactive Data Analytics & Machine Learning Pipeline**

## Project Overview
Equipment failure in heavy industrial operations can cost millions of dollars in downtime and safety hazards. This project builds a machine learning model to predict catastrophic machinery failures before they happen by analyzing real-time sensor data (Torque, Rotational Speed, Temperature, and Tool Wear). 

## Tech Stack
* **Language:** Python
* **Data Manipulation:** Pandas
* **Machine Learning:** Scikit-Learn (Random Forest)
* **Data Engineering:** Imbalanced-Learn (SMOTE)
* **Interactive Visualization:** Plotly

## The Challenge & Solution
* **The Problem (Class Imbalance):** Because heavy machinery rarely breaks down, the initial model suffered from the "Accuracy Trap." It achieved 98% accuracy by simply guessing that no machine would ever break, completely missing the actual failures.
* **The Solution (SMOTE):** I engineered a balanced dataset using the **Synthetic Minority Over-sampling Technique (SMOTE)**. By generating highly realistic synthetic failure data for the training set, I forced the algorithm to recognize the failure patterns, successfully increasing the critical failure detection rate (Recall) by nearly 40%.

## Key Business Insights
1. **Interactive Risk Mapping:** Deployed Plotly scatter maps to isolate the "Danger Zones" of machine operation. 
2. **Operational Boundaries:** The data proves that failures are not random. The vast majority of catastrophic failures occur during extreme imbalances between Rotational Speed and Torque (e.g., high torque at low speeds).
3. **Preventative Action:** By actively monitoring these specific operational boundaries, field engineers can halt operations for maintenance before the physical breaking point is reached. <img width="997" height="647" alt="image" src="https://github.com/user-attachments/assets/8e8945f0-8313-452a-a710-fbf769c40f00" />


## View the Project
Click on the `Predictive_Maintenance.ipynb` file above to view the complete code, the SMOTE implementation, and the interactive Plotly visualizations.
