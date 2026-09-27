# 🎨 Phase 3: Project Design

---

## 📌 Project Title
# **Auto Ticket Classification using Flow Designer**

---

## 🏗️ System Design
The project is designed using **ServiceNow Flow Designer** to automatically classify IT support tickets[span_7](start_span)[span_7](end_span).

---

## 🗃️ Custom Table
* **Table Name:** Incident Workflow[span_8](start_span)[span_8](end_span)
* **Description:** The table is used to store the school/organization IT ticket records[span_9](start_span)[span_9](end_span).

---

## 📋 Fields
* **Number** – Auto Number[span_10](start_span)[span_10](end_span)
* **Caller** – Reference to `sys_user`[span_11](start_span)[span_11](end_span)
* **Category** – Choice[span_12](start_span)[span_12](end_span)
* **Subcategory** – Choice[span_13](start_span)[span_13](end_span)
* **Short Description** – String[span_14](start_span)[span_14](end_span)
* **Description** – String[span_15](start_span)[span_15](end_span)
* **State** – Choice[span_16](start_span)[span_16](end_span)
* **Assigned Group** – Reference to `sys_user_group`[span_17](start_span)[span_17](end_span)
* **Assigned to** – Reference to `sys_user`[span_18](start_span)[span_18](end_span)

---

## 🔀 Category and Subcategory Design
* **Network** ➔ Wi-Fi[span_19](start_span)[span_19](end_span)
* **Hardware** ➔ Projector[span_20](start_span)[span_20](end_span)
* **Access** ➔ Forgot Password[span_21](start_span)[span_21](end_span)
* **Performance** ➔ Slow Computer[span_22](start_span)[span_22](end_span)

---

## ⚙️ Automation Design
When a new ticket is created, **Flow Designer** checks the Short Description for predefined keywords[span_23](start_span)[span_23](end_span)[span_24](start_span)[span_24](end_span):

* **WiFi or Network** ➔ Category: Network, Subcategory: Wi-Fi[span_25](start_span)[span_25](end_span)[span_26](start_span)[span_26](end_span)
* **Projector** ➔ Category: Hardware, Subcategory: Projector[span_27](start_span)[span_27](end_span)[span_28](start_span)[span_28](end_span)
* **Password or Login** ➔ Category: Access, Subcategory: Forgot Password[span_29](start_span)[span_29](end_span)[span_30](start_span)[span_30](end_span)
* **Slow or Hanging** ➔ Category: Performance, Subcategory: Slow Computer[span_31](start_span)[span_31](end_span)[span_32](start_span)[span_32](end_span)

---

## 📧 Email Notification
After ticket classification, an automated email notification is sent to the caller[span_33](start_span)[span_33](end_span)[span_34](start_span)[span_34](end_span).

---

## 🎯 Expected Result
The system automatically classifies the ticket and assigns the appropriate Category and Subcategory[span_35](start_span)[span_35](end_span)[span_36](start_span)[span_36](end_span).
