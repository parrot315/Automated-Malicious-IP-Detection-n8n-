# Automated Malicious IP Detection using n8n

An automated Security Operations Center (SOC) workflow built with **n8n** to identify malicious IP addresses using the **AbuseIPDB API**. The workflow analyzes a list of IP addresses, filters those with a high abuse confidence score, and stores the results in **Google Sheets** for further investigation and reporting.

---

## Project Overview

This project demonstrates how workflow automation can simplify threat intelligence tasks in a SOC environment. Instead of manually checking every IP address, the workflow automatically queries the AbuseIPDB API, evaluates the results, and records malicious IPs for analysts.

---

## Features

- Automated IP reputation analysis
- Integration with the AbuseIPDB Threat Intelligence API
- Filters malicious IPs using a configurable confidence score threshold
- Stores malicious IP information in Google Sheets
- Built using n8n low-code automation
- Easy to customize for additional threat intelligence sources

---

## Workflow

1. Manual trigger starts the workflow.
2. A predefined list of IP addresses is loaded.
3. Each IP is processed individually.
4. The AbuseIPDB API is queried for reputation data.
5. IPs with an Abuse Confidence Score above the threshold are identified.
6. The following information is extracted:
   - IP Address
   - Abuse Confidence Score
   - Country
   - Total Reports
   - Last Reported Date
7. Results are automatically appended to a Google Sheets document.

---

## Technologies Used

- n8n
- JavaScript
- AbuseIPDB API
- Google Sheets API
- REST API
- JSON

---

## Project Structure

```
n8n-malicious-ip-detection/
│
├── README.md
├── workflow.json
└── screenshots/
    ├── workflow.jpg
    └── result.jpg
```

---

## Setup

### Requirements

- n8n
- AbuseIPDB API Key
- Google Account
- Google Sheets Credentials configured in n8n

### Steps

1. Clone this repository.
2. Import `workflow.json` into n8n.
3. Replace the placeholder AbuseIPDB API key with your own.
4. Configure Google Sheets credentials.
5. Execute the workflow.

---

## Example Output

For every malicious IP detected, the workflow stores:

| Field | Description |
|-------|-------------|
| IP Address | Suspicious IP |
| Abuse Score | Abuse Confidence Score |
| Country | Country Code |
| Reports | Total Abuse Reports |
| Last Reported | Latest Abuse Report Date |

---

## Screenshots

### Workflow

Add your workflow screenshot here.

### Result

Add your Google Sheets output screenshot here.

---

## Future Improvements

- Integrate VirusTotal API
- Email or Slack notifications
- Real-time monitoring using Webhooks
- Automatic report generation
- Dashboard visualization
- Support multiple threat intelligence providers

---

## Security Notice

This repository does **not** include API keys or credentials.

Before using the workflow, replace the placeholder API key with your own AbuseIPDB API key.

---

## Learning Outcomes

This project demonstrates practical knowledge of:

- Security Automation
- Threat Intelligence
- SOC Workflow Automation
- REST API Integration
- JSON Processing
- JavaScript in n8n
- Google Sheets Automation

---

## Author

**Ali Haider**

Cybersecurity Student | SOC & Cloud Security Enthusiast

GitHub: https://github.com/parrot315

LinkedIn: https://www.linkedin.com/in/ali-haider-57901a383
