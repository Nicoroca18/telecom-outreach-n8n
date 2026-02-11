# n8n Complete Email Automation

This n8n workflow automates outbound B2B email campaigns. It extracts company and contact data from Google Sheets/Drive, enriches it with web and LinkedIn info, generates personalized emails with AI, evaluates them, updates a CRM-like system, and sends Slack notifications after each run.

## Features

- **Google Drive Trigger:** Watches a folder for new Excel/CSV files.
- **Data Extraction:** Pulls company and contact info from files.
- **Web & LinkedIn Scraping:** Reads website and LinkedIn pages for enrichment.
- **AI Email Generation:** Creates initial emails and follow-ups in multiple languages.
- **AI Email Evaluation:** Scores emails and suggests improvements.
- **Email Mapping:** Prepares final email content for sending.
- **CRM Integration:** Updates a data table with sent emails and company info.
- **Slack Notifications:** Sends workflow completion updates.
- **File Upload:** Stores processed files in a target Google Drive folder.

## How It Works

1. Watch a folder in Google Drive for new files.
2. Extract data from uploaded Excel sheets.
3. Clean and merge company/contact data.
4. Scrape website and LinkedIn pages for extra context.
5. Use AI to generate personalized emails and follow-ups.
6. Evaluate emails with AI to ensure quality.
7. Map final email content and store it in the data table.
8. Notify via Slack and upload processed files to Google Drive.

## Setup

1. Clone this repo:

   ```bash
   git clone https://github.com/Nicoroca18/telecom-outreach-n8n.git
   cd n8n-complete-email-automated
	
2.	Install dependencies:
 	```bash
   	npm install
   	```
   
3.	Configure credentials for:

	•	Google Drive
	•	Slack
	•	AI model (Google Gemini)
	•	Hunter API (optional)


4. Import the workflow JSON into your n8n instance.

5. Start n8n:
	```
	n8n start
	```


Notes

- All AI prompts and outputs are contained in the workflow nodes.
- Replace placeholder credentials with your own before running.
- The workflow is modular—nodes can be updated or replaced without breaking the flow.
- Use only with non-confidential test data if sharing publicly.



  
