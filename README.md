# 🤖 AI Resume Screening System

An AI-powered Resume Screening System that automatically parses resumes, extracts structured information, compares candidates against a job description using an LLM, and ranks applicants based on their suitability.

## 🚀 Features

- 📄 Parse PDF and DOCX resumes
- 🧠 AI-powered resume parsing using LLM
- 📋 AI-powered job description parsing
- ✅ Extract structured information using Pydantic
- 🎯 Match candidates with job requirements
- 📊 Generate compatibility scores (0–100)
- 🏆 Rank candidates from best to worst
- 🔍 Display Top 2 and Lowest 2 candidates
- 💬 Provide AI-generated feedback on strengths and missing skills

---

## 🛠️ Tech Stack

- Python
- Groq API
- GPT OSS Model
- Pydantic
- PyPDF
- python-docx
- dotenv

---

## 📂 Project Structure

```
resume-screening/
│
├── resumes/
│   ├── resume1.pdf
│   ├── resume2.docx
│
├── resume_parser.py
├── requirements.txt
├── .env
└── README.md
```

---

## ⚙️ How it Works

### Step 1
Parse the Job Description using an LLM.

Extract:
- Role
- Required Skills
- Preferred Skills
- Responsibilities
- Minimum Experience
- Education Requirements

### Step 2
Parse each Resume.

Extract:
- Name
- Email
- Phone
- Skills
- Experience
- Education
- Projects
- Certifications

### Step 3
Compare Resume with Job Description.

The LLM evaluates:

- Skill Match
- Missing Skills
- Experience Match
- Overall Compatibility Score
- Final Verdict

### Step 4
Sort all candidates by score.

Display:
- Top Candidates
- Lowest Candidates

---

## Example Output

```
Processing: Abhay Singh.pdf
Score: 73%

Processing: Ashish Raj.pdf
Score: 80%

TOP 2 Candidates

Ashish Raj - 80%
Anshit Verma - 70%

LOWEST 2 Candidates

Abhay Singh - 60%
Priyanshu Singh - 58%
```

---

## Installation

Clone the repository

```bash
git clone https://github.com/yourusername/AI-Resume-Screening.git
```

Install dependencies

```bash
pip install -r requirements.txt
```

Create a `.env` file

```env
GROQ_API_KEY=your_api_key
```

Run the project

```bash
python resume_parser.py
```

---

## Future Improvements

- Streamlit Web Interface
- Resume Upload Portal
- Export Results to Excel/CSV
- Semantic Search using Embeddings
- Vector Database Integration
- ATS-style Score Breakdown
- Batch Processing Optimization

---

## Learning Outcomes

This project demonstrates:

- Prompt Engineering
- Structured Output (JSON Schema)
- Pydantic Validation
- Resume Parsing with LLMs
- Job Description Analysis
- Candidate Ranking
- LLM Application Development

---

## License

This project is licensed under the MIT License.

---

⭐ If you found this project useful, consider giving it a star!
