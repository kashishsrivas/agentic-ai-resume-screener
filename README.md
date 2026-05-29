# Agentic AI Resume Screening Pipeline

An automated backend workflow built in **n8n** that parses job descriptions and candidate resumes, leverages generative AI to evaluate skills alignment, and exports a structured assessment dashboard.

## 🚀 Features
- **Automated Ingestion:** Captures PDF documents via a webhook/form submission wrapper.
- **AI-Powered Evaluation:** Uses the **Google Gemini 2.5 Pro** model to dynamically map candidate credentials against a target Job Description.
- **Data Structuring:** Implements a JavaScript node to clean up, validate, and structure the AI's output array.
- **Automated Reporting:** flattens the processed data and exports it seamlessly into a structured CSV file.

## 🛠️ Tech Stack
- **Orchestration:** n8n
- **AI Model:** Google Gemini 2.5 Pro API
- **Data Manipulation:** JavaScript / Node.js
- **Data Target:** CSV Spreadsheet

## 📋 How to Import & Run
1. Download the `workflow.json` file from this repository.
2. Open your local n8n instance (`http://localhost:5678`).
3. Create a blank canvas, click the menu (`...`) in the top right, and select **Import from File**.
4. Configure your Google Gemini credentials in the chat model node.
5. Hit **Execute workflow**!
