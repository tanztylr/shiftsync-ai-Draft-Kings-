# Project Charter: ShiftSync AI

## 1. Executive Summary & Business Case
As organizations rapidly integrate emerging technologies into core product lines, the demand for AI-literate talent is outpacing market supply. Simultaneously, operational roles face a shift in day-to-day responsibilities. 

**ShiftSync AI** is an internal talent mobility platform designed to proactively map current employee skill sets against future AI-augmented role requirements. By automating skill-gap analyses and generating personalized learning paths, this initiative maximizes internal talent mobility, protects institutional knowledge, reduces external recruitment costs, and accelerates the adoption of AI-assisted productivity tools across the enterprise.

---

## 2. Project Objectives & Success Metrics (KPIs)
*   **Objective 1:** Build and pilot a functional MVP platform for the Customer Operations department within 30 days.
*   **Objective 2:** Establish a standardized logic for matching current skills to future-state technical roles.
*   **KPI 1 (Business Value):** Target a 15% reduction in external recruitment costs for technical roles by filling vacancies internally.
*   **KPI 2 (Project Delivery):** Achieve 100% on-time delivery of the MVP workspace with cross-functional sign-off from Legal, InfoSec, and Engineering.

---

## 3. Scope Boundaries
### In-Scope
*   Development of a functional MVP dashboard using Python (Streamlit or FastAPI backend).
*   Integration of LLM APIs (OpenAI/Anthropic) to ingest unstructured resume/LinkedIn data and parse it into 10 critical HRIS data points.
*   Automated generation of a 3-step personalized upskilling roadmap per user profile.
*   Cross-functional governance framework (RASCI Matrix, RAID Log, Change Management Playbook).

### Out-of-Scope
*   Direct live API integration with actual corporate HRIS production systems (Workday/Greenhouse) during the MVP phase (synthesized/mock data will be used).
*   Automatic purchasing or procurement of third-party training courses listed in the upskilling roadmaps.

---

## 4. Technical Design: The 10 Critical AI Data Points
To drive progress via emerging tech, the AI skills-mapping engine requires structured data. The system will extract, normalize, and weigh the following 10 data points from employee profiles to calculate role compatibility:

1.  **Core Domain Expertise:** Primary functional area (e.g., Customer Support, Operations).
2.  **Technical Literacy Score:** Current familiarity with software, databases, or low-code tools.
3.  **Adjacent/Transferable Skills:** Soft skills such as stakeholder management, data analysis, or problem-solving.
4.  **Years of Experience in Current Role:** Proxies the depth of institutional-specific knowledge.
5.  **Historical Upskilling Speed:** Record of completing past company training or certifications.
6.  **Expressed Career Interest:** Employee’s self-stated career trajectory goals.
7.  **Current Tool Stack Familiarity:** Specific applications utilized daily (e.g., Jira, Zendesk, SQL).
8.  **Project/Delivery Methodology:** Experience with Agile, Scrum, or Waterfall frameworks.
9.  **Bandwidth/Availability Capacity:** Current utilization rate to determine hours available per week for upskilling.
10. **Manager Readiness Rating:** Leadership's assessment of the employee's adaptability to change.
