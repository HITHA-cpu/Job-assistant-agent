# Job Assistant Backend – LLM Resume Scorer Module

This module of the **Job Assistant AI Backend** enables automated resume evaluation using AI. It securely connects to OpenAI (or compatible APIs), parses resumes in PDF/DOCX formats, and generates intelligent score reports using a Large Language Model (LLM).

---

##  Features
- **API Key Integration:** Securely loads `OPENAI_API_KEY` from `.env` using `dotenv`.
- **Resume Parsing:**
  - PDF → Parsed via [`pdf-parse`](https://www.npmjs.com/package/pdf-parse)
  - DOCX → Parsed via [`mammoth`](https://www.npmjs.com/package/mammoth)
- **LLM Resume Scorer Agent:**
  - Analyzes extracted resume text using OpenAI or compatible APIs.
  - Returns overall score, key strengths, and improvement areas.
  - Handles errors (missing key, quota exceeded, invalid file) gracefully.

---

##  Setup & Installation

### Clone the project
```bash
git clone <your-repo-url>
cd Job-assistant-agent
