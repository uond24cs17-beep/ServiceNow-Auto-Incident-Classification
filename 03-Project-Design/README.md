# 🎨 PHASE 3: PROJECT DESIGN

---

## 📌 Project Title
# **Auto Ticket Classification using Flow Designer**

---

## 📐 Workflow Architecture

```text
[ New Incident Created ] ➡️ [ Flow Designer Triggered ]
                                     │
                                     ▼
                      [ Inspect Short Description ]
                                     │
         ┌───────────────────────────┼───────────────────────────┐
         ▼                           ▼                           ▼
[ Keyword: Wi-Fi ]          [ Keyword: Hardware ]       [ Keyword: Password ]
         │                           │                           │
         ▼                           ▼                           ▼
( Assign: Network )         ( Assign: Hardware )        ( Assign: IT Support )
