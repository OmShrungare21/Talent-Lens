# 🔍 TalentLens — AI-Powered Resume Screener

**TalentLens** is an AI-powered resume screening system that helps recruiters evaluate and rank candidates against a given job description. By analyzing resumes in PDF and DOCX formats, it identifies relevant skills, highlights missing requirements, calculates candidate match scores, and generates structured hiring recommendations using the Groq LLM API.

## 🚀 Key Features

- 📄 **Resume Parsing:** Extract information from PDF and DOCX resumes.
- 🤖 **AI-Powered Analysis:** Use a large language model to evaluate candidate profiles against job requirements.
- 🎯 **Skill Matching:** Identify relevant skills and missing qualifications.
- 📊 **Match Score Calculation:** Estimate how closely a candidate's resume aligns with a job description.
- 🏆 **Candidate Ranking:** Compare and rank candidates according to their match scores.
- 💡 **Hiring Recommendations:** Generate structured insights to support recruiter decision-making.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Core application logic |
| Groq API | AI-powered resume analysis |
| Pydantic | Structured data validation |
| PyPDF | PDF text extraction |
| python-docx | DOCX document processing |
| uv | Python dependency and environment management |

## ⚙️ How It Works

1. **Provide a job description:** Enter the role requirements and desired skills.
2. **Upload resumes:** Supply candidate resumes in supported PDF or DOCX formats.
3. **Extract resume information:** The system reads the documents and extracts relevant text.
4. **Analyze candidates:** AI evaluates the extracted information against the job requirements.
5. **Calculate match scores:** Candidate profiles are assessed for relevance to the role.
6. **Rank candidates:** Candidates are organized by their match scores.
7. **Review recommendations:** Recruiters use the generated insights to support their shortlisting decisions.

## 📦 Prerequisites

Before running TalentLens, ensure you have:

- Python installed at a version compatible with the project configuration.
- Git installed.
- `uv` installed for dependency management.
- A Groq API key.

## 💻 Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/Parasmate18/TalentLens.git
cd TalentLens
```

### 2. Install dependencies

Install `uv` if it is not already available:

```bash
pip install uv
```

Sync the project dependencies:

```bash
uv sync
```

### 3. Configure your Groq API key

Create or configure the environment variable expected by the application for your Groq API key.

For example, on Windows PowerShell:

```powershell
$env:GROQ_API_KEY="your_groq_api_key"
```

Replace `your_groq_api_key` with your actual API key. Never commit API keys or other secrets to GitHub.

> Check the application's configuration in `main.py` and `miniproject.py` to confirm the exact environment variable name and configuration method.

### 4. Run the application

```bash
uv run python miniproject.py
```

If you prefer to activate the project's virtual environment and run Python directly, use the appropriate activation command for your operating system.

## 📂 Project Structure

```text
TalentLens/
├── main.py          # Main application module
├── miniproject.py   # Application entry point
├── pyproject.toml   # Project metadata and dependencies
├── uv.lock          # Locked dependency versions
├── .python-version  # Python version configuration
├── .gitignore       # Git ignore rules
├── .devcontainer/   # Development container configuration
└── README.md        # Project documentation
```

## 🎯 Use Cases

- Resume screening for job openings.
- Comparing candidate qualifications with job descriptions.
- Identifying relevant skills and potential skill gaps.
- Prioritizing candidates for further review.
- Supporting recruitment and shortlisting workflows.

## 🔮 Future Enhancements

Potential improvements for future versions include:

- A web-based recruiter dashboard.
- Bulk resume upload and batch processing.
- Candidate comparison reports and visual analytics.
- Exportable screening results in CSV or PDF format.
- Resume parsing with additional structured fields.
- Improved explainability for match scores.
- Integration with applicant tracking systems.

## ⚠️ Important Note

TalentLens is designed to assist recruiters, not replace human judgment. AI-generated match scores and recommendations may contain errors and should be reviewed alongside the candidate's actual qualifications. The system should not be used as the sole basis for hiring decisions.

## 👨‍💻 Author

**Paras Mate**

GitHub: [@Parasmate18](https://github.com/Parasmate18)

## 📄 License

A license has not been specified here. Add an appropriate `LICENSE` file before distributing the project under an open-source license.
