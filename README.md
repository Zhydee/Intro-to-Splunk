# Intro to Splunk
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

 ## 🆕 New Search Interface Components
 
## 💾 Save As Menu

The **Save As Menu** allows you to save your search as a knowledge object for future reuse and sharing.

## 🔍 Search Interface Components

### 🗂️ Search Result Tabs
- **Event Tab** – Displays events returned for the search.
- **Pattern Tab** – Allows you to see patterns in the data.
- **Statistic / Visualization Tabs** – Display search-generated statistics or visualizations.

---

### ⚙️ Search Action Button

The **Search Action Button** provides quick access to several actions for managing your search jobs:

- **Edit Job Setting**
- **Send to Background**
- **Inspect Search Jobs**
- **Delete Search Jobs**

---

### 📤 Export Icon

Use the **Export Icon** to download your search results in the following formats:

- **Raw**
- **CSV**
- **XML**
- **JSON**

---

### 🔄 Search Mode Selector
- **Fast Mode** – Cuts down on field info; only returns default and required fields.
- **Smart Mode** – Toggles behavior based on the type of search run.
- **Verbose Mode** – Returns all fields and events; discovers everything possible.

---

### 🕒 Timeline
- Dynamically adjusted based on the time range chosen in the **Time Range Picker**.
- You can select a specific range on the timeline to investigate further.

---

### 📃 Event List
Displays a list of matching events for the query.

---

### 🧾 Field Sidebar

The **Field Sidebar** helps users explore fields extracted from the events in their search results. It contains two main sections:

- **Selected Fields** – Default fields included in the search results.
- **Interesting Fields** – Fields extracted by Splunk based on metadata analysis and relevance.

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

Mastering Splunk search syntax helps extract meaningful results. Below are useful techniques with visual examples.

---

### 1. 🔎 Wildcard Search  
Add `*` at the end of a word to return events that start with that word.

---

### 2. 🔤 Case Insensitive  
Search is not case sensitive – all matching results are returned.

---

### 3. ⚖️ Boolean Operators  
Used with multiple terms (evaluated in this order):  
- `NOT`, `OR`, `AND`

> 💡 Use parentheses `()` to control the evaluation order.

---

### 4. 🗣️ Exact Phrase  
Place quotes `" "` around phrases for exact matching.

---

### 5. 🧩 Escaping Quotes  
Use backslash `\` to escape multiple quotes inside a search term.


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

### 📊 How to Access and Use Reports:

- Go to **Reports tab** from the application menu  

- Click title to run or open in search  
- Use arrow to expand and view:
  - Creator  
  - App context  
  - Permissions  

---

### ⚙️ Edit Menu Options:

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
- **Clone**, **Embed**, **Delete**



## 📊 Creating Dashboard

I used data from:  
🔗 [DHCP Log Analysis – Splunk Project #7](https://github.com/0xrajneesh/Splunk-Projects-For-Beginners/blob/main/project%237-analyzing-dhcp-logs-using-splunk-siem.md)

---

### 🔧 Data Parsing

Before creating the dashboard, I learned how to **Extract New Fields**:

1. Choose an event from the list  
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

### 💾 Save As Options

From the **Save As** menu, you can choose to save the current search as:

- **Report**
- **Alert**
- **Existing Dashboard**
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

- In the visualization, changed the **legend** position from **right** to **top**  
- Saved the panel to an existing dashboard

---

### 🛠️ Dashboard Page Features

When clicking **Edit**, you can add panels using various methods:

---

#### ➕ Add Panel Options

- **New** – Create from scratch  
- **New from Report** – Build from saved reports  
- **Clone from Dashboard** – Copy from another dashboard  
- **Add Prebuilt Panel**  

---

#### ⚙️ Other Options

- View and edit **XML source**  
- Add input fields  
- Toggle between **Dark** and **Light** theme

---

#### 📊 Tools on Each Chart Panel

- **Edit Search**
- **Select Visualization** – Modify chart formats
- **More Actions:**
  - **Edit Drilldown**
  - **Trellis Layout**


## 🧪 Dashboard Studio

From the dashboard I created, I clicked the 3-dot menu and chose **Clone in Dashboard Studio**.

### 📋 Clone Popup

- **Layout Mode Options**:
  - **Absolute** – Pixel-perfect, fully customizable placement  
  - **Grid** – Snap-aligned, organized in rows

---

### 🧰 Dashboard Studio Features

- **Top Controls**:
  - Add new visualization  
  - Add input  
  - Add markdown text  
  - Show/hide configuration panel  
  - Configure data sources  
  - Edit dashboard JSON  

---
