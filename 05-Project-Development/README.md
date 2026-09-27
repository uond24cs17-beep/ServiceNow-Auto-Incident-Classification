# ⚡ Phase 5: Implementation - Part 2

---

## 📌 Objective
To build the workflow trigger and conditional logic using ServiceNow Flow Designer.

---

## ⚡ Step 1: Trigger Setup
* **Trigger Condition:** Created Record on **Incident Workflow** table.

---

## 🔀 Step 2: Conditional Actions
* 📶 **If Short Description contains "WiFi" or "Network":** 
  ➔ Update Record ➔ Category: Network, Subcategory: Wi-Fi
* 📹 **Else If Short Description contains "Projector":** 
  ➔ Update Record ➔ Category: Hardware, Subcategory: Projector
* 🔑 **Else If Short Description contains "Password":** 
  ➔ Update Record ➔ Category: Access, Subcategory: Forgot Password
* 💻 **Else If Short Description contains "Slow":** 
  ➔ Update Record ➔ Category: Performance, Subcategory: Slow Computer

---

## 📧 Step 3: Notification Action
* Added **Send Email** action to notify the caller upon classification completion.

