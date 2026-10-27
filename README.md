# Awesome-Business-Continuity-Management
<<<<<<< HEAD
=======
# Awesome-Business-Continuity-Management

Copy-Item README.md README.md.bak -Force
# Manual step: replace SaaS and Open-Source sections with content above
git add README.md
git commit -m "docs: add BCM pricing (Fusion $40K+, Castellan UK £33K/3yr and £138K DVLA, Archer CDW $49.87/mo, Noggin A$75K/yr) and flag open-source gap; note ServiceNow no product pricing"
git push
# Awesome-Business-Continuity-Management

# Awesome-Business-Continuity-Management
>>>>>>> 69f1df92acfa18fb086bf03a0e0abd1ca52bc1cc

## Top Business Continuity Management (BCM) Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Business Impact Analysis, Recovery Planning & Organizational Resilience*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Business Continuity Management (BCM)**. These tools enable organizations to identify critical business functions, assess the impact of disruptions, develop recovery strategies, and coordinate crisis response—ensuring that operations can continue or be restored quickly when adverse events occur.



**Examples** include ServiceNow Business Continuity Management, Fusion Risk Management, Castellan (Riskonnect), Assurance Software, Archer, MetricStream, Noggin, Preparis, Quantivate, and BC in the Cloud (Everbridge) (the category leaders).



