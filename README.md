# 👤 ATS Resume Analyzer

An AI-powered **Applicant Tracking System (ATS) Resume Analyzer** built with **Streamlit** and **Groq Llama 3.1**. The application compares resumes with a job description, calculates an ATS match score, identifies strengths and weaknesses, highlights missing keywords, and ranks multiple resumes based on their compatibility with the job requirements.

---

## 🚀 Features

### 📄 Single Resume Analysis
- Upload a PDF resume.
- Paste the Job Description (JD).
- AI-generated ATS match score.
- Resume summary.
- Key strengths and weaknesses.
- Missing keywords from the JD.
- Personalized suggestions to improve the resume.

### 📊 Multiple Resume Ranking
- Upload multiple PDF resumes.
- Compare each resume against the same job description.
- Rank candidates based on ATS score.
- Identify the top candidate.
- Download the ranking report as a CSV file.

---

## 🛠️ Tech Stack

- Python
- Streamlit
- Groq API (Llama 3.1-8B Instant)
- pdfplumber
- Pandas
- Regular Expressions (re)

---

## 📂 Project Structure

```
ATS-Resume-Analyzer/
│
├── app.py                 # Main Streamlit application
├── requirements.txt       # Project dependencies
├── .env                   # API key (optional)
├── .gitignore
├── README.md
```

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/MohammedZahid05/ATS-Resume-Analyzer.git
```

### 2. Navigate to the Project

```bash
cd ATS-Resume-Analyzer
```

### 3. Create a Virtual Environment

Windows

```bash
python -m venv venv
```

Activate it

```bash
venv\Scripts\activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 Configure the Groq API Key

Replace the placeholder API key in `app.py`:

```python
client = Groq(api_key="YOUR_API_KEY")
```

with your own Groq API key:

```python
client = Groq(api_key="gsk_your_api_key")
```

> **Recommended:** Store your API key in a `.env` file instead of hardcoding it.

Example:

```env
GROQ_API_KEY=your_api_key
```

---

## ▶️ Run the Application

```bash
streamlit run app.py
```

Open your browser and visit:

```
http://localhost:8501
```

---

## 📋 How to Use

### Single Resume Analysis

1. Enter the Job Description.
2. Upload a PDF resume.
3. Click **Analyze Resume**.
4. View:
   - ATS Match Score
   - Resume Summary
   - Strengths
   - Weaknesses
   - Missing Keywords
   - Suggestions for Improvement

### Multiple Resume Ranking

1. Enter the Job Description.
2. Upload multiple PDF resumes.
3. Click **Rank Resumes**.
4. View ranked candidates.
5. Download the ranking report as a CSV file.

---

## 📊 Output

For each resume, the application provides:

- ATS Match Percentage
- Resume Summary
- Key Strengths
- Key Weaknesses
- Missing Keywords
- Resume Improvement Suggestions

For multiple resumes:

- Candidate Ranking
- Highest Scoring Candidate
- CSV Report Download

---

## 📦 Dependencies

```
streamlit
groq
pdfplumber
pandas
```

Install all dependencies using:

```bash
pip install -r requirements.txt
```
