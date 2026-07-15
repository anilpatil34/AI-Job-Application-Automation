# 🤖 AI Job Application Automation Workflow

> An AI-powered job application automation workflow built with **n8n**, **JavaScript**, **REST APIs**, and **Google Gemini AI**. The workflow automatically fetches live job listings, filters relevant opportunities, analyzes job descriptions using AI, and generates intelligent job recommendations.

---

## 📌 Project Overview

Searching and evaluating hundreds of job postings manually is time-consuming. This workflow automates the process by integrating a public Job Board API with Google Gemini AI to identify suitable job opportunities based on predefined criteria.

The workflow demonstrates practical skills in workflow automation, API integration, JavaScript data processing, AI integration, and automation design.

---

## 🚀 Features

- ✅ Fetches live job listings from a public Job API
- ✅ Extracts job title, company, description, and application URL
- ✅ Filters relevant jobs using JavaScript
- ✅ Processes each job individually using Loop Over Items
- ✅ Integrates Google Gemini AI for intelligent job analysis
- ✅ Generates AI Match Score
- ✅ Identifies missing skills
- ✅ Provides AI recommendation on whether to apply
- ✅ Modular and reusable workflow built in n8n

---

# 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| n8n | Workflow Automation |
| JavaScript | Data Processing & Filtering |
| REST API | Fetch Job Listings |
| HTTP Request | API Integration |
| Google Gemini AI | AI Job Analysis |
| JSON | Data Exchange |

---

# 📷 Workflow Overview

![Workflow Overview](screenshots/workflow-overview.png)

---

# ⚙️ Workflow Architecture

```
Manual Trigger
      │
      ▼
HTTP Request
(Fetch Live Jobs)
      │
      ▼
JavaScript
(Parse Job Data)
      │
      ▼
JavaScript
(Filter Relevant Jobs)
      │
      ▼
Loop Over Items
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
AI Job Recommendation
```

---

# 🔄 Workflow Steps

### 1️⃣ Manual Trigger

Starts the automation workflow manually inside n8n.

---

### 2️⃣ Fetch Jobs

Retrieves live job listings from the Arbeitnow Job Board API.

Extracted fields include:

- Job Title
- Company Name
- Description
- Application URL

---

### 3️⃣ Parse Response

JavaScript extracts only the required fields from the API response.

---

### 4️⃣ Filter Jobs

Filters relevant jobs based on predefined keywords such as:

- Python
- Backend

Only matching jobs continue through the workflow.

---

### 5️⃣ Loop Through Jobs

Processes each selected job individually.

---

### 6️⃣ AI Job Analysis

Each job description is sent to Google Gemini AI.

The AI evaluates:

- Job Match Score
- Missing Skills
- Recommendation
- Reasoning

---

### 7️⃣ Parse AI Response

JavaScript converts the AI response into structured JSON.

Example:

```
{
  "score": 88,
  "reason": "Strong Python and REST API match",
  "missing_skills": [
      "Docker",
      "AWS"
  ],
  "apply": true
}
```

---

# 📁 Repository Structure

```
AI-Job-Application-Automation/
│
├── README.md
├── workflow.json
├── .gitignore
│
└── screenshots/
      ├── workflow-overview.png
      └── execution-result.png
```

---

# ▶️ Getting Started

## Clone Repository

```bash
git clone https://github.com/anilpatil34/AI-Job-Application-Automation.git
```

---

## Import Workflow

1. Open n8n
2. Create a New Workflow
3. Click **Import from File**
4. Select

```
workflow.json
```

---

## Configure API

Add your own Google Gemini API Key before running the workflow.

> **Note:** Never commit your API key to GitHub.

---

## Execute Workflow

Click

```
Execute Workflow
```

The workflow will automatically:

- Fetch Jobs
- Filter Jobs
- Analyze Jobs using AI
- Return AI Recommendations

---

# 📊 Skills Demonstrated

- Workflow Automation
- JavaScript
- REST API Integration
- HTTP Requests
- JSON Processing
- AI Integration
- Prompt Engineering
- Data Filtering
- Problem Solving
- Automation Design

---

# 💡 Future Improvements

- Resume Parsing
- ATS Resume Matching
- AI Resume Customization
- AI Cover Letter Generation
- LinkedIn Job Search
- Naukri Integration
- Indeed Integration
- Google Sheets Logging
- Email Notifications
- Automatic Job Applications

---

# 🎯 Learning Outcomes

This project demonstrates practical experience with:

- Designing automation workflows
- Working with REST APIs
- Processing JSON data
- Integrating Generative AI into real-world workflows
- Building modular automation pipelines
- Using JavaScript inside n8n

---

# 👨‍💻 Author

**Anil Patil**

Full Stack Developer | AI & Automation Enthusiast

- GitHub: https://github.com/anilpatil34
- LinkedIn: https://www.linkedin.com/in/anil-patil-b1a726241/

---

# ⭐ If you found this project useful

Please consider giving the repository a ⭐ on GitHub.
