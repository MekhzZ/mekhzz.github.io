---
title: "HealthSparq Provider Data Engine"
excerpt: "A high-security data synchronization engine designed to bypass WAF protections and retrieve 3,865+ restricted medical provider records."
tags: [Data]
rank: 3
---
**[GitHub](https://github.com/MekhzZ/HealthSparqProviderDataEngine.git)**

### Project Overview
<p class="text-justify">Engineered a custom synchronization engine to aggregate provider information from the HealthSparq Nevada Medicaid portal. The system successfully navigated an Imperva WAF environment and bypassed a 300-result visibility cap to retrieve a complete dataset of 3,865 unique provider records.</p>

### Key Technical Contributions
* **Advanced Sharding**: Implemented **Specialty-Based Sharding** to overcome API index limits, extracting 129 internal codes to ensure 100% database visibility.
* **Security & Authentication**: Developed a **Stateless Token Handshake** to replace volatile cookie-based sessions, performing backend "activation" via insurer gateways for higher stability.
* **Polite Scraping Architecture**: Integrated linear backoff with jitter and reactive re-authentication to mimic legitimate browser fingerprints (Chrome 120 TLS) and avoid robotic signatures.
* **Data Integrity**: Built a transformation pipeline to de-duplicate "Provider-at-Location" instances into a clean, analysis-ready JSONL dataset.

### Impact & Results
* **100% Coverage**: Successfully bypassed visibility caps to extract 3,865 unique providers.
* **Resilience**: Created a "Resume Capability" feature that skips completed shards, significantly saving bandwidth and processing time.

### Tech Stack
**Python 3.12** | **curl_cffi** | **Stateless Auth** | **Data Orchestration**

