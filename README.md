README.md
🤖 AI Job Application Automation Workflow
Overview

This project is an AI-powered job application automation workflow developed using n8n, JavaScript, REST APIs, and Google Gemini AI. It automates the process of discovering job opportunities, filtering relevant positions, and analyzing job descriptions to determine whether a job matches a candidate's profile.

Instead of manually searching and reviewing hundreds of job postings, the workflow intelligently performs these tasks and returns AI-based recommendations.

Features
Fetches live job listings from a public Job Board API.
Extracts important job details.
Filters jobs based on keywords.
Processes each job individually.
Uses Google Gemini AI to analyze job descriptions.
Generates AI Match Score.
Identifies missing skills.
Recommends whether to apply.
Built using a no-code/low-code automation platform (n8n).
Workflow Architecture
Manual Trigger
       │
       ▼
HTTP Request
(Get Live Jobs)
       │
       ▼
JavaScript
(Parse API Response)
       │
       ▼
JavaScript
(Filter Relevant Jobs)
       │
       ▼
Loop Over Jobs
       │
       ▼
HTTP Request
(Google Gemini AI)
       │
       ▼
JavaScript
(Parse AI Response)
       │
       ▼
AI Recommendation
Technologies Used
n8n
JavaScript
REST API
HTTP Request
Google Gemini AI API
JSON
AI Prompt Engineering
Workflow Automation