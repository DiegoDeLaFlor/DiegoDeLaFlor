<h1 align="center">
  <img src="https://readme-typing-svg.herokuapp.com/?font=Righteous&size=32&center=true&vCenter=true&width=700&height=70&duration=4000&lines=Hey,+I'm+Diego+De+La+Flor+👋;AI+Developer+%C2%B7+LLM+Agents+%C2%B7+RAG;Building+QA+skills+that+run+in+production." />
</h1>

<p align="center">
  <a href="https://www.linkedin.com/in/diego-de-la-flor-02048a237/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  <a href="https://diegodelaflor.netlify.app" target="_blank">
    <img src="https://img.shields.io/badge/Portfolio-0e75b6?style=for-the-badge&logo=astro&logoColor=white"/>
  </a>
  <a href="mailto:diegoalonso139@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
  <a href="https://www.youtube.com/@CronoZ2926" target="_blank">
    <img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white"/>
  </a>
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=DiegoDeLaFlor&style=flat-square&color=0e75b6" alt="Profile views"/>
</p>

---

## 🎯 About Me

> **I build LLM-agent skills and RAG pipelines that run in production and save engineering teams real hours.**

I'm an **AI Developer at Mandü HR** with **3 years** of experience and a **QA → Full Stack → AI** progression inside the same production HR tech.

I'm part of the team that maintains the engineering area's **internal LLM-agent toolkit**, and I **own the QA vertical**: I design, maintain and evolve every QA skill the team consumes. The RAG pipeline I designed cut test-case creation time by **70.9%** (50h → 14.55h per sprint), and I refactored it into the modular skills I maintain today.

My focus is **maintainability**: impact that holds up sprint after sprint, not just in a demo.

### What I work on

- **LLM agents & RAG in production** — Jira/Confluence ingestion, pgvector + ChromaDB, OpenAI & Anthropic APIs, MCP integrations, context engineering
- **QA automation with LLMs** — test-case generation from sprint docs, Jira upload, endpoint → Postman mapping, Playwright E2E generation with automatic evidence
- **Multi-agent orchestration** — LangGraph state machines with review-retry loops (see the public repos below)
- **Full-stack foundation** — NestJS, React, Angular, Laravel, .NET; SQL/NoSQL; Azure, Docker

---

## 🏆 Featured Projects — code available

### 1️⃣ Legacy-to-Modern Architect — AI migration agent

