Automated Reporting Pipeline – Outlook to Power BI Integration
🚀 Project Overview

This project demonstrates an end-to-end automated reporting pipeline that integrates:

Microsoft Outlook

Microsoft Power Automate

Google Drive

Google Cloud Platform (API)

Python

Microsoft Power BI

The objective of this solution is to eliminate manual file handling, automate data ingestion, and enable real-time reporting for credit score analysis.

🧩 Problem Statement

Field agents were sending credit score reports via email attachments.
Manually downloading, organizing, transforming, and visualizing this data was:

Time-consuming

Error-prone

Not scalable

This project automates the entire workflow from email receipt to dashboard visualization.

⚙️ Architecture Workflow
1️⃣ Email Segregation

Created a rule in Outlook to filter agent emails.

Conditions:

Email must contain an attachment

Subject must contain "Credit Score"

Emails must be moved to Filed Agent Reports folder

2️⃣ Automation Using Power Automate

Built an Automated Cloud Flow

Automatically transfers attachments from Outlook to Google Drive

Files stored inside a dedicated folder: Field Agent Reports

3️⃣ Google Drive API Integration

Created API credentials using Google Cloud Platform

Enabled Google Drive API access

Established secure authentication flow

4️⃣ Python as Data Bridge

Python acts as the transportation layer between Google Drive and Power BI.

Libraries used:

pip install google-auth google-auth-oauthlib google-auth-httplib2 google-api-python-client pandas

Handled environment configuration issues:

Resolved pip.exe not recognized error

Configured system PATH variables for Python installation

5️⃣ Power BI Integration

Connected Power BI to Google Drive via Python script

Imported sample files for transformation (best practice to avoid transforming full dataset initially)

Created reusable transformation logic

6️⃣ Data Modeling & Visualization

Performed structured data transformation

Built interactive dashboards

Implemented DAX measures such as:

Average Credit Enquiry = AVERAGEX(Table, Table[CreditEnquiry])
📈 Key Features

✔ Fully automated email-to-dashboard pipeline
✔ API-based cloud integration
✔ Secure authentication with Google Drive
✔ Python-powered data transportation
✔ Scalable transformation logic
✔ Dynamic Power BI dashboards

🏗 Tech Stack

Microsoft Outlook

Microsoft Power Automate

Google Drive API

Google Cloud Platform

Python (pandas, google-api-client)

Microsoft Power BI

DAX

🎯 Business Impact

Eliminates manual file downloads

Reduces reporting turnaround time

Ensures centralized and structured data storage

Enables real-time performance tracking

Scalable automation framework

💡 What I Learned

End-to-end automation architecture design

API authentication & integration

Environment troubleshooting & PATH configuration

Efficient data modeling strategy in Power BI

Importance of transforming sample files before full-scale deployment

🔮 Future Enhancements

Scheduled refresh automation

Error handling & logging mechanism

Automated notification system for failed flows

Migration to fully cloud-native architecture

If you found this project helpful or interesting, feel free to ⭐ the repository.
