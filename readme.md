# 🏅 Tokyo Olympics Azure Data Engineering Project

This project demonstrates how to build a dynamic, parameterized data pipeline using **Azure Data Factory** to extract Olympic datasets from a public GitHub repository and load them into **Azure Data Lake Storage Gen2**.

## 📦 Project Overview

- Ingests multiple CSV files (Athletes, Coaches, Teams, etc.) from GitHub
- Uses **HTTP Linked Service** and **parameterized datasets**
- Dynamically stores data into a **`raw-data` folder** in the `dynamic-olympic` container in Azure Data Lake (`ahmeddlsgen2` account)
- Integrated with **GitHub DevOps** for source control and versioning

## 🧰 Tools & Technologies

- Azure Data Factory
- Azure Data Lake Gen2
- GitHub DevOps Integration
- REST API (HTTP connector)
- Parameterized pipelines & datasets

## 🔁 Pipeline Flow

1. Dynamically reads CSV files from GitHub using an HTTP dataset
2. Uses parameters to make the pipeline reusable for multiple files
3. Writes the files into Azure Data Lake in `/raw-data/` directory
4. GitHub integration enables CI/CD and collaborative development

## 📂 Example Files Ingested

- Athletes.csv  
- Coaches.csv  
- Teams.csv  
- Medals.csv  
- EntriesGender.csv

## 📌 Getting Started

To reuse or extend this project:
1. Clone this repo
2. Connect your ADF instance to GitHub using this repo
3. Replace Linked Service credentials with your own
4. Publish and trigger the pipeline

## 🙋‍♂️ Author

**Ahmed Hassan Abdelmohsen**

---