| | |
| --- | --- |
| **Problem** | Migrating a legacy codebase (Java, PHP, TypeScript, Python, COBOL) to a clean modern architecture is months of manual, error-prone rewriting. |
| **Solution** | A **6-stage LangGraph state machine** — Ingest → Parse → Index → Plan → Generate → Review — that reverse-engineers a repo, embeds it into **PostgreSQL + pgvector** for RAG, maps bounded contexts to NestJS modules and Angular features, and generates the project with a **4-pass review loop** that retries on critical findings. |
| **Stack** | `TypeScript` `LangGraph` `RAG` `pgvector` `OpenAI API` `NestJS` `Angular` `Clean Architecture` |
| **Result** | Real migration included in the repo: a ~40-file IoT sensor platform → **37 files across 3 NestJS modules in 4 min 39 s**, with a migration quality report. |
| **Repo** | [DiegoDeLaFlor/Legacy-to-Modern-Architect](https://github.com/DiegoDeLaFlor/Legacy-to-Modern-Architect) |

### 2️⃣ Agent for Bug Fixing — multi-agent orchestration

| | |
| --- | --- |
| **Problem** | Fixing a bug ticket well means three different jobs: find the root cause, propose the minimal fix, and try to break it. One agent doing all three tends to skip the last one. |
| **Solution** | An MVP of **three cooperating agents on LangGraph** — *Investigator* (RCA, locates suspect files), *Programmer* (minimal fix with impact assessment), *Verifier* (runs tests and tries to break the change) — driven from a local CLI with a JSON ticket. |
| **Stack** | `Python` `LangGraph` `CLI` `pytest` |
| **Result** | Console report with RCA, fix proposal, PASS/FAIL evidence and logs for every ticket. |
| **Repo** | [DiegoDeLaFlor/Agent-for-bug-fixing](https://github.com/DiegoDeLaFlor/Agent-for-bug-fixing) |

### 3️⃣ DevInsight — engineering intelligence platform

| | |
| --- | --- |
| **Problem** | Teams have no cheap way to turn a GitHub repo into actionable architecture and quality insights. |
| **Solution** | SaaS MVP: **ASP.NET Core backend (DDD + Clean Architecture)** with GitHub OAuth and repo cloning, a **Roslyn AST analyzer**, a **FastAPI AI engine** that generates insights, and a **React** dashboard. Orchestrated with Docker Compose. |
| **Stack** | `C# / .NET 9` `Roslyn` `DDD` `Clean Architecture` `FastAPI` `Python` `React` `Docker` |
| **Status** | Working MVP (analyze → view issues & insights). Next: EF Core persistence, multi-language AST. |
| **Repo** | [DiegoDeLaFlor/DevInsight-Platform](https://github.com/DiegoDeLaFlor/DevInsight-Platform) |

---

## 🔒 Production & research work — private

### QA Skills with LLM Agents — Mandü HR

| | |
| --- | --- |
| **Problem** | Writing test cases by hand from Jira user stories and Confluence specs took ~50 hours per sprint. |
| **Solution** | RAG pipeline over Jira + Confluence (**pgvector + ChromaDB**, OpenAI/Anthropic API), refactored into **modular skills** inside the internal LLM-agent toolkit: test-case generation, automatic Jira upload, endpoint → Postman mapping (happy & unhappy paths), and **Playwright E2E generation** that runs each case and captures evidence. |
| **Impact** | **70.9% less time** creating test cases (50h → 14.55h per sprint), sustained in production and used daily by QA teams. |

### Agricultural Recommendation System — IoT + Machine Learning

| | |
| --- | --- |
| **Problem** | Coffee farmers lack data-driven guidance based on real field conditions. |
| **Solution** | End-to-end research project: **ESP32 sensors** (humidity, NPK, rain) → **Spring Boot** edge backend → **.NET on Azure** → REST API serving predictions. |
| **Result** | **3 models evaluated (Random Forest, XGBoost, CatBoost) on ~9,983 samples**; Random Forest selected for production. |

### YouTube Shorts Content Automation

| | |
| --- | --- |
| **Solution** | **n8n** flow chaining OpenAI (script) → Stability AI (images) → ElevenLabs (voice) → Google Sheets/Drive (queue & assets). |
| **Result** | **20+ shorts per month** generated with no manual intervention. |

---

## 💻 Tech Stack

### AI & Agents

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![RAG](https://img.shields.io/badge/RAG-FF6B6B?style=flat-square&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?style=flat-square&logoColor=white)
![OpenAI API](https://img.shields.io/badge/OpenAI_API-412991?style=flat-square&logo=openai&logoColor=white)
![Anthropic API](https://img.shields.io/badge/Anthropic_API-191919?style=flat-square&logo=anthropic&logoColor=white)
![pgvector](https://img.shields.io/badge/pgvector-336791?style=flat-square&logo=postgresql&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6F00?style=flat-square&logoColor=white)

### QA & Testing

![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white)
![Cypress](https://img.shields.io/badge/Cypress-17202C?style=flat-square&logo=cypress&logoColor=white)
![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=flat-square&logo=selenium&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white)
![JMeter](https://img.shields.io/badge/JMeter-D3D3D3?style=flat-square&logoColor=black)
![BrowserStack](https://img.shields.io/badge/BrowserStack-F26B21?style=flat-square&logo=browserstack&logoColor=white)

### Backend & Cloud

![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Laravel](https://img.shields.io/badge/Laravel-FF2D20?style=flat-square&logo=laravel&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=flat-square&logo=csharp&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0089D6?style=flat-square&logo=microsoftazure&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2CA5E0?style=flat-square&logo=docker&logoColor=white)

### Frontend & Mobile

![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Angular](https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)

### Data

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=flat-square&logo=mongodb&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)

---

## 📊 GitHub Analytics

<div align="center">
  <table>
    <tr>
      <td width="50%">
        <img src="https://github-readme-stats-salesp07.vercel.app/api?username=DiegoDeLaFlor&count_private=true&show_icons=true&theme=react&rank_icon=github&border_radius=10" alt="GitHub Stats" />
      </td>
      <td width="50%">
        <img src="https://github-readme-stats-salesp07.vercel.app/api/top-langs/?username=DiegoDeLaFlor&hide=HTML&langs_count=8&layout=compact&theme=react&border_radius=10&size_weight=0.5&count_weight=0.5&exclude_repo=github-readme-stats" alt="Top Languages" />
      </td>
    </tr>
  </table>
</div>

> **Note:** Public metrics reflect open-source and personal projects. Most of my production work lives in private organizational repositories under confidentiality agreements.

---

## 🎓 University projects — UPC, Software Engineering

Earlier work from my degree, kept public for reference:
[Four Dreams](https://github.com/fourdreamsupc) (DDD microservices on Azure, .NET) ·
[AdventureHub](https://github.com/AdventureHub-AplicacionesMoviles) (Flutter + NestJS) ·
[Diseño de Experimentos](https://github.com/Diseno-de-Experimentos) (Jenkins CI/CD, Cucumber BDD, JMeter) ·
[Digital UX — DermApp](https://github.com/digital-ux-upc-open-source-2022-2) (React/Angular healthtech)

---

## 🎬 Content

I also run a **YouTube channel** on mystery and narrative-driven discovery. Structuring a story from research to final cut is the same discipline as designing a system: know the audience, cut what doesn't serve the outcome.

[![Watch on YouTube](https://img.shields.io/badge/Watch_the_Channel-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/@CronoZ2926)

---

## 🚀 Let's Build Something

I'm interested in:

- **LLM agents and RAG systems** that ship to production and stay maintainable
- **Developer tooling** that removes real hours from engineering workflows
- **Open-source work** on agent orchestration and QA automation

<div align="center">

  **[📧 Email](mailto:diegoalonso139@gmail.com) • [💼 LinkedIn](https://www.linkedin.com/in/diego-de-la-flor-02048a237/) • [🌐 Portfolio](https://diegodelaflor.netlify.app)**

</div>

<img alt="GitHub contribution snake" src="https://raw.githubusercontent.com/DiegoDeLaFlor/DiegoDeLaFlor/output/github-contribution-grid-snake-dark.svg" />

---

<p align="center">
  <em>Built with passion for engineering excellence. Dark mode optimized. © 2026</em>
</p>
