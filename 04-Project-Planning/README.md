# 🛠️ Phase 4: Implementation - Part 1

---

## 📌 Objective
To set up the foundational database architecture in ServiceNow by creating the custom table and necessary fields.

---

## 🗂️ Step 1: Table Creation
* Created a custom table named **Incident Workflow**.
* Configured auto-numbering for unique ticket identification.

---

## 📋 Step 2: Field Configuration
* 👤 **Caller:** Created reference field pointing to User table (`sys_user`).
* 🏷️ **Category:** Created Choice field with Network, Hardware, Access, Performance.
* 🏷️ **Subcategory:** Created Choice field dependent on Category.
* 📝 **Short Description & Description:** String fields for user inputs.
* 📊 **State:** Choice field for ticket progress tracking.
