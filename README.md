# Resume Builder: Streamlining Success in Career Crafting

A full-stack web application that helps job seekers create professional, polished resumes with **real-time preview**, **PDF download**, and an intelligent **Skill Gap Analysis tool** — all in one place.

> Real-Time Research Project | Department of CSE, GRIET, Hyderabad | 2023–2024


##  Problem Statement

Creating a standout resume is one of the biggest challenges for job seekers today. Most existing resume builders focus only on formatting, leaving users without guidance on content quality, skill relevance, or how to tailor their resume to specific job roles. This project solves that by combining a professional resume builder with an NLP-powered skill analysis tool.

##  Key Features

-  **Step-by-step resume creation** — personal details, education, work experience, projects, skills, and summary
-  **Real-time preview** — see your resume update live as you type
-  **PDF download** — export a professionally formatted resume instantly using `jsPDF`, `html2canvas`, and `html2pdf`
-  **Skill Gap Analysis** — input your desired job role and get personalized recommendations on skills you're missing
-  **Cross-device compatible** — accessible from any browser or device


##  How the Skill Gap Analysis Works

1. **User inputs their skills** — the tool normalizes inputs (trims whitespace, converts to lowercase) for consistency
2. **User selects a desired job role** from a predefined list based on industry standards
3. **Skill comparison** — user skills are matched against the required skills for that role using a CSV job-skills dataset
4. **Gap identification** — missing skills are highlighted
5. **Personalized recommendations** — the tool suggests specific skills, certifications, or experiences to improve employability


## System Architecture

User Input (React Frontend)
        ↓
Personal Info → Education → Work Experience → Projects → Skills → Summary
        ↓
Skill Gap Analysis (NLP-based comparison with jobs dataset)
        ↓
Real-Time Resume Preview (HTML rendered)
        ↓
PDF Export (jsPDF + html2canvas + html2pdf)


##  Modules

| Module | Description |
|--------|-------------|
| **Personal Information** | Full name, contact details, LinkedIn profile |
| **Education** | Multiple degrees, institutions, graduation years |
| **Work Experience** | Job titles, companies, descriptions, employment dates |
| **Projects** | Project name, role, description, timeline, and links |
| **Skills + Skill Gap Analysis** | Skill input + comparison against job role requirements |
| **Resume Preview** | Live formatted preview that mirrors the final output |
| **PDF Generator** | One-click export using html2pdf / jsPDF |


##  Tech Stack

| Category | Tools |
|----------|-------|
| Frontend | React.js, HTML, CSS, JavaScript |
| Backend | Node.js |
| PDF Generation | jsPDF, html2canvas, html2pdf |
| Data | CSV job-skills dataset for skill gap analysis |
| Version Control | Git |
| IDE | Visual Studio Code |


## Results

- Users could create a complete, professionally formatted resume in minutes
- Skill Gap Analysis successfully identified missing skills and provided targeted recommendations based on the selected job role
- PDF export produced clean, ready-to-submit resumes directly from the browser
- Real-time preview eliminated the need for repeated submissions to check formatting


##  Dataset

A **jobs-skillset CSV dataset** is used for the Skill Gap Analysis. It maps job roles (e.g., Software Engineer, Data Analyst, Web Developer) to their required skill sets based on industry standards and job market research. User-entered skills are compared against this dataset to identify gaps.


## Future Scope

- AI-powered resume content suggestions based on job descriptions
- Multiple resume templates and custom styling options
- Integration with LinkedIn for auto-importing profile data
- ATS (Applicant Tracking System) score checker
- Expanded job-skills dataset with continuous updates from live job postings
- User accounts for saving and managing multiple resume versions


##  References

Key references include Jadhav et al. (2023) on full-stack resume builder systems, Mulla (2023) on resume builders with job prediction, and Kulkarni et al. (2023) on resume parsing using ML and NLP. Full reference list available in the project report.
