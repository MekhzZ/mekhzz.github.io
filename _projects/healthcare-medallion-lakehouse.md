---
title: "Payer-Scale Medallion Lakehouse"
excerpt: "Longitudinal High-Risk Patient & Cost Analytics using Databricks, PySpark, and HIPAA-compliant de-identification."
tags: [Data, AI/ML]
rank: 1
---
**[GitHub](https://github.com/MekhzZ/PayerScaleMedallionLakehouse)**

### Project Overview
<p class="text-justify">Developed a Medallion Architecture (Bronze, Silver, Gold) on Databricks to identify high-risk, high-cost members in US Healthcare. The project transforms fragmented CMS synthetic claims data into a unified "Patient 360" view for analytical insights.</p>

### Key Technical Contributions
* **Architecture**: Built an ELT pipeline using **PySpark** and **SparkSQL** to process Inpatient, Outpatient, and Pharmacy claims.
* **Security & Compliance**: Implemented **HIPAA-compliant de-identification** using SHA-256 Hashing with SALT and the Safe-Harbour method.
* **Advanced Analytics**: Engineered custom metrics including:
    * **Total Cost of Care (TCOC)**: Aggregated spend across multiple silos.
    * **Provider Fragmentation Score**: Measuring risk through unique provider counts per patient.
    * **Rescue-to-Preventive Ratio**: Identifying gaps in preventive care coordination.

### Impact & Results
* Identified a cohort of High-Risk patients (Diabetes + CKD) driving **3.5x higher costs** than the general population.
* Created a scalable Gold Layer table for longitudinal patient tracking.

### Tech Stack
**Databricks** | **PySpark** | **SparkSQL** | **Medallion Architecture**



