# Healthcare-Analytics
Power BI Travel &amp; Hospitality dashboard analyzing 9,043+ records across 13 datasets | ADR · Guest Reviews · Flight Analytics · Revenue | Power Query · DAX · Custom Theme
# 🏥 Healthcare Operations & Financial Analytics — Power BI Portfolio Project

## 📌 Project Overview
A comprehensive, end-to-end Healthcare Analytics project built with **Power Query** and **Power BI**. This dashboard integrates operational clinic data, patient clinical vitals, and financial billing systems to optimize patient care and maximize hospital revenue collection across multiple datasets.

---

## 📂 Datasets Used

| Table | Type | Key Columns | Description |
|-------|------|-------------|-------------|
| Encounters Log | Fact | EncounterID, PatientID, ProviderID | Detailed records of patient clinic visits and appointments |
| Insurance Claims | Fact / Data | ChargeID, AmountBilled, AmountPaid, Status | Financial claims, billing amounts, and insurance status |
| Vitals Log | Fact / Data | EncounterID, BloodType, SystolicBP, HeartRate | Clinical metrics, blood types, and patient vital signs |
| Patients Master | Dimension | PatientID, FirstName, LastName, Gender, DateOfBirth | Patient demographic profiles and master data |
| Providers Master | Dimension | ProviderID, FullName, Speciality | Healthcare providers and doctor reference data |
| Facilities Master | Dimension | FacilityID, FacilityName, Type | Hospital and clinic location reference data |
| Date Table | Dimension | Date, Year, Quarter, Month Name, Year Month | Centralized calendar table for advanced time-intelligence |

---

## 🔧 Tools & Skills Demonstrated

- **Power Query** — Data transformation, cleaning, handling blank dates, and preparing healthcare schemas.
- **Data Modeling (Star Schema)** — Designing a robust data model by establishing critical relationships, resolving cross-filtering limitations, and linking financial logs to operational logs.
- **DAX (Data Analysis Expressions)** — Developing customized business measures and advanced columns:
  * `Total Patients`, `Total Encounters`
  * `Total Amount Billed`, `Total Amount Paid`
  * `Collection Rate %` (Revenue collection performance tracking)
  * `Patient Age` & `Age Group` (Dynamic demographic segmentation)
- **UI/UX Design** — Creating a modern multi-page dashboard with container layouts, unified healthcare color themes, conditional formatting, and **Sync Slicers** for interactive cross-page filtering.

---

## 🚀 Key Features & Dashboard Architecture

### 📄 Page 1: Executive Summary (Operational View)
* High-level operational overview tracking overall patients and encounters.
* Line chart analyzing encounter trends over time.
* Breakdown of encounter types (Emergency, Outpatient, Urgent Care) using Donut Charts.
* Top 5 Providers ranked dynamically by their total patient encounters.

### 📄 Page 2: Financial & Claims Analysis (Revenue View)
* Financial health cards showing **Total Billed ($6.55M)** vs. **Total Paid ($5.24M)**.
* **Collection Rate % (79.96%)** tracker to identify financial leakages.
* Comparative column charts showing billing vs. actual payments for each insurance provider.
* Advanced Matrix table with conditional formatting to spotlight high-risk insurance claims.

### 📄 Page 3: Clinical Metrics & Vitals (Medical View)
* Patient distribution by **Blood Type** (identifying A+ and B- dominance).
* Time-series line chart tracking monthly fluctuations in average **Systolic Blood Pressure (BP)** and **Heart Rate**.
* Interactive slicers for dynamic filtering by **Gender** and **Age Group** (e.g., Under 18, 18-35, Over 65).

---

## 🧠 Lessons Learned & Data Insights

1. **Revenue Gap Identified:** The overall collection rate stands at **79.96%**, leaving over $1.3M in uncollected or denied billing—presenting a clear opportunity for revenue cycle optimization.
2. **Operational Leaders:** Doctor Mary Garcia is the top performing provider, managing over 2.6K encounters across the system.
3. **Cross-Filtering Optimization:** Solved a critical data modeling challenge where the central Date Table could not filter isolated billing logs by establishing proper cross-filter directions between encounters and financial tables.
4. **Demographic Insights:** Custom DAX segmentation revealed clear age-group patterns and blood type distributions, allowing better capacity planning for specific clinical treatments.

---

## 👤 Author
**AbdelHassib ESSAYAD** Data Analyst / Business Intelligence Specialist  
Power BI · Power Query · DAX · Healthcare Business Intelligence  

🔗 [GitHub Portfolio] https://github.com/hassib-essayad
📧 essayad@gmail.com
