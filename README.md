<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:00F5FF,100:7B2FF7&height=220&section=header&text=Adwaita%20Narayan%20Behera&fontSize=42&fontColor=ffffff&fontAlignY=36&desc=Backend%20Engineer%20%C2%B7%20Applied%20AI%20%C2%B7%20Automation&descSize=18&descAlignY=58&animation=fadeIn" alt="Banner" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&duration=3000&pause=800&color=00F5FF&center=true&vCenter=true&width=700&lines=Building+FastAPI+backends+that+scale;Shipping+LLM+%2B+RAG+pipelines;Deploying+full-stack+apps+on+AWS+%26+Vercel;Open+to+SDE+%2F+Python+Backend+roles+%F0%9F%9A%80" alt="Typing animation"/>

<br/>

<img src="https://img.shields.io/badge/Python-0d1117?style=for-the-badge&logo=python&logoColor=00F5FF"/>
<img src="https://img.shields.io/badge/FastAPI-0d1117?style=for-the-badge&logo=fastapi&logoColor=00F5FF"/>
<img src="https://img.shields.io/badge/PostgreSQL-0d1117?style=for-the-badge&logo=postgresql&logoColor=00F5FF"/>
<img src="https://img.shields.io/badge/Next.js-0d1117?style=for-the-badge&logo=nextdotjs&logoColor=00F5FF"/>
<img src="https://img.shields.io/badge/AWS-0d1117?style=for-the-badge&logo=amazonaws&logoColor=00F5FF"/>

<br/><br/>

<img src="https://komarev.com/ghpvc/?username=AdwaitaNarayan&label=Profile%20Views&color=00F5FF&style=for-the-badge&labelColor=0d1117" alt="Views"/>
<img src="https://img.shields.io/badge/Status-Open%20to%20Work-00F5FF?style=for-the-badge&labelColor=0d1117"/>

</div>

<br/>

## 🖥️ `whoami`

```bash
$ whoami
adwaita-narayan-behera

$ cat profile.json
{
  "role":      "Software Developer Engineer",
  "location":  "Angul, Odisha, India 🇮🇳",
  "focus":     ["Backend APIs", "LLM & RAG systems", "Automation pipelines"],
  "shipped":   "Pixlume → pixlume.online",
  "education": "B.Tech CSE · CGPA 8.10",
  "seeking":   "Entry-level SDE / Python Backend Developer"
}

$ echo $PHILOSOPHY
Clean architecture. Reliable APIs. Production-ready AI.
```

I build **backend services and applied AI systems**: REST APIs with **FastAPI, SQLAlchemy and PostgreSQL**, taken all the way to production on **AWS EC2 + Nginx** and **Vercel**. Across two internships I've shipped hiring-automation engines and OCR + RAG document pipelines.

<br/>

## 🧬 Pixlume Architecture

```mermaid
flowchart LR
    U(["👤 User Browser"]) --> FE["Next.js Frontend<br/>hosted on Vercel"]
    FE -- "REST / JSON<br/>(CORS enabled)" --> NG["Nginx<br/>reverse proxy"]

    subgraph EC2 ["☁️ AWS EC2"]
        NG --> API["FastAPI app<br/>app/main.py"]
        API --> R["Routers<br/>/photos · /admin"]
        R --> SV["Services<br/>business logic"]
        SV --> ORM["SQLAlchemy Async ORM<br/>+ Pydantic schemas"]
    end

    ORM --> DB[("PostgreSQL<br/>photo metadata")]
    AL["Alembic<br/>migrations"] -.-> DB
    SV --> CL["Cloudinary<br/>high-res image storage"]
```

<br/>

## 🔍 Document Extraction Pipeline

