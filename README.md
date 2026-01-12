<h1 align="center">💊 Healthcare Drug Use Analytics Platform</h1>

<p align="center">
  <em>End-to-End Business Analysis Case Study.</em>
</p>
<p align="center">
  <img src="dashboard/FinalVideoWalkThrough-ezgif.com-speed.gif" alt="Healthcare Dashboard Demo" width="80%" />
</p>


---

## 📌 Business Problem

Healthcare stakeholders lack a unified view of drug usage patterns across states, facilities, and demographics. Fragmented data makes it difficult to identify high-usage regions, assess disparities, and support policy or operational decisions.

---

## 👥 Stakeholders

- Healthcare administrators
- Policy & compliance teams
- Clinical operations leadership

---

## 💼 Business Questions

- Which drug categories show the highest utilization across care settings?
- Are there regional or state-level disparities in drug usage?
- Which demographics exhibit abnormal or high-risk usage patterns?
- Where should intervention, policy review, or resource allocation be prioritized?

---
## 📋 Key Requirements

- Ability to drill down from national → state → facility level
- Consistent KPI definitions across all dashboards
- Filters by drug type, demographic group, and care setting
- Clean, validated data model to avoid reporting discrepancies
- Self-service exploration for non-technical stakeholders
---

## 💻 From Business Need to Technical Logic

- Business need: Identify regions with unusually high drug usage  
  Technical approach: SQL aggregation by state and drug category with normalized metrics

- Business need: Understand demographic risk patterns  
  Technical approach: Grouping and filtering by age, setting, and drug type

- Business need: Enable stakeholder exploration  
  Technical approach: Interactive dashboards with drill-downs and parameter controls

---

## 🎯 Real-World Scenario

Simulating a real-world public health research scenario, this project answers:

-  **Who** is most impacted by drug use?
-  **Where** are the highest-risk regions?
-  **What socioeconomic factors** contribute to these trends?

---

## 🚀 Key Outcomes

✔️ Over **60%** of drug-related incidents occur in **Emergency Departments**  
✔️ **Opioids & Cannabis** are the most reported substances  
✔️ **Rural counties** and **youth populations** are highly vulnerable  
✔️ **West Virginia** and **New Mexico** lead in per capita incidents, correlating with low income  

---

## 📊 Visual Insights

<p align="center">
  <img src="dashboard/FinalVideoWalkThrough-ezgif.com-video-to-gif-converter.gif" width="40%" />
  <img src="dashboard/FinalVideoWalkThrough-ezgif.com-video-to-gif-converter (1).gif" width="40%" />
  <img src="dashboard/FinalVideoWalkThrough-ezgif.com-video-to-gif-converter (2).gif" width="40%" />
</p>

Explore interactive dashboards showing:
- National trends by setting & state  
- Demographic usage by drug type  
- Urban vs. rural disparities  
- Facility-level hotspots

## 🧠 Behind the Scene
<p align="center">
  <img src="dashboard/diagram images/ERD.png" width="30%" />
  <img src="dashboard/diagram images/Relationship.png" width="60%" />
</p>

---

## 🛠️ Tools & Technologies

| Tool          | Purpose                                |
|---------------|----------------------------------------|
| `Google Colab`| Data wrangling, validation             |
| `Python`      | Pandas, NumPy, Matplotlib              |
| `Tableau`     | Interactive dashboards, storytelling   |
| `Excel`       | Initial review, calculations           |
| 🆕`KNIME`    | Clustering, forecasting, scenarios, GIS           |

---

## 🗂️ Project Structure
```
healthcare-drug-use-analytics/
├── README.md
├── LICENSE
├── data/
│   ├── aggregated_by_hospital.csv
│   ├── aggregated_by_state.csv
│   ├── figure_all_drugs_by_demographics.csv
│   ├── figure_all_drugs_by_urban_rural.csv
│   ├── figure_benzodiazepines_by_demographics.csv
│   ├── figure_cannabis_by_demographics.csv
│   ├── figure_opioids_by_demographics.csv
│   ├── figure_stimulants_by_demographics.csv
│   ├── figure_summary_all_settings.csv
│   ├── full_analysis_data.csv
│   ├── healthcare_data.csv
│   ├── Hospital_General_Information.csv
│   └── state_socioeconomic_yearly.csv
├── notebooks/
│   └── drug_use_analysis_colab.ipynb
├── dashboards/
│   └── dashboard_images/
│       ├── dashboard 1.png
│       ├── dashboard 2.png
│       ├── dashboard 3.png
│       └── dashboard 4.png
├── documentation/
│   ├── Summary Final.pdf
│   ├── Detailed Report Final.pdf
│   ├── Glossary.pdf
│   └── PM.pdf
│   └── Advanced Analytics Extension Report.pdf 🆕
│   └── Advanced Analytics Summary Report.pdf 🆕
├── advanced 🆕
│   ├── screenshots 
│       ├── Screenshot 1
│       ├── Screenshot 2
│       ├── Screenshot 3
│       ├── Screenshot 4
│       ├── Screenshot 5
│       ├── Screenshot 5
│       ├── Screenshot 7
├── LICENSE
└── README.md
```

