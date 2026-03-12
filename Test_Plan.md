Test Plan: Salesforce Sales Cloud (Lead-to-Cash)
1. Introduction
This test plan outlines the strategy for verifying the end-to-end "Lead-to-Cash" workflow within a Salesforce Developer Org. The goal is to ensure data integrity and business logic consistency from initial lead acquisition to final revenue realization.

2. Test Scope
In-Scope
Lead Management: Validation of mandatory fields, Lead conversion logic, and record mapping.

Opportunity Management: Price Book association, Product addition, and automated Amount calculations.

Sales Stages: Verification of Stage transitions and "Closed Won" status finalization.

Data Integrity: Ensuring Account and Contact details remain consistent across converted records.

Out-of-Scope
Integration testing with external ERP or Marketing Cloud systems.

Performance/Load testing of the Salesforce Org.

3. Testing Strategy
Manual Testing: Used for initial exploratory testing and UI/UX validation.

Functional Testing: Verification of business rules (e.g., Lead conversion mapping).

Automation (Work in Progress): Utilizing Playwright + Python for regression testing of the login and core lead creation flows.

4. Tools & Environment
Platform: Salesforce Sales Cloud (Developer Edition)

Automation Framework: Playwright (Python)

Test Management: Microsoft Excel (Manual Test Cases)

Defect Tracking: GitHub Issues / Bug Reports (Excel)

Browser: Google Chrome (Latest)

5. Entry & Exit Criteria
Entry: Salesforce Org is configured with Standard Price Books and active Products.

Exit: All High and Medium priority test cases are executed. All "Showstopper" bugs are resolved or documented.

6. Risk Assessment
Risk: Salesforce dynamic IDs can cause automation flakiness.

Mitigation: Use robust selectors (XPath/CSS) based on stable attributes rather than auto-generated IDs.
