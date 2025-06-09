
# 🧠 Alzheimer's Disease and Healthy Ageing Data Analysis

This project presents a comprehensive pipeline for exploring, cleaning, securing, and analyzing the **Alzheimer's Disease and Healthy Ageing Data**. The data-driven approach includes profiling, validation, privacy-preserving transformation, and role-based access control (RBAC) for secure sharing of insights.

## 📁 Repository Structure

The repository is organized into two main directories:

- `docs/` – Contains the project report and documentation files.
- `src/` – Contains the source code notebooks for data integrity analysis and RBAC implementation.

## 📊 Dataset Overview

The dataset includes:
- **Temporal & Spatial Coverage**: Multiyear and location-based insights into Alzheimer's prevalence.
- **Demographic Breakdown**: Age, gender, and other strata.
- **Confidence Intervals**: Low & high confidence limits for measured values.
- **Geolocation Info**: Latitude and longitude (obfuscated for privacy).

## ✅ Data Quality & Processing

**Key Challenges Addressed:**
- **Missing Values**: Imputed using mean (numerical) and mode (categorical).
- **Outliers**: Detected and handled to preserve statistical integrity.
- **Skewed Distributions**: Addressed to ensure validity for statistical modeling.

**Schema Validation**: A custom schema was defined to enforce data consistency.

**Privacy Measures**:
- Obfuscation and pseudonymization of sensitive fields.
- Tokenization and encryption for sensitive columns like `RowId`, `LocationDesc`, `Latitude`, and `Longitude`.

## 🔐 Role-Based Access Control (RBAC)

Implemented a flexible RBAC system to control access based on user roles:

| Role         | Accessible Data Columns                            |
|--------------|----------------------------------------------------|
| Data Analyst | Key statistical data and numerical insights        |
| Researcher   | Broader context including geographical breakdowns  |
| Admin        | Full access including metadata and sensitive fields|

Each user is assigned a role, and access is granted accordingly.

## 📈 Insights & Visualizations

- Histograms with KDE plots showed normal distribution after preprocessing.
- Pie and bar charts provided a demographic and regional overview.
- Class prevalence visualized per region to highlight disparities.
- Geographic analysis identified hotspots like **Tennessee** with high Alzheimer’s prevalence.

## 📌 Conclusions

- Cleaned and validated data is now reusable for **predictive modeling**.
- RBAC ensures **secure collaboration** among stakeholders.
- The structured approach lays a foundation for **ML-based health outcome predictions**.

## 🚀 Future Work

- Extend RBAC to support OAuth or external identity providers.
- Develop predictive models using location, demographics, and prevalence.
- Publish anonymized dataset for open research purposes.

## 📜 License

This project is for academic use. Data was modified for privacy and research integrity. Please refer to the dataset's original license for any usage beyond this scope.