---

## 📈 Dashboards Showcase

- **Dashboard 1**: Drug-related incidents by setting and state  
- **Dashboard 2**: Demographics & drug types (opioids, cannabis, stimulants, etc.)  
- **Dashboard 3**: Socioeconomic and rural/urban disparities  
- **Dashboard 4**: Facility-specific usage concentration

---

## 🆕 KNIME Extension: Advanced Analytics, Simulation & GIS

To move beyond descriptive Tableau dashboards, I extended the project in **KNIME** (no-code analytics platform).  

### 🔹 Advanced Analytics Layer
- **K-Means Clustering** – segmented states into:  
  - 🟠 Moderate Burden, Lower-Income  
  - 🔴 High-Income, High-Burden  
  - 🟢 Stable States with Lower Burden
<p align="center">
  <img src="advanced/screenshots/Screenshot (21).png" width="30%" />
  <img src="advanced/screenshots/Screenshot (24).png" width="30%" />
</p>
- **Time Series Forecasting (SARIMA)** – projected 12 months of future drug-use cases, revealing seasonal spikes 
<p align="center">
  <img src="advanced/screenshots/Screenshot (35).png" width="30%" />
  <img src="advanced/screenshots/Screenshot (43).png" width="30%" />
</p>
### 🔹 Scenario Simulation
- Developed **What-If models** with workflow variables.  
- Example: *+5% population growth & –10% prescription regulation* → overall cases ↓ but ED reliance ↑
<p align="center">
<img src="advanced/screenshots/Screenshot (44).png" width="30%" />
<img src="advanced/screenshots/Screenshot (45).png" width="30%" />
</p>
### 🔹 Geospatial Mapping
- Used **KNIME GIS Extensions** to build choropleth maps.  
- Hotspots aligned with poverty-heavy regions, guiding targeted resource allocation 🎯    
<p align="center">
<img src="advanced/screenshots/Screenshot (46).png" width="40%" />
</p>
---

## ⚡Decisions Enabled

- Identification of high-usage regions requiring policy review
- Visibility into demographic and facility-level usage trends
- Data-backed support for resource allocation and compliance discussions

---

## 📥 Data Sources

- **Healthcare Facility Data**: [HealthData.gov – HHS](https://healthdata.gov)
- **Socioeconomic Indicators**: [U.S. Census Bureau – ACS](https://data.census.gov)

---

## ▶️ Walkthrough Demo

🎬 [**Final Project Walkthrough Video**](https://drive.google.com/file/d/14JWPkNZdPiaVKG-on70i7fiIJevOviJa/view?usp=drive_link)

> Includes full explanation of methodology, findings, and dashboard tour.

---

## 💼 Role & Contribution

- Led full **data lifecycle**: extraction, transformation, visualization  
- Applied **business analysis** to define use case & requirements  
- Integrated **public health** and **data science** methodologies  
- Delivered **PM deliverables**: WBS, glossary, stakeholder documents
- 🆕 Extended project with **ML/AI enhancements**: clustering, forecasting, scenario modeling, GIS mapping

---

## 💬 Contact

**Vaibhav Nangia**  
👨‍💼 Business Data Analyst | PMP-Certified Project Manager | BI Storyteller  
🔗 [LinkedIn](https://www.linkedin.com/in/vaibhavnangia08050805/)  
📧 [Email](mailto:nangiavaibhav9@gmail.com)

---

## ⚠️ Limitations

This project focuses on exploratory and decision-support analysis. In a production environment, additional steps such as stakeholder-led KPI validation, automated data pipelines, and governance controls would be required.

---

<p align="center">
  <img src="https://img.shields.io/badge/Status-Complete-brightgreen" />
  <img src="https://img.shields.io/badge/Python-3.10-blue" />
  <img src="https://img.shields.io/badge/Tableau-Interactive-blueviolet" />
  <img src="https://img.shields.io/badge/Colab-Notebooks-orange" />
</p>

