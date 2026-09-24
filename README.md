# Automated Incident Classification in ServiceNow

## Project Overview
This project automates the classification of incidents in ServiceNow based on keywords provided in the short description. When an incident is logged with specific issue descriptions (e.g., "Projector not turning on"), the system automatically sets the appropriate Category and Subcategory using Flow Designer.

---

## 📌 Phase 1: Brainstorming & Ideation Phase
- **Problem Statement:** IT service desks receive high volumes of tickets daily. Manual categorization leads to delay, human error, and misrouting of incidents.
- **Proposed Solution:** Implement an automated workflow in ServiceNow using Flow Designer to inspect incoming incident details and classify them instantly.
- **Target Category:** Hardware / Projector Issues.

---

## 📌 Phase 2: Requirement Analysis Phase
- **Platform:** ServiceNow Developer Instance (PDI)
- **Tooling:** Flow Designer, Custom Tables, Update Sets
- **Functional Requirements:**
  1. Trigger when a new incident record is created.
  2. Check if `Short Description` contains keywords like "Projector".
  3. Automatically set `Category` to **Hardware** and `Subcategory` to **Projector**.

---

## 📌 Phase 3: Project Design Phase
- **Data Model:** Custom Incident Table (`u_incident_workflow`) with Choice fields for Category and Subcategory.
- **Workflow Logic:**
  - **Trigger:** Record Created -> `u_incident_workflow` Table.
  - **Condition:** `Short Description` contains "Projector".
  - **Action:** Update Record -> Set Category = Hardware, Subcategory = Projector.

---

## 📌 Phase 4: Project Planning Phase
- **Module 1:** Custom Table Setup & Choice List Configuration.
- **Module 2:** Flow Creation & Condition Rules definition in Flow Designer.
- **Module 3:** Workflow Activation and Testing with Sample Incidents.
- **Module 4:** Exporting Configuration via Update Set for Deployment.

---

## 📌 Phase 5: Project Development Phase
- Configured custom table and choices on ServiceNow instance.
- Developed the automated workflow logic using ServiceNow Flow Designer.
- Grouped all technical configurations inside a custom Update Set (`Project Update Set`).
- Complete Update Set exported as XML for delivery (Uploaded in this repository).

---

## 📌 Phase 6: Project Testing Phase
- **Test Case:** Created a test incident with Short Description: *"Projector not turning on"*.
- **Result:** Successfully validated that Category auto-filled to **Hardware** and Subcategory to **Projector**.
- **Execution Log:** Verified Flow Designer execution logs showing successful trigger and field update.

---

## 📌 Phase 7: Project Documentation Phase
- All project requirements, table definitions, and workflow diagrams documented.
- Exported XML file saved as proof of technical implementation.

---

## 📌 Phase 8: Project Demonstration Phase
- Public Repository created with complete phase-wise project breakdown.
- Demo video recorded showcasing live incident creation and auto-classification.
- https://drive.google.com/file/d/1k7DLwueAE1rcMJ9GYi0pZ-9l6ZwLC6g9/view?usp=drivesdk
