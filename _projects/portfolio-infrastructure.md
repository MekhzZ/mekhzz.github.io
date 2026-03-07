---
title: "Portfolio Infrastructure & Analytics Engine"
excerpt: "Architecting a high-performance, Jekyll-based technical hub with GA4/GTM tracking."
tags: [Data]
rank: 1
---

**[GitHub](https://github.com/MekhzZ/mekhzz.github.io.git)**

### Project Overview
<p class="text-justify">Rather than utilizing a standard "no-code" site builder, I engineered this portfolio as a Data-as-Code project to serve as a centralized, version-controlled repository for my professional identity. The site is designed to act as a high-fidelity "front door" for my projects, experiences and more while providing near to real-time, actionable insights into engagement through a custom-built analytics pipeline.</p>

### Key Features
* **Modular Architecture:** Leveraged the Jekyll framework to decouple content (Markdown) from presentation (Liquid/SCSS),

* **Advanced Analytics Integration:** Engineered a non-intrusive integration of Google Tag Manager (GTM) by utilizing theme-specific "hooks", ensuring no interference with the core layout while maintaining global tracking.

* **Recruiter Attribution Pipeline:** Architected a custom UTM tracking strategy (?utm_source=resume) to create a "conversion funnel." This allows for the differentiation between organic traffic and direct interest from my LaTeX-generated CV.

* **Caching & Asset Optimization:** Solved browser-side caching issues for UI assets (like bio-photos and favicons) by implementing a version-query parameter system (?v=2).

### Impact & Results
* **Data-Driven Visibility:** Successfully validated the end-to-end data pipeline, capturing live "Resume" source traffic within the GA4 DebugView and Real-time reports.

* **Operational Efficiency:** Achieved a "Single Source of Truth" for professional assets, reducing the time required to update project documentation across multiple platforms by 80%.

* **Professional Branding:** Demonstrated full-stack technical literacy by showcasing the ability to manage web infrastructure and marketing analytics.

### Tech Stack
**Jekyll** | **YAML** | **Markdown** | **Google Tag Manager (GTM)** | **Google Analytics 4 (GA4)** | **Git** | **GitHub Pages**

