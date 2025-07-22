# Intro-to-Splunk
# 📘 Splunk Learning Journey

This repo documents my learning journey with Splunk, one of the most widely used SIEM tools. I'm exploring its core features, especially the Search & Reporting app, to understand how to analyze data effectively for monitoring and alerting.

---

## 💻 Splunk Setup

I installed and configured **Splunk Enterprise** on a **virtual machine running Ubuntu** during my semester break.  
This setup allows me to practice log ingestion, create dashboards, and experiment with Splunk’s security features in a controlled environment.

 ![Image Alt](https://private-user-images.githubusercontent.com/67587985/469162306-2101682a-cd1e-4723-85cf-151b0af12666.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTMxODM4NDksIm5iZiI6MTc1MzE4MzU0OSwicGF0aCI6Ii82NzU4Nzk4NS80NjkxNjIzMDYtMjEwMTY4MmEtY2QxZS00NzIzLTg1Y2YtMTUxYjBhZjEyNjY2LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA3MjIlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwNzIyVDExMjU0OVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTY4ZGNmZGUwNGFjMDY2OWM3ZWJkMzViOWVjNGU3ZDVkNGE2ZWM5ZDcwNmRhYzY4NTEwYzNlN2NmOGY0YzdiNTgmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.XuZN8B6Sx3ac2GPbSrTqz249prRMqFUV8-MbWQ5o8Ms)
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

 ![Image Alt](https://private-user-images.githubusercontent.com/67587985/469163876-dc9e5077-27cd-47a0-bdad-d5c80f51f22a.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTMxODM5MTIsIm5iZiI6MTc1MzE4MzYxMiwicGF0aCI6Ii82NzU4Nzk4NS80NjkxNjM4NzYtZGM5ZTUwNzctMjdjZC00N2EwLWJkYWQtZDVjODBmNTFmMjJhLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA3MjIlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwNzIyVDExMjY1MlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTUzYWI2MTBjNzE2ZThlMDA0MWZmNjUwODBhMDAwZTNkZTBhOTIyN2EzMWIyOTI0MWM4NTZkZGM5Mzc2ZjIxZDMmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.ILfJCLvU7OE14k2F19SNfL8qe6KmfrZNMhhHPpEb1_8)
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

 ![Image Alt](https://private-user-images.githubusercontent.com/67587985/469164422-9410c59a-0a83-4d95-b3ff-d2cf0b823509.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTMxODQwMDQsIm5iZiI6MTc1MzE4MzcwNCwicGF0aCI6Ii82NzU4Nzk4NS80NjkxNjQ0MjItOTQxMGM1OWEtMGE4My00ZDk1LWIzZmYtZDJjZjBiODIzNTA5LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA3MjIlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwNzIyVDExMjgyNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWQ0YzhjZTIwMTJkYWNjMTk2MjY4MmE2ZDNhOGUxNTNhYWY5OWE5NmM4OGY3YzUzMTM2MTZhMGJlZTJjMTg2MWUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0._TzNocyOdX40wERi5QxFlb_bpbLNS79irXQZn12X9Ng)

 ## 🆕 New Search Interface Components

- **Save As Menu** – Allows saving search as knowledge object.
- **Search Result Tabs**:
  - **Event Tab** – Displays events returned for the search.
  - **Pattern Tab** – Allows to see pattern in the data.
  - **Statistic/Visualization Tabs** – Display search-generated statistics/visualizations.
- **Search Action Button**:
  - Edit, Send to background, Inspect search jobs, Delete search jobs
  - **Export icon** – Raw, CSV, XML, JSON
- **Search Mode Selector**:
  - **Fast mode** – Cuts down on field info, only returns default and required fields.
  - **Smart mode** – Toggles behavior based on type of search run.
  - **Verbose mode** – Returns all fields and events, discovers everything possible.
- **Timeline** – Dynamically decided by the time chosen in the Time Range Picker; can select specific range to investigate.
- **Event List**
- **Field Sidebar**:
  - **Selected Fields** – Default fields
  - **Interesting Fields** – Extracted by Splunk based on its metadata

> **Note:** Commands that create statistics and visualizations are called **transforming commands**.

---

## ⏲️ Search Job Duration

- By default, a search job will remain active for **10 minutes**, after which Splunk needs to re-run the job.
- A **shared job** will remain active for **7 days**.

---

## 🧭 Exploring Events

In the event list:

- Search term will be highlighted.
- Events are shown with newest first.
- Timestamp is based on user's timezone settings.
- Bottom of each event shows: `host`, `source`, `sourcetype`
- Rolling over text allows to:
  - Add to search
  - Exclude events with that text
  - Launch new search using the text
  - Info button opens dropdown for event action

---

## 🧠 Using Search Terms

1. Add `*` at the end of word to return events that start with the word.
2. Not case sensitive – all matching results are returned.
3. **Booleans** (used with multiple terms, with order of evaluation):
   - `NOT`, `OR`, `AND`
   - Use parentheses `()` to control evaluation order.
4. Exact phrases – Place quotes `" "` around them.
5. Use backslash (`\`) to escape multiple quotes.

---




