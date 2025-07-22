# Intro-to-Splunk
# 📘 Splunk Learning Journey

This repo documents my learning journey with Splunk, one of the most widely used SIEM tools. I'm exploring its core features, especially the Search & Reporting app, to understand how to analyze data effectively for monitoring and alerting.

---

## 💻 Splunk Setup

I installed and configured **Splunk Enterprise** on a **virtual machine running Ubuntu** during my semester break.  
This setup allows me to practice log ingestion, create dashboards, and experiment with Splunk’s security features in a controlled environment.

---

## 📦 Built-in Apps in Splunk

Splunk comes with several built-in apps that extend its functionality:

- **Search & Reporting**  
  The main interface used to run searches, create dashboards, and analyze events.
  
- **Audit Trail**  
  Allows administrators to track user activities within the Splunk platform for compliance and auditing.

- **Splunk Secure Gateway**  
  Enables Splunk to send alerts and dashboards to mobile devices using secure communication.

These apps help streamline monitoring, analysis, and remote access for Splunk users across various use cases.

---

## 🔐 Splunk Predefined Roles

There are three predefined user roles in Splunk:

- **Administrator**
  - Can install apps, ingest data, and create knowledge objects for all users.
- **Power User**
  - Can create and share knowledge objects within apps and perform real-time searches.
- **User**
  - Can view their own knowledge objects and any shared with them.

---

## 🔍 Search & Reporting App Overview

The **Search & Reporting** app provides a default interface for searching, analyzing, and visualizing data.

### 🧩 Main Components

1. **Search Bar** – Run queries using strings or SPL (Search Processing Language).
2. **Time Range Picker** – Define a specific time range to retrieve relevant events.
3. **How to Search Panel** – Contains links to documentation and tutorials.
    - **Data Summary Breakdown**:
        - **Hosts** – Origin system (hostname/IP/FQDN).
        - **Sources** – File path, port, or script where events came from.
        - **Sourcetypes** – Classification of the data format.
4. **Table View** – UI-driven way to explore data without writing SPL.
5. **Search History Menu** – View and re-run past searches.
    - **Filter Window** – Filter search history by terms.
    - **Time Filter** – View searches from Today, Last 7 Days, or Last 30 Days.

> **Note:**
> By default, a search job stays active for **10 minutes**.
> Shared jobs stay active for **7 days**.

---

## 🔎 Using the Search Function

I uploaded sample data from this GitHub repo:  
🔗 [splunk-sample-data](https://github.com/tmartin14/splunk-sample-data)

### 💡 Key Learnings:

- **Search assistant** shows auto-complete terms, syntax help, and contextual matches.
- **Time Picker** improves performance by limiting the search scope.
- Search results highlight the term used.
- Default fields shown per event: `host`, `source`, `sourcetype`.
- Hovering on text in the event list allows you to:
  - Add to search
  - Exclude matching events
  - Start new search
  - View event action info

---

## 🆕 New Search Interface Features

- **Save As Menu**
  - Save a search as a knowledge object
- **Search Result Tabs**
  - **Events** – Raw log output
  - **Patterns** – View common patterns in the data
  - **Statistics / Visualization** – Appears when a transforming command is used
- **Search Action Buttons**
  - Edit, Send to Background, Inspect Job, Delete Job, Export (Raw, CSV, XML, JSON)
- **Search Mode Selector**
  - **Fast Mode** – Returns only default/required fields
  - **Smart Mode** – Adapts to query type
  - **Verbose Mode** – Returns all field and event data
- **Timeline** – Interactive range selector tied to time picker
- **Field Sidebar**
  - **Selected Fields** – Default fields like `_time`, `host`
  - **Interesting Fields** – Extracted automatically by Splunk

> 🧠 **Note:** Commands that generate stats/visuals (like `stats`, `chart`) are called **Transforming Commands**.

---

## ✏️ Search Term Tips

1. `error*` – Add asterisk to match **events starting with a word**.
2. **Not case sensitive** – Searches are case-insensitive by default.
3. **Booleans**:
    - Order of evaluation: `NOT` → `OR` → `AND`
    - Use parentheses `()` to control logic flow
4. **Exact phrases** – Use quotes (`"failed login"`)
5. **Escaping quotes** – Use backslash `\"` if the phrase contains quotes.

---

## 📌 Upcoming Modules (From Splunk Training)

I'll be learning more in these next modules:

### 🔸 Module 6 – What are Commands?
- Understand the anatomy of Splunk's search language:
  - Search terms, commands, functions, arguments, clauses
- Learn best practices for writing efficient searches

### 🔸 Module 7 – What are Knowledge Objects?
- Five categories:
  - Data interpretation, classification, enrichment, normalization, data models
- Understand different types of knowledge objects and how they’re used in Splunk

---

Stay tuned for more updates as I continue exploring Splunk!

#Splunk #SIEM #CyberSecurity #LearningByDoing

