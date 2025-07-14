<img width="1920" height="1080" alt="Screenshot (83)" src="https://github.com/user-attachments/assets/a44cc976-ef9e-4ba6-acaa-5ae5ed3587fc" />

# 🚀 Data Engineering Assignment – Azure Data Factory Based Workflows

This project showcases multiple real-world Data Engineering tasks implemented using **Azure Data Factory (ADF)**, **Azure SQL Database**, **Blob Storage**, and **Self-hosted Integration Runtime (SHIR)**.

---

## 📌 Objective

To design and implement cloud-based data pipelines to handle structured data from on-premise and external sources using ADF, with advanced orchestration, transformation, and automation features.

---

## ✅ Tasks Covered

### 🔹 Task 1: Extract Data from Local Server via SHIR and Load into Azure SQL Database

- **Configured SHIR** (Self-hosted Integration Runtime) on a local machine to connect on-premise data to Azure
- Created a pipeline to:
  - Read threshold value from a local/Blob-based CSV file
  - Lookup row count from Azure SQL Customer table
  - Conditionally copy data to Blob Storage in JSON format (if count > threshold)
- **Technologies**: Azure Data Factory, Blob Storage, Azure SQL DB, Lookup Activity, If Condition, Copy Activity

---

### 🔹 Task 2: Connect to FTP/SFTP Server and Extract Data

- Configured **Linked Service** to securely connect to an external **FTP/SFTP server**
- Extracted remote files and stored them in **Azure Blob Storage**
- Built ADF pipeline to automate FTP data ingestion

---

### 🔹 Task 3: Incremental Load Pipeline with Daily Automation

- Designed pipeline using **Watermarking Technique** for incremental load
- Scheduled with **daily triggers**
- Only new or updated records were processed, improving performance

---

### 🔹 Task 4: Schedule Pipeline to Run on the Last Saturday of Each Month

- Created **custom time-based trigger**
- Used **ADF expression logic** to identify last Saturday
- Automated monthly batch processing for periodic reporting

---

### 🔹 Task 5: Implement Retry Logic in Data Pipelines

- Handled **transient failures** using:
  - **Retry policies** on activities
  - Wait + Retry pattern using `Until`, `Wait`, and `Set Variable` activities
- Improved pipeline **resilience and reliability**

---

## 🛠️ Tools & Services Used

- **Azure Data Factory (ADF)**
- **Azure SQL Database**
- **Azure Blob Storage**
- **FTP/SFTP Linked Service**
- **Self-hosted Integration Runtime (SHIR)**
- **Triggers (Schedule, Custom)**
- **Pipeline Activities**: Lookup, If Condition, Copy, Wait, Set Variable, Until

---

## 📁 Folder Structure