```mermaid
flowchart LR
    A["📄 Input document<br/>PDF / scanned image"] --> B["Text extraction<br/>PyMuPDF · PaddleOCR · PyTesseract"]
    B --> C["Clean + normalise text"]
    C --> D{"Keyword / pattern<br/>classifier"}

    D --> T1["Accounting"]
    D --> T2["Bookkeeping"]
    D --> T3["Payroll"]
    D --> T4["Audit"]
    D --> T5["Tax Planning"]
    D --> T6["Financial Reporting"]

    T1 & T2 & T3 & T4 & T5 & T6 --> E["Field extractor<br/>per document type"]
    E --> F["Validated structured JSON"]
    F --> G[("Database / API response")]
```

<details>
<summary><b>📋 Document types, trigger keywords and extracted fields</b></summary>
<br/>

| Type | Trigger keywords / patterns | Extracted fields |
|---|---|---|
| **Accounting** | Balance Sheet, P&L, Trial Balance, Debit, Credit, Ledger | Date, Assets, Liabilities |
| **Bookkeeping** | Cash Book, Voucher, Day Book, Journal | Date, Narration, Amount |
| **Payroll** | Salary Slip, Net Pay, PF, TDS, Employee | Month, Name, Net Salary |
| **Audit** | Audit Report, Opinion, Findings, CA, Audit Observations | Company Name, Year, Opinion |
| **Tax Planning** | Section 80C, Investment, Tax Saving, Taxable Income | Income, Tax Plan, Deductions |
| **Financial Reporting** | Q1/Q2 Results, EPS, Revenue, Net Profit, Cash Flow | Period, Revenue, Net Profit |

</details>

<br/>

## 🛠️ Arsenal

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,fastapi,django,sqlalchemy,postgres,nextjs,react,js,aws,nginx,vercel,git,github,postman,vscode,tensorflow,pytorch&theme=dark" alt="Tech stack"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/LangChain-0d1117?style=flat-square&logo=langchain&logoColor=00F5FF"/>
  <img src="https://img.shields.io/badge/FAISS-0d1117?style=flat-square&logo=meta&logoColor=00F5FF"/>
  <img src="https://img.shields.io/badge/HuggingFace-0d1117?style=flat-square&logo=huggingface&logoColor=00F5FF"/>
  <img src="https://img.shields.io/badge/Ollama-0d1117?style=flat-square&logo=ollama&logoColor=00F5FF"/>
  <img src="https://img.shields.io/badge/Pydantic-0d1117?style=flat-square&logo=pydantic&logoColor=00F5FF"/>
  <img src="https://img.shields.io/badge/Cloudinary-0d1117?style=flat-square&logo=cloudinary&logoColor=00F5FF"/>
  <img src="https://img.shields.io/badge/Pandas-0d1117?style=flat-square&logo=pandas&logoColor=00F5FF"/>
  <img src="https://img.shields.io/badge/Jupyter-0d1117?style=flat-square&logo=jupyter&logoColor=00F5FF"/>
</p>

<br/>

## 💼 Experience

<details open>
<summary><b>🧠 AI Developer Intern · Hirekarma Pvt. Ltd.</b> &nbsp;<code>Nov 2025 – Feb 2026</code></summary>
<br/>

- Built REST APIs with **FastAPI, SQLAlchemy and PostgreSQL** for candidate assessments, job roles, reporting and playlists
- Developed AI **question generation, evaluation and scoring engines** for hiring workflows
- Implemented **ATS resume scoring, domain classification** and personalised job-recommendation pipelines

</details>

<details open>
<summary><b>🔍 AI/ML Engineer Intern · AAANS Services Pvt. Ltd.</b> &nbsp;<code>Jul 2025 – Oct 2025</code></summary>
<br/>

- Designed **OCR automation pipelines** (PaddleOCR, PyTesseract, PyMuPDF) to extract structured data from PDFs
- Built **RAG-based PDF Q&A** systems with LangChain + FAISS
- Fine-tuned and evaluated LLMs for domain-specific QA and text classification

</details>

<br/>

## 🚀 Featured Projects

