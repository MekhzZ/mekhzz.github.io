# My Portfolio: Infrastructure & Design
#### A High-Performance Static Portfolio Built with Jekyll, Liquid, and Medallion-Style Content Organization

## Project Overview
This project involved architecting a personal portfolio. Moving beyond simple templates, I customized the Minimal Mistakes Jekyll theme to serve as a centralized hub for my projects, automated resumes, experiences and more.

- **Content as Data:** Organized projects and experiences using YAML/Markdown collections, treating site content as structured data.
- **Automation:** Streamlined the deployment process using GitHub Pages and Jekyll build pipelines.
- **SEO & Analytics:** Implemented tracking structures (such as UTM parameters) to analyze recruiter traffic and engagement.

## Technical Stack
- Framework: Jekyll (Ruby-based Static Site Generator).
- Hosting: GitHub Pages with custom domain mapping at https://mekhzz.github.io/

## Analytics Setup

### Phase 1: Google Analytics 4 (GA4) Creation
GA4 acts as Data Warehouse. It receives and processes the raw event data.

- Account Setup: Go to [Analytics](https://analytics.google.com/). Created an account and a Property named "Portfolio."

- Data Stream: Selected Web and entered URL (mekhzz.github.io).

- Measurement ID: Copied the G-XXXXXXXXXX code. This is the unique key that tells GTM where to send the "packets."

- Enhanced Measurement: Kept this ON. It automatically tracks "File Downloads" (resume PDF) and "Outbound Clicks".

### Phase 2: Google Tag Manager (GTM) Infrastructure
GTM is the Ingestion Engine. It listens for user actions and "tags" them for GA4.
- Container: Created a Web Container.

- The Tag:

    - Created a New Tag type: Google Tag.

    - Tag ID: Pasted GA4 Measurement ID.

    - The Trigger: Set it to Initialization - All Pages.

- Pro-Tip: Using "Initialization" instead of "Page View" ensures UTM parameters are captured reliably before the user has a chance to navigate away.

- Publish: Click Submit. The ingestion logic is not live until this version is published.

### Phase 3: Architecting the UTM Tracking Link
UTM (Urchin Tracking Module) parameters allow us to perform Source Attribution. Think of these as metadata tags for your incoming traffic.

- To track the README, appended these parameters to URL: https://mekhzz.github.io/?utm_source=readme&utm_medium=link&utm_campaign=portfolio_v1  

## Impact
- Reduced the time to update my professional profile across platforms by 80% through a "Single Source of Truth" repository.
- Tracking each data points that land on my portfolio

## Shout Out
- https://github.com/mmistakes/minimal-mistakes