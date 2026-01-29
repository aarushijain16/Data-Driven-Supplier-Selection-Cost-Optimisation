# Data-Driven Supplier Selection & Cost Optimisation
## *Analytics project focused on building a model-ready data foundation for cost-efficient sourcing decisions*

# Overview

This project demonstrates how data engineering and feature optimisation can enable smarter, cost-driven supplier selection in complex procurement environments.

Working with a simulated dataset for Acme Corporation, I built a robust data preparation and feature engineering pipeline to transform raw transactional, task, and supplier data into a clean, model-ready dataset for supplier cost optimisation.

Using:

- Multi-source data integration (tasks, suppliers, costs)

- Feature selection using variance and correlation analysis

- Feature scaling and normalisation for ML readiness

- Exploratory analysis to validate data quality and structure

The goal was to create a reliable analytical foundation that supports predictive supplier recommendation, improves cost transparency, and enables data-driven sourcing decisions instead of intuition-based selection.

# Business Problem

Acme Corporation faced challenges in selecting the most cost-effective suppliers for a wide range of operational tasks:

- Supplier selection relied heavily on manual judgement

- High-dimensional task and supplier data made comparison difficult

- No standardised framework to evaluate supplier–task cost efficiency

- Poor data readiness for predictive or optimisation models

Key questions addressed:

- How can supplier performance be evaluated consistently across tasks?

- Which task and supplier features actually matter for cost optimisation?

- How can raw operational data be transformed into model-ready inputs?

- How can procurement move from reactive decisions to predictive sourcing?

# Solution Approach

I designed a structured, end-to-end data engineering and feature optimisation pipeline to support future supplier recommendation models.

🔹 Data Ingestion & Quality Validation

- Integrated three datasets: task data, supplier data, and task-supplier cost data

- Performed structural validation using schema checks and data profiling

- Identified and removed duplicate records to ensure data integrity

- Confirmed completeness (no missing values across datasets)

🔹 Data Transformation & Integration

- Standardised inconsistent Task ID formats across datasets

- Unified all Task IDs into a consistent date-based format

- Merged task, supplier, and cost data into a consolidated analytical table

- Removed records without valid cost linkage to ensure modelling relevance

🔹 Feature Selection – Variance Filtering

- Evaluated variability across 116 task features

- Removed low-variance features below a defined threshold

- Reduced noise while retaining informative task characteristics

- Supplier features retained due to sufficient variability

🔹 Feature Scaling & Normalisation

- Applied Min-Max scaling to all numerical features

- Normalised values to a consistent range (-1 to 1)

- Ensured fair feature contribution during future model training

🔹 Feature Selection – Correlation Filtering

- Performed correlation analysis on task features

- Identified highly correlated feature pairs

- Removed redundant features to reduce multicollinearity

- Reduced task features from 116 → 19 robust, independent features

# Key Business Insights and Strategic Impact

*(Translated for procurement, operations, and analytics teams)*

- High-dimensional operational data hides true cost drivers
 → Feature reduction improves clarity and decision quality

- Redundant and correlated features weaken model reliability
 → Correlation filtering improves interpretability and robustness

- Normalised features are critical for fair supplier comparison
 → Prevents scale-driven bias in predictive models

- Data preparation is the biggest bottleneck in analytics adoption
 → Strong foundations unlock faster, more accurate optimisation models

This project converts raw procurement data into a strategic analytical asset.

# Strategic Recommendations

- Establish a standardised data pipeline for supplier evaluation

- Use feature-optimised datasets as inputs for supplier recommendation models

- Integrate cost prediction into procurement planning workflows

- Reduce reliance on manual judgement for supplier selection

- Treat data engineering as a core capability, not a one-time task

# Tools and Technologies

- Python

- pandas, NumPy – data cleaning, transformation, integration

- scikit-learn – feature scaling, variance filtering, correlation analysis

- matplotlib / seaborn – exploratory analysis and correlation heatmaps

# Why this Matters for Operations & Analytics Teams

This project shows how analytics can:

- Enable predictive, cost-efficient sourcing

- Improve supplier comparison transparency

- Support scalable procurement decision-making

- Lay the groundwork for optimisation and ML models

The same approach applies to:

- Procurement & sourcing analytics

- Vendor management systems

- Cost optimisation initiatives

- Supply chain decision support

# 📌 Note

This project is based on a confidential, university-provided dataset.

Raw data and full implementation code are not shared publicly.

The repository focuses on methodology, decision logic, and business impact.

# 💬 How I Can Help You

If your organisation wants to:

- Optimise supplier selection using data

- Reduce sourcing costs through predictive analytics

- Build model-ready procurement datasets

- Move from intuition-led to analytics-led sourcing

I can help design data pipelines, feature engineering frameworks, and analytics solutions tailored to your procurement data.