**Open-source emphasis**: This section is notably thin compared to other categories—BCM is a specialized, compliance-heavy domain where open-source options remain nascent or fragmented. The projects listed below are early-stage, domain-specific, or adjacent to core BCM rather than full platform replacements.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[ServiceNow Business Continuity Management](https://www.servicenow.com/)**  

  Enterprise BCM on the Now Platform with crisis management, business impact analysis (BIA), recovery and exercise management, and emergency notification via Everbridge integration; the Zurich release adds threat assessment enhancements allowing BCM managers to trigger assessments before, during, and after crises with automated next steps . Dependencies identified in BIA can be assessed against CMDB configuration item data during crisis events .



- **[Fusion Risk Management](https://www.fusionrm.com/)**  

  Enterprise Resilience Decision System replacing static continuity plans with live, data-driven recovery; maps relationships across people, processes, places, systems, and third parties to show what is impacted and what to prioritize during disruption . Designed for complex, regulated organizations needing executive-ready reporting and configurable workflows .



- **[Castellan (Riskonnect)](https://www.riskonnect.com/)**  

  BCM platform (merged with Riskonnect) offering BIA and plan development; Gartner reviewers note it works well out-of-the-box without consultancy for some banking clients, while others cite limited customization for process/product/department-level BIAs .



- **[Assurance Software](https://assurancesoftware.com/)**  

  Business continuity and risk management platform; reviewers highlight responsive customer service and flexibility since divesting from SunGard in 2018 .



- **[Archer](https://www.archerirm.com/)**  

  Operational Resilience platform integrating BIA, business continuity, IT disaster recovery, incident management, and crisis management in one system; features continuous dependency mapping, scenario testing, and quantified risk decisions .



- **[MetricStream](https://www.metricstream.com/)**  

  BCM software covering BIA with automated criticality scoring, RTO/RPO mapping, continuity plan templates, emergency mass notification across 25+ channels, AI-powered issue management, and vendor risk integration .



- **[Noggin](https://www.noggin.io/)**  

  Integrated resilience workspace with BIA tools, dependency mapping, recovery strategies, exercise/scenario testing, and digitized business continuity plans; no-code customization and ISO-aligned templates .



- **[Preparis](https://www.preparis.com/)**  

  Cloud-based continuity suite for everyday businesses with alert (bi-directional notifications), plan, assess (BIA), detect, and report modules .



- **[Quantivate](https://quantivate.com/)**  

  BCM software with integrated risk assessment, BIA, strategies, plan development, exercises, emergency notification, and incident management; recognized as Champion and Gold Medalist by SoftwareReviews .



- **[BC in the Cloud (Everbridge)](https://www.everbridge.com/)**  

  Low-code BCM platform trusted by 6,500+ customers; covers risk assessment through recovery with built-in templates, compliance workflows, RTO vs RTA comparison, and Everbridge 360 critical event management integration .



## Open-Source GitHub Projects



- **[Scribe (nocomp/scribe)](https://github.com/nocomp/scribe)**  

  Open-source hospital crisis management platform (AGPL) built for multi-site, multi-language healthcare crisis coordination; features an integrated scenario injector for training without touching production, an animator console for playing crisis scenarios in real time, isolated databases per exercise instance, and JSON-replayable scenarios; designed for GDPR/HDS compliance with 100% on-premise deployment and no cloud dependency .



- **[SitRep (f-eld-ch/sitrep)](https://github.com/f-eld-ch/sitrep)**  

  Open-source real-time situation management software for command staffs (AGPL); central journal for logging incoming/outgoing messages with centralized triage to appropriate recipients, digital crisis map with FOCP symbol subset, and feedback-driven development backed by Swiss non-profit F-ELD for civil protection use .



- **[Stronghold (mehdi-arfaoui/Stronghold)](https://github.com/mehdi-arfaoui/Stronghold)**  

  Open-source disaster recovery posture scanner (read-only, zero telemetry) for AWS environments; surfaces the "Reality Gap" between claimed protection and proven recoverability, tracks scenario coverage (AZ failure, data corruption, region failure), validates runbook liveness, and generates DR plans and runbooks from current infrastructure state .



- **[pyblastradius](https://pypi.org/project/pyblastradius/)**  

  Open-source blast radius analysis and criticality scoring tool (Python SDK with Rust core); supports Terraform dependency discovery (real), dbt lineage parsing (partial), and graph-based blast radius/criticality analysis; other integrations (Kubernetes, Airflow, OpenTelemetry) are not yet implemented—treat current release as foundation for custom dependency analysis workflows rather than a complete BCM platform .



### Additional Strong Open-Source Options



- **Business Impact Assessment (fstelte)** — Python/Flask web application for conducting BIAs locally or organization-wide with SQLite or MariaDB backend; archived in November 2025 with a successor solution planned, but the codebase remains available for reference .

- **GitHub `business-impact-analysis` topic** — 6 public repositories including BIA templates for small businesses, NIST SP 800-34 aligned BCP for FinTech, and scenario-based cyber risk analyses; fragmented but useful as starting points for custom BIA tooling .

- **openDesk** — While not a BCM platform, this open-source office suite (files, chat, email, video conferencing) was tested by German social insurance organizations as an emergency workplace in BCM scenarios and found suitable for crisis communication when primary IT fails; relevant as a resilience infrastructure component .



**Frameworks for building custom systems**: Combine **Scribe** for hospital crisis scenario training and command coordination, **SitRep** for command staff situation management with journal logging, and **Stronghold** for proving disaster recovery posture in AWS environments in a self-hosted resilience toolkit; these tools address specific BCM-adjacent needs (crisis coordination, DR validation) rather than replacing full BCM platforms with BIA, plan management, and executive dashboards.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- BCM platforms handling critical business process data and crisis communications must comply with applicable regulations (ISO 22301, DORA, industry-specific requirements) and organizational resilience policies.

- **Open-source BCM is significantly underdeveloped compared to other IT management categories**—the projects listed above address specific niches (hospital crisis simulation, command staff situation management, DR posture validation) but do not collectively replace commercial BCM platforms with integrated BIA, plan management, exercise tracking, and executive reporting. Organizations requiring full BCM capability should plan for commercial platforms or substantial custom development.

- Verify license terms for commercial use; Scribe and SitRep use AGPL, Stronghold is open-source (check repository), and pyblastradius is a PyPI package with mixed implementation status .



---



**Made for business continuity managers, resilience officers, crisis coordinators, and risk management teams.**  

Let's make business continuity management more open, testable, and recoverable.
