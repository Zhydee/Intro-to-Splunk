# Intro to Splunk
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
 ![Image Alt](https://private-user-images.githubusercontent.com/67587985/469197172-fa82a930-7ead-4665-80fb-0b67e0e1ada5.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTMxODg2OTUsIm5iZiI6MTc1MzE4ODM5NSwicGF0aCI6Ii82NzU4Nzk4NS80NjkxOTcxNzItZmE4MmE5MzAtN2VhZC00NjY1LTgwZmItMGI2N2UwZTFhZGE1LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA3MjIlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwNzIyVDEyNDYzNVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWVhMDdhMDM2YjAwMDhiYjJjMzZjNGZkNzllN2MyNmRkY2IyZTk3NWIzNjE0YzVlYzg5ZmUwM2U3ZDBhYTAxNjAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.FIsurz3PlzcYPXi6U5RU3FRI6l1M4TwzKIKRquR-Ois)
## 💾 Save As Menu

The **Save As Menu** allows you to save your search as a knowledge object for future reuse and sharing.

![Save As Menu in Splunk](https://private-user-images.githubusercontent.com/67587985/469197616-e728c287-a1c1-4149-9a5b-a8e4d930bca2.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTMxODg3MzQsIm5iZiI6MTc1MzE4ODQzNCwicGF0aCI6Ii82NzU4Nzk4NS80NjkxOTc2MTYtZTcyOGMyODctYTFjMS00MTQ5LTlhNWItYThlNGQ5MzBiY2EyLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA3MjIlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwNzIyVDEyNDcxNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTY1YWExODRmNDNmNjQ1ZTAwZTE3NzY5NzJmNDJkMGM2NmI2Yzg4NGMyZGI3MWVhMWIxNzAzM2M0Y2FlYzZlZWMmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.GqPKex8FTWeXO5ZwDYC7aE0KhIi-NrRmczT9_B8FMJM)

## 🔍 Search Interface Components

### 🗂️ Search Result Tabs
- **Event Tab** – Displays events returned for the search.
- **Pattern Tab** – Allows you to see patterns in the data.
- **Statistic / Visualization Tabs** – Display search-generated statistics or visualizations.
 ![Image Alt](https://private-user-images.githubusercontent.com/67587985/469199212-90aa7e0c-813d-4b86-950f-28533fdbf542.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTMxODkwMDIsIm5iZiI6MTc1MzE4ODcwMiwicGF0aCI6Ii82NzU4Nzk4NS80NjkxOTkyMTItOTBhYTdlMGMtODEzZC00Yjg2LTk1MGYtMjg1MzNmZGJmNTQyLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA3MjIlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwNzIyVDEyNTE0MlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTcyZTljMjk3NmEzOTFiM2I3YzYwZTgzZDExMmZhMDE5OTUxMGQyNjM1MTIyMTE1YzYwNWU4MmE0MDIyYWJlNzkmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.Hg9xwVqP02PtNFK3_ZJyoDLrrMAGHExrLvGNG4iavZU)
---

### ⚙️ Search Action Button

The **Search Action Button** provides quick access to several actions for managing your search jobs:

- **Edit Job Setting**
- **Send to Background**
- **Inspect Search Jobs**
- **Delete Search Jobs**

![Search Action Button in Splunk](https://private-user-images.githubusercontent.com/67587985/469200284-81493940-e28e-4a5f-8f00-203873886521.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTMxODkxNTYsIm5iZiI6MTc1MzE4ODg1NiwicGF0aCI6Ii82NzU4Nzk4NS80NjkyMDAyODQtODE0OTM5NDAtZTI4ZS00YTVmLThmMDAtMjAzODczODg2NTIxLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA3MjIlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwNzIyVDEyNTQxNlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTc4YzAyMjAxZWEwMjIxYmU2M2Y4YWMzMmJjNzljYWI4OTA3NTY3YTJkMTg0MWQ1N2FkMzM1YzNhNzRkOTRhNjgmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.seP6n1OYohkyIN9hxWRRpS0KlKMQ8Y2Tn0Kh8bjOUtk)

---

### 📤 Export Icon

Use the **Export Icon** to download your search results in the following formats:

- **Raw**
- **CSV**
- **XML**
- **JSON**

 ![Image Alt](https://private-user-images.githubusercontent.com/67587985/469201853-d5cbd191-5318-4906-8016-84954872cda8.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTMxODk0MTYsIm5iZiI6MTc1MzE4OTExNiwicGF0aCI6Ii82NzU4Nzk4NS80NjkyMDE4NTMtZDVjYmQxOTEtNTMxOC00OTA2LTgwMTYtODQ5NTQ4NzJjZGE4LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA3MjIlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwNzIyVDEyNTgzNlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTdlMDNjMzY5MTEwZTc2MTM0MWRhMTQ4MzdkOGJmNTQwYmM5NDM5NzRlZmE3YmU5MjkzYjNlODc2MjgwNzhlMzImWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.B0hK3fbh2OlLMouOqY8Damj1d-gTFHD257Zp7Bd76l4)

---

### 🔄 Search Mode Selector
- **Fast Mode** – Cuts down on field info; only returns default and required fields.
- **Smart Mode** – Toggles behavior based on the type of search run.
- **Verbose Mode** – Returns all fields and events; discovers everything possible.

 ![Image Alt](https://private-user-images.githubusercontent.com/67587985/469202334-e502d0bf-aa48-4866-a5e4-01acfb1de889.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTMxODk0OTcsIm5iZiI6MTc1MzE4OTE5NywicGF0aCI6Ii82NzU4Nzk4NS80NjkyMDIzMzQtZTUwMmQwYmYtYWE0OC00ODY2LWE1ZTQtMDFhY2ZiMWRlODg5LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA3MjIlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwNzIyVDEyNTk1N1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWNmMTc4OTIxODAzM2NjYWU3NDM5YzBjMzgzMWJmOTI2YmYyNGI1M2FlNmRjMjFlYTE5N2FiYTJmMmM1MmQ1ZWYmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.saYwJyKA0DptVuZmOdxMkuqkElnHsWkuSllitN7L7Do)
---

### 🕒 Timeline
- Dynamically adjusted based on the time range chosen in the **Time Range Picker**.
- You can select a specific range on the timeline to investigate further.
 ![Image Alt](https://private-user-images.githubusercontent.com/67587985/469202711-a1b0409d-6aca-41c8-b266-645e32ed3bd1.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTMxODk1NDgsIm5iZiI6MTc1MzE4OTI0OCwicGF0aCI6Ii82NzU4Nzk4NS80NjkyMDI3MTEtYTFiMDQwOWQtNmFjYS00MWM4LWIyNjYtNjQ1ZTMyZWQzYmQxLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA3MjIlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwNzIyVDEzMDA0OFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTIxZjRhMmNiZTIwYzc5NTdmOGExNmZjNjk4NTdmZmViZTY3NmM5MTU5YTM3MmM5ZTczM2I1YzdiZGUyM2Y4NjcmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.Bodew2XMWKUwzilp1ESaaAjQijOrdfU2KE77-xRW0bw)
---

### 📃 Event List
Displays a list of matching events for the query.
 ![Image Alt](https://private-user-images.githubusercontent.com/67587985/469203178-a1841034-11b3-491d-96c3-6aa128214794.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTMxODk2MjQsIm5iZiI6MTc1MzE4OTMyNCwicGF0aCI6Ii82NzU4Nzk4NS80NjkyMDMxNzgtYTE4NDEwMzQtMTFiMy00OTFkLTk2YzMtNmFhMTI4MjE0Nzk0LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA3MjIlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwNzIyVDEzMDIwNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTA0NWM1MDU3NjY0YTQ1YzY2YzA0MTdiOWEwYTg2Y2E5NTZhODk4NDU0YTYxNjFjNDc3MWQ1NTM3MTEyZWVkYWImWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.I7Q139nURf3iN_PAgoDIx5KLGLXmzwCup9z4vLfknb0)
---

### 🧾 Field Sidebar

The **Field Sidebar** helps users explore fields extracted from the events in their search results. It contains two main sections:

- **Selected Fields** – Default fields included in the search results.
- **Interesting Fields** – Fields extracted by Splunk based on metadata analysis and relevance.

![Field Sidebar in Splunk](https://private-user-images.githubusercontent.com/67587985/469203632-3bd51147-c624-4980-9da6-1e5045f2932f.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTMxODk2ODgsIm5iZiI6MTc1MzE4OTM4OCwicGF0aCI6Ii82NzU4Nzk4NS80NjkyMDM2MzItM2JkNTExNDctYzYyNC00OTgwLTlkYTYtMWU1MDQ1ZjI5MzJmLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA3MjIlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwNzIyVDEzMDMwOFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWM2MDYyYzU5NjAyNGEyMjQ2NTc2NGUzNDAwNmIzZjY2NjI5OTYxNzdmMDE2OTY5ZjNmNWJmODY0ZmZhNDkwYWUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.ZOrutleNZHtIfgJoZzpazAEb0ImKtRpY1cHnX9MEdek)

## ⏲️ Default Features

> 🔁 **Transforming Commands:**  
> Commands that create statistics and visualizations are referred to as **transforming commands**.

> ⏳ **Search Job Timeout:**  
> By default, a search job will remain active for **10 minutes**. After that, Splunk must re-run the job.

> 🗓️ **Shared Job Duration:**  
> A **shared job** will remain active for **7 days**.


---

## 🧭 Exploring Events

In the event list:
 ![Image Alt](https://private-user-images.githubusercontent.com/67587985/469205262-1d28f655-c374-4066-b3d0-39302311776d.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTMxODk5MjYsIm5iZiI6MTc1MzE4OTYyNiwicGF0aCI6Ii82NzU4Nzk4NS80NjkyMDUyNjItMWQyOGY2NTUtYzM3NC00MDY2LWIzZDAtMzkzMDIzMTE3NzZkLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA3MjIlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwNzIyVDEzMDcwNlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTdiZmRlNDY5MDIxMjE1YzA1YTEyOGM5Yzg4MGY2ODM3NGE2YWJjZmRjYThmNjI4Y2U0YWUzYWQ0YzJiYTU3OGQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.WtUyMqQ5bmtlZMsuqa4fweyFn00YIbDrTplm2CJIG2E)
 
- Search term will be highlighted.
- Events are shown with newest first.
- Timestamp is based on user's timezone settings.
- Bottom of each event shows: `host`, `source`, `sourcetype`
- Rolling over text allows to:
  - Add to search
  - Exclude events with that text
  - Launch new search using the text
   ![Image Alt](https://private-user-images.githubusercontent.com/67587985/469205872-e930c19a-814d-47e4-8860-5a33cc62137e.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTMxOTAwMjAsIm5iZiI6MTc1MzE4OTcyMCwicGF0aCI6Ii82NzU4Nzk4NS80NjkyMDU4NzItZTkzMGMxOWEtODE0ZC00N2U0LTg4NjAtNWEzM2NjNjIxMzdlLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA3MjIlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwNzIyVDEzMDg0MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWJlM2JiMjkyYzRiZDg3MGEwMzY4YzFhOTI5MmNmYjRlNjhkNzM3YmI0YTRmZmIxYzVjMDdjZDhhOTVmN2U1YmQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.-2FnnajFVfY99IXoI2q9cNK43fqB9ORKpryYLBljCL0)
- Info button opens dropdown for event action
 ![Image Alt](https://private-user-images.githubusercontent.com/67587985/469206088-f19ec568-82b2-496b-b610-2ca3241c7172.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTMxOTAwNDEsIm5iZiI6MTc1MzE4OTc0MSwicGF0aCI6Ii82NzU4Nzk4NS80NjkyMDYwODgtZjE5ZWM1NjgtODJiMi00OTZiLWI2MTAtMmNhMzI0MWM3MTcyLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA3MjIlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwNzIyVDEzMDkwMVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTdiN2RlZWYwMDY4N2RkYmE1N2JmMjJmODgwMTNkNmFhMWY4NGNkOTkyM2M3N2FlZDYzYThmYTJlMjUwNmMzMjEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.SFpEdV3uXJgozaqHDk72H69VXNfPaez6u-EMJ4ZFMrA)

---

## 🧠 Using Search Terms

Mastering Splunk search syntax helps extract meaningful results. Below are useful techniques with visual examples.

---

### 1. 🔎 Wildcard Search  
Add `*` at the end of a word to return events that start with that word.

![Image Alt](https://private-user-images.githubusercontent.com/67587985/469207027-7dceca90-35f7-4519-8ec3-6044330d89f3.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTMxOTAxODcsIm5iZiI6MTc1MzE4OTg4NywicGF0aCI6Ii82NzU4Nzk4NS80NjkyMDcwMjctN2RjZWNhOTAtMzVmNy00NTE5LThlYzMtNjA0NDMzMGQ4OWYzLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA3MjIlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwNzIyVDEzMTEyN1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTQwOGI5ZmZkZWI1MjllODFiNzZiNWMyMmRhZmEyMjA3MmVlNjRiOWZjMTQ5ODMzNGU5NDYzOTM3NjI4YzliNjYmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.x_eHu4vI1rd5M0n7jygs7kWx6U8hq2pwVFrpDEk8pmA)

---

### 2. 🔤 Case Insensitive  
Search is not case sensitive – all matching results are returned.

---

### 3. ⚖️ Boolean Operators  
Used with multiple terms (evaluated in this order):  
- `NOT`, `OR`, `AND`

![Image Alt](https://private-user-images.githubusercontent.com/67587985/469207027-7dceca90-35f7-4519-8ec3-6044330d89f3.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTMxOTA1MTksIm5iZiI6MTc1MzE5MDIxOSwicGF0aCI6Ii82NzU4Nzk4NS80NjkyMDcwMjctN2RjZWNhOTAtMzVmNy00NTE5LThlYzMtNjA0NDMzMGQ4OWYzLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA3MjIlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwNzIyVDEzMTY1OVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTUzYjBmYjU3NWYwODQ3NzdhYmIxMDhjYTQ2YTEzYWY3ZGYyNmM4MDdiNTNjNzVkNDBiZjRjNGIwYTdjYTkxOTAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.J7yaXFsfPJ_ifM-_bZkcrGNViY6rNvtFywMf8-NNQJ0)

> 💡 Use parentheses `()` to control the evaluation order.

![Image Alt](https://private-user-images.githubusercontent.com/67587985/469207173-5a480aea-ae03-42e0-8f7e-5fc4e775cc42.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTMxOTA1MTUsIm5iZiI6MTc1MzE5MDIxNSwicGF0aCI6Ii82NzU4Nzk4NS80NjkyMDcxNzMtNWE0ODBhZWEtYWUwMy00MmUwLThmN2UtNWZjNGU3NzVjYzQyLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA3MjIlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwNzIyVDEzMTY1NVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWJkNDMxY2Y5NzNlYTRlZjlhNjg4NDJiMjVkZjk3MWMyYjcxYTM2MmRlOTk4YWRjNGQ4OGE1M2YyNjI2MDg1YTQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.nE3jw9BCGZAM6527MXlmgpi2OBtHkSl-drajr87lplE)
---

### 4. 🗣️ Exact Phrase  
Place quotes `" "` around phrases for exact matching.

![Image Alt](https://private-user-images.githubusercontent.com/67587985/469207353-3f902128-e9cb-465d-8443-522cb15efdb3.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTMxOTA1MTQsIm5iZiI6MTc1MzE5MDIxNCwicGF0aCI6Ii82NzU4Nzk4NS80NjkyMDczNTMtM2Y5MDIxMjgtZTljYi00NjVkLTg0NDMtNTIyY2IxNWVmZGIzLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA3MjIlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwNzIyVDEzMTY1NFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWYzMDM3Y2MwNjEyYzBiZGJjOWQ4MDk4NTNkNzM3ZWNiZTM5NmFhZjQ3YjI2OTI3OWMxZTRkNWU3NWQxNDk1MWYmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.pwX34lWaJltvwkeMNZ9oIt_ASXfNRrlL07SMvzXNOcw)

---

### 5. 🧩 Escaping Quotes  
Use backslash `\` to escape multiple quotes inside a search term.

![Image Alt](https://private-user-images.githubusercontent.com/67587985/469207503-783ca889-aeca-46ed-a3b2-942d4e5f638b.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTMxOTA4NDYsIm5iZiI6MTc1MzE5MDU0NiwicGF0aCI6Ii82NzU4Nzk4NS80NjkyMDc1MDMtNzgzY2E4ODktYWVjYS00NmVkLWEzYjItOTQyZDRlNWY2MzhiLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA3MjIlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwNzIyVDEzMjIyNlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTYzNjA2NGFlNDYxZTljOWVmYzljZGFjOTdhMGEzM2YzM2ZmNmYzNzM2N2M4MjA0NzQxYWM0YjEwNTJmOGY3NmMmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.5-RPTVRjEwbNr2NIByYwT_knDVoggN4DDJEfoHFyzyw)


## 🔎 Commands for Search Result

### 5 Components of Splunk's Search Language:
1. **Search Terms** – Foundation of search queries  
2. **Commands** – Tell Splunk what we want to do with the search results (create charts, compute statistics, format data)  
3. **Function** – Explain how we want to chart, compute, and evaluate the results  
4. **Arguments** – Variables we want to apply to the function  
5. **Clauses** – Explain how we want the results grouped or defined

### Most Efficient Way to Filter Events:
1. Time  
2. Index  
3. Source  
4. Host  
5. Sourcetype

---

## 📚 Knowledge Objects

### 5 Categories of Knowledge Objects:

#### 1. Data Interpretation
- **Fields** – Automatically extracted from data based on selected sourcetype  
- **Field Extraction** – Manually add additional insights to your data  
- **Calculated Fields** – Added at search time to perform calculations based on values of existing fields

#### 2. Data Classification
- **Event Types** – Categorize events based on search terms  
- **Transaction** – Group of conceptually related events that span time

#### 3. Data Enrichment
- **Lookups** – Add other fields/values to events not included in indexed data  
- **Workflow Actions** – Create links within events that interact with external resources or narrow the search

#### 4. Data Normalization
- **Tags** – Designate descriptive names for key-value pairs (labels); useful to search events with specific field values  
- **Field Aliases** – Normalize data over multiple sources; assign one or more aliases to extracted fields and apply fields to a lookup table

#### 5. Data Models (Search-Time Mapping)
- **Hierarchically structured datasets** – Consist of events, searches, and/or transactions

---

## 📝 Creating Reports

- Use reports to easily share information with others  
- Since my data had limited info, I saved a visualization showing **which day had the most attacks**

> **Note:** Naming conventions for reports vary by company

### How to Access and Use Reports:
- Go to **Reports tab** from the application menu  
- Click title to run or open in search  
- Use arrow to expand and view:
  - Creator
  - App context
  - Permissions

### Edit Menu Options:
- **Edit Description**  
- **Edit Permission**  
  - By default, reports are private to the owner  
  - To allow others to view, go to “Display for” → choose “App” and set read/write access  
  - Only admins can display reports across all apps  
  - Power users can be granted read/write for app-level sharing
- **Run As Dialog**  
  - Run as owner OR as the user executing the report  
- **Edit Schedule**  
  - Reduces strain from repeated ad hoc searches  
  - Warns that scheduling overrides “Run As” setting  
  - Options: hourly, daily, weekly, monthly or cron  
  - Specify time range and schedule window  
  - Trigger actions:
    - Send via email
    - Post to external URL (webhook)
    - Run custom script  
- **Edit Acceleration**  
- Links to: **Clone**, **Embed**, **Delete**

---

## 📊 Creating Dashboard

I used data from:  
🔗 [DHCP Log Analysis – Splunk Project #7](https://github.com/0xrajneesh/Splunk-Projects-For-Beginners/blob/main/project%237-analyzing-dhcp-logs-using-splunk-siem.md)

---

### 🔧 Data Parsing

Before creating the dashboard, I learned how to **Extract New Fields**:

1. Chose an event from the list  
2. On **Select Method**, I chose **Regular Expression**  
3. On **Select Fields**, I extracted:
   - Source IP → `src_ip`  
   - Destination IP → `dst_ip`  
4. On **Validate**, ensured no incorrect values were highlighted  
5. On **Save**, I could define permission scope:
   - Private (only me)
   - Shared within the app
   - Shared across all apps

---

### 📈 Creating Dashboards

#### 1. First Panel: Top Destination IPs (`dst_ip`)
- In Visualization, chose **Pie Chart**
- From **Save As**, selected:
  - Report
  - Alert
  - Existing Dashboard
  - **New Dashboard**

#### 2. New Dashboard Prompt:
- Added a title  
- Set permission:  
  - Private  
  - Shared in App  
- Selected type:
  - **Classic Dashboard**
  - **Dashboard Studio**

#### 3. Second Panel: Top Source IPs (`src_ip`)
- In visualization, changed **legend** from right to top  
- Saved to existing dashboard

---

### 🛠️ Dashboard Page Features

When clicking **Edit**, I could add panels:

#### Add Panel Options:
- **New** – Create from scratch  
- **New from Report** – Build from saved reports  
- **Clone from Dashboard** – Copy from another dashboard  
- **Prebuilt Panel**

#### Other Options:
- View and edit **XML source**  
- Add input fields  
- Toggle between **Dark** and **Light** theme

#### Panel Tools:
- **Edit Search**  
- **Select Visualization** – Modify chart formats  
- **More Actions**:
  - **Edit Drilldown**  
  - **Trellis Layout**

---

## 🧪 Dashboard Studio

From the dashboard I created, I clicked the 3-dot menu and chose **Clone in Dashboard Studio**.

### Clone Popup:
- **Layout Mode Options**:
  - **Absolute** – Pixel-perfect, fully customizable placement  
  - **Grid** – Snap-aligned, organized in rows

### Dashboard Studio Features:
- Top Controls:
  - Add new visualization  
  - Add input  
  - Add markdown text  
  - Show/hide configuration panel  
  - Configure data sources  
  - Edit dashboard JSON

---





