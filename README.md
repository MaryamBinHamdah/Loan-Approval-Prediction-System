# 💳 Loan Approval Prediction: A Data-Driven Approach to Credit Risk

<p align="center">
  <a href="https://public.tableau.com/views/FinalGraph_17638895054630/Story1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link" target="_blank">
    <img src="https://github.com/HesKal/Loan-Approval-Prediction-System/blob/main/4_Tableau_Dashboard/Dashboard_Preview.jpg?raw=true" alt="Tableau Dashboard Preview" width="90%"/>
  </a>
    

  <em>An interactive Tableau dashboard created to visualize key findings. Click the image to explore the live dashboard.</em>
</p>

## 🌟 Business Problem & Objective

In the competitive financial services industry, accurately assessing credit risk is fundamental to profitability and survival. Lending institutions face a dual challenge: minimizing losses from loan defaults while not being overly cautious and rejecting creditworthy applicants.

This project tackles this problem by developing a data-driven solution for a Credit Risk Manager. The core objective is to build a machine learning model that can **accurately predict loan approval status**, thereby automating the initial screening process, reducing financial risk, and improving decision-making efficiency.

---

## 📊 Data Source

The analysis for this project was conducted using the **Loan Approval Prediction Dataset**, a publicly available dataset from Kaggle.

*   **Source:** Kaggle
*   **Dataset Link:** [Loan Approval Prediction Dataset](https://www.kaggle.com/datasets/architsharma01/loan-approval-prediction-dataset )
*   **Owner/Author:** Archit Sharma

*Giving credit to the original data source is a fundamental aspect of ethical data science practice.*

---

## 🚀 The CRISP-DM Journey: A Methodical Approach

We adopted the **Cross-Industry Standard Process for Data Mining (CRISP-DM)** to structure our project, ensuring a comprehensive and business-focused workflow from start to finish.

<details>
<summary><strong>Click to see how we mapped our project to the CRISP-DM phases</strong></summary>

| Phase (CRISP-DM) | What We Did in This Project |
| :--- | :--- |
| **Business Understanding** | Defined the problem of credit risk, identified the Credit Risk Manager as the key stakeholder, and set the objective to predict loan defaults. |
| **Data Understanding** | Sourced the "Loan Approval Prediction Dataset" from Kaggle and performed Exploratory Data Analysis (EDA) in Tableau to discover initial patterns, such as the strong correlation between `cibil_score` and `loan_status`. |
| **Data Preparation** | Cleaned the dataset (verified no missing values), transformed categorical features (e.g., `education`) into numerical format for Logistic Regression, and removed the non-predictive `loan_id` attribute. |
| **Modeling** | Built and trained two distinct classification models in AI Studio: a **Decision Tree** and a **Logistic Regression** model, using a 70/30 train-test split. |
| **Evaluation** | Compared the models using Accuracy, Precision, and Recall. The **Decision Tree emerged as the superior model with 96.72% accuracy**. We also performed a detailed error analysis to understand the business impact of False Positives vs. False Negatives. |
| **Deployment** | For this project, deployment involved creating this comprehensive repository, a detailed written report, and an interactive **Tableau Dashboard and Storyboard** to communicate our findings and recommendations to business stakeholders. |

</details>

---

## 🔬 Model Development & Comparison

Two classification models were built to predict `loan_status`. The results clearly identified a winner.

| Model | Accuracy | Precision | Recall | Key Takeaway |
| :--- | :--- | :--- | :--- | :--- |
| 🌳 **Decision Tree** | **96.72%** | **97.37%** | **97.37%** | **Selected Model.** Superior performance and high interpretability ("white-box"). |
| 📈 **Logistic Regression**| 91.02% | 94.29% | 91.09% | Good baseline, but less accurate and produced more costly errors (especially False Negatives). |

The **Decision Tree** was chosen not only for its superior accuracy but also for its transparency, a critical feature in the finance industry where decisions must be explainable.

---

## 💡 Key Business Insights & Recommendations

Our analysis yielded several actionable insights:

1.  **CIBIL Score is King:** The applicant's credit score is the most dominant predictor of the loan outcome.
2.  **Income Sets Limits, It Doesn't Decide:** Income level was not a primary driver for approval, but rather determined the maximum loan amount.
3.  **Demographics Have Minimal Impact:** Factors like education and employment status had a negligible effect on the final decision in this dataset.

Based on this, we recommended the deployment of the Decision Tree model as an **automated pre-screening tool** to fast-track high-quality applications and automatically flag high-risk ones, allowing human analysts to focus on "borderline" cases where their expertise is most valuable.

---

## 🛠️ Technologies & Skills

*   **Data Mining & ML:** `Classification (Decision Tree, Logistic Regression)`, `Model Evaluation (Confusion Matrix, Accuracy, Precision, Recall)`, `CRISP-DM Methodology`
*   **Data Visualization & Storytelling:** `Tableau`
*   **Design & Presentation:** `Canva`
*   **Core Platform:** `AI Studio`
*   **Version Control:** `Git`, `GitHub`
*   **Core Skills:** `Business Acumen`, `Data-Driven Decision Making`, `Exploratory Data Analysis (EDA)`, `Feature Selection`

---

## 📂 Project Files & Live Demo

*   **[`1_Model_Development/`](./1_Model_Development):** Contains screenshots and diagrams of the AI Studio workflows for both models.
*   **[`2_Dataset/`](./2_Dataset):** Contains the raw `Loan_Approval_Prediction_Dataset.csv` file.
*   **[`3_Documentation/`](./3_Documentation):** Contains the final detailed project report and presentation.
*   **[`4_Tableau_Dashboard/`](./4_Tableau_Dashboard):** Contains screenshots and a link to the live, interactive dashboard.

> **[🔗 Click here to explore the live Tableau Dashboard!](https://public.tableau.com/views/FinalGraph_17638895054630/Story1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link )**

---

## 👥 The Team

This project was a successful collaboration between:

*   **Hessa Khalfan** ([@Heskal](https://github.com/Heskal ))
*   **Nourah Alghfeli** ([@NourahAlghfeli](https://github.com/NourahAlghfeli ))
*   **Maryam BinHamdah** ([@MaryamBinHamdah](https://github.com/MaryamBinHamdah ))

*   My Role: Focused on advanced visualizations in Tableau (Stacked Bars, Box Plots) and was responsible for designing the final PowerPoint presentation.


## 📜 License

This project is licensed under the **MIT License**. See the `LICENSE` file for details.
