# 🎨 Phase 3: Project Design

---

## 📌 Project Title
# **Auto Ticket Classification using Flow Designer**

---

## 🏗️ System Design
The project is designed using **ServiceNow Flow Designer** to automatically classify IT support tickets.

---

## 🗃️ Custom Table
* **Table Name:** Incident Workflow
* **Description:** The table is used to store school and organization IT ticket records.

---

## 📋 Fields
* 🔢 **Number** ➔ Auto Number
* 👤 **Caller** ➔ Reference to `sys_user`
* 🏷️ **Category** ➔ Choice
* 🏷️ **Subcategory** ➔ Choice
* 📝 **Short Description** ➔ String
* 📄 **Description** ➔ String
* 📊 **State** ➔ Choice
* 👥 **Assigned Group** ➔ Reference to `sys_user_group`
* 👤 **Assigned to** ➔ Reference to `sys_user`

---

## 🔀 Category and Subcategory Design
* 📶 **Network** ➔ Wi-Fi
* 🖥️ **Hardware** ➔ Projector
* 🔐 **Access** ➔ Forgot Password
* ⚡ **Performance** ➔ Slow Computer

---

## ⚙️ Automation Design
When a new ticket is created, **Flow Designer** checks the Short Description for predefined keywords:
* 📶 **WiFi or Network** ➔ Category: Network, Subcategory: Wi-Fi
* 📹 **Projector** ➔ Category: Hardware, Subcategory: Projector
* 🔑 **Password or Login** ➔ Category: Access, Subcategory: Forgot Password
* 💻 **Slow or Hanging** ➔ Category: Performance, Subcategory: Slow Computer

---

## 📧 Email Notification
After ticket classification, an automated email notification is sent to the caller.

---

## 🎯 Expected Result
The system automatically classifies the ticket and assigns the appropriate Category and Subcategory.

