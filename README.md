# Automated-AI-driven-discovery-of-the-exact-technologies-powering-any-company.
Automated n8n workflow that scans BuiltWith + AI to list any company’s real tech stack (CMS, analytics, hosting, security) straight into Google Sheets—zero code, batch ready.
| Feature                          | Benefit                                                                                                      |
| -------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| **AI-Powered Extraction**        | Uses OpenAI GPT-4.1-mini to parse BuiltWith data and identify only *actual* technologies—no marketing fluff. |
| **Zero-Code**                    | Drag-and-drop n8n workflow—works out of the box.                                                             |
| **Batch Processing**             | Handles hundreds of domains in one run via `Loop Over Items`.                                                |
| **Real-Time Google Sheets Sync** | Inserts or updates rows automatically in the connected Google Sheet.                                         |
| **Extensible Schema**            | JSON-schema based structured output makes it trivial to add new fields.                                      |

Tech Stack
n8n – workflow orchestration
OpenAI GPT-4.1-mini – language model for intelligent parsing
Google Sheets API – data persistence
BuiltWith – raw technology intelligence
Jina.ai Reader – fast, clean HTML→text conversion

Quick Start
Clone or fork this repo.
Import finding-company-technologies.json into your n8n instance.
Connect credentials:
Google Sheets OAuth2
OpenAI API key
Update the Google Sheet ID in the two Google-Sheets nodes (or leave the demo sheet for testing).
Add your company domains in column Company Domain.
Hit “Execute Workflow”—watch the sheet populate.
