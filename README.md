# Project 1: Live Data Automation & AI Processing with n8n and Google Gemini

A production-ready n8n automation workflow designed to fetch data from Google Sheets, perform external HTTP web research, process the retrieved information using the Google Gemini Chat Model, and automatically save the structured AI output back into Google Sheets.

## 🚀 Workflow Overview
This workflow automates the tedious process of manual web research and content/data enrichment by leveraging advanced Generative AI and structured workflows.

### ⚙️ How It Works (Node by Node)
1. **Manual/Scheduled Trigger**: Initiates the workflow sequence (`When clicking 'Execute workflow'`).
2. **Data Retrieval**: Connects to the Google Sheets API to read targeted live rows or specific input data (`Get row(s) in sheet`).
3. **External Research via HTTP**: Sends dynamic web requests to scrapers or external APIs to collect real-time online data (`HTTP Request`).
4. **AI Processing (LLM Chain)**: Utilizes n8n's `Basic LLM Chain` connected to the **Google Gemini Chat Model** to intelligently parse, summarize, or analyze the data based on precise system prompts.
5. **Data Enrichment**: Writes the structured, finalized AI responses directly back into the specified Google Sheet row (`Append or update row in sheet`).

## 🛠️ Architecture & Tech Stack
* **Automation Platform:** n8n
* **AI Model:** Google Gemini Chat Model
* **Integrations:** Google Sheets API, HTTP Request Protocol

## 📂 Project Structure
* `workflow.json` - The complete exportable JSON file of this n8n configuration.
* `README.md` - Documentation for the workflow execution.

## 🚀 How to Import and Use
1. Copy the contents of the `workflow.json` file from this repository.
2. Open your n8n instance and create a new workflow.
3. Paste the copied JSON (`Ctrl+V` or `Cmd+V`) directly into the n8n canvas.
4. Configure your credentials for **Google Sheets** and **Google Gemini Chat Model**.
5. Save and execute the workflow!
6.
