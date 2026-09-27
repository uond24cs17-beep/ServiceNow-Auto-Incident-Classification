# 🔍 PHASE 2: REQUIREMENT ANALYSIS

---

## 🖥️ Platform & Tools
# **ServiceNow Developer Instance (PDI)**
* **Module:** Flow Designer & Incident Management
* **Version Control:** GitHub Repository

---

## ⚙️ Functional Requirements
* **Trigger:** Automatically fire when a new Incident record is created.
* **Inspection:** Scan `Short Description` for key keywords (e.g., *Wi-Fi*, *Hardware*, *Password*).
* **Action:** Automatically update `Category`, `Subcategory`, and `Assignment Group`.

---

## 📊 Non-Functional Requirements
* **Performance:** Processing completed within seconds of submission.
* **Accuracy:** 100% accurate rule-based classification.
* **Scalability:** Handles continuous incoming incident requests seamlessly.