<table align="center">
  <tr>
    <td width="50%" valign="top">
      <h3 align="center">📸 Pixlume</h3>
      <p align="center"><sub><b>LIVE · FULL-STACK</b></sub></p>
      <p align="center">Photography platform to browse, search and download high-res images. Next.js + FastAPI + PostgreSQL, Cloudinary storage, deployed on Vercel and AWS EC2 behind Nginx.</p>
      <p align="center"><a href="https://pixlume.online"><img src="https://img.shields.io/badge/Visit%20Live-00F5FF?style=for-the-badge&logo=googlechrome&logoColor=0d1117"/></a></p>
    </td>
    <td width="50%" valign="top">
      <h3 align="center">📄 Document Processing System</h3>
      <p align="center"><sub><b>OCR · LLM · RAG</b></sub></p>
      <p align="center">Intelligent document extraction and PDF question-answering using OCR, LangChain and FAISS.</p>
      <p align="center"><a href="https://github.com/AdwaitaNarayan/Data_Analyst_AI_Agent"><img src="https://img.shields.io/badge/Repository-00F5FF?style=for-the-badge&logo=github&logoColor=0d1117"/></a></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3 align="center">🔤 Odia Character Recognition</h3>
      <p align="center"><sub><b>DEEP LEARNING · CV</b></sub></p>
      <p align="center">End-to-end Odia alpha-numeric classifier. EfficientNet-B0, ResNet-50 and SVM models served via REST APIs.</p>
      <p align="center"><a href="https://github.com/AdwaitaNarayan/Odia-Charecter-Recognition"><img src="https://img.shields.io/badge/Repository-00F5FF?style=for-the-badge&logo=github&logoColor=0d1117"/></a></p>
    </td>
    <td width="50%" valign="top">
      <h3 align="center">🧠 Machine Learning Projects</h3>
      <p align="center"><sub><b>PREDICTION · CLASSIFICATION</b></sub></p>
      <p align="center">Prediction, classification and detection models.</p>
      <p align="center"><a href="https://github.com/AdwaitaNarayan/Machine-Learning-Projects"><img src="https://img.shields.io/badge/Repository-00F5FF?style=for-the-badge&logo=github&logoColor=0d1117"/></a></p>
    </td>
  </tr>
</table>

<p align="center"><sub>Also: <a href="https://github.com/AdwaitaNarayan/Python-DSA">Python DSA</a> · data structures and algorithms in Python</sub></p>

<br/>

## 🐍 Contribution Snake

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/AdwaitaNarayan/AdwaitaNarayan/output/github-contribution-grid-snake-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/AdwaitaNarayan/AdwaitaNarayan/output/github-contribution-grid-snake.svg">
    <img alt="Contribution snake" src="https://raw.githubusercontent.com/AdwaitaNarayan/AdwaitaNarayan/output/github-contribution-grid-snake-dark.svg">
  </picture>
</p>

<br/>

## 🌐 Let's Connect

<p align="center">
  <a href="mailto:adwaitanarayan8@gmail.com"><img src="https://img.shields.io/badge/Email-00F5FF?style=for-the-badge&logo=gmail&logoColor=0D1117"/></a>
  <a href="https://www.linkedin.com/in/adwaita-narayan-behera/"><img src="https://img.shields.io/badge/LinkedIn-00F5FF?style=for-the-badge&logo=linkedin&logoColor=0D1117"/></a>
  <a href="https://pixlume.online"><img src="https://img.shields.io/badge/Pixlume-00F5FF?style=for-the-badge&logo=googlechrome&logoColor=0D1117"/></a>
  <a href="https://github.com/AdwaitaNarayan"><img src="https://img.shields.io/badge/GitHub-00F5FF?style=for-the-badge&logo=github&logoColor=0D1117"/></a>
</p>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:7B2FF7,50:00F5FF,100:0d1117&height=120&section=footer" width="100%" alt="Footer"/>
