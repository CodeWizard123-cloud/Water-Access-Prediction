# 💧 Water Access Prediction using IBM watsonx.ai AutoAI

This project uses **IBM watsonx.ai’s AutoAI** to automatically generate machine learning pipelines to predict **water access** levels across different demographics and sectors in India. The prediction is based on simple yet powerful features such as **state**, **age group**, **sector**, **gender**, and **indicator type**.

---

## 🎯 Project Objective

To build a predictive model that can estimate **levels of access to water** (e.g., sufficient, inadequate, no access) for different groups of people using **demographic and categorical features**. This supports improved planning, targeting of water resources, and policy interventions.

---

## 📦 Dataset Description

The dataset contains the following columns:

| Feature        | Description                              |
|----------------|------------------------------------------|
| `State`        | Indian state/region                      |
| `Age_Group`    | Age group of the individuals             |
| `Sector`       | Urban or Rural sector                    |
| `Gender`       | Gender group: Male / Female              |
| `Indicator`    | Type of indicator (related to water access) |
| `Access_Level` | **Target Variable** – Level of water access (e.g., Adequate, Low, None)

---

## 🧠 Tools Used

| Component       | Technology Used                  |
|----------------|----------------------------------|
| Platform        | IBM watsonx.ai (AutoAI tool)     |
| Model Builder   | AutoAI (automated ML pipeline builder) |
| Language        | Auto-generated Python (via notebooks) |
| Data Format     | CSV                              |

---

## 🛠️ Steps to Run the Project

### Using IBM watsonx.ai:

1. Go to: [https://dataplatform.cloud.ibm.com](https://dataplatform.cloud.ibm.com)
2. Create a new project.
3. Upload the notebook `WaterAccessAutoAI.ipynb` as an asset.
4. Upload the dataset (e.g., `water_access_data.csv`) as a **Data Asset**.
5. Open the notebook and click **"Run in AutoAI"**.
6. AutoAI will:
   - Clean and preprocess your data
   - Encode categorical variables (e.g., Gender, Sector)
   - Select top-performing ML pipelines
   - Display leaderboard of models with performance metrics

---

## 📈 Model Output

AutoAI selects the best pipeline based on a scoring metric (e.g., Accuracy or F1-score).

| Metric        | Value (Example)   |
|---------------|------------------|
| Accuracy      | 82.5%             |
| F1-score      | 81.3%             |
| Best Pipeline | XGBoost Classifier or Voting Ensemble |

---

## 🔍 Key Features Considered

All features are **categorical**:
- State
- Age Group
- Gender
- Sector (Urban/Rural)
- Indicator Type

Target variable: **Access_Level**

---

## 🔬 Research References

The following resources were used for background research and methodology inspiration:

1. **"Machine Learning for Public Health"**, Elsevier, 2020  
2. **"AI for Sustainable Development Goals (SDGs)"**, Nature, 2022  
3. **"Water Accessibility Modeling Using Machine Learning"**, IJAEGT, 2021  
4. **IBM AutoAI Documentation**: [https://www.ibm.com/cloud/watson-studio/autoai](https://www.ibm.com/cloud/watson-studio/autoai)  
5. India Water Portal & Census Reports for demographic trends

---

## 💬 Challenges Faced

- Entire dataset composed of **categorical variables** → encoding needed.
- Some indicator values were **inconsistent** or had overlapping meanings.
- Balancing the **class distribution** of Access_Level categories.

---

## 🚀 Future Enhancements

- Incorporate **temporal data** (year-wise analysis).
- Deploy model using **Streamlit or Flask** for public access.
- Connect to **live dashboards** (e.g., Tableau, Power BI).
- Integrate **mobile-based reporting** for rural surveys.

---

## 📌 Folder Structure

