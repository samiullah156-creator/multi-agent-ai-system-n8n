<!-- styled:v2 -->
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1d1726,50:167dfe,100:9533fa&height=180&section=header&text=Multi-Agent%20AI%20System%20in%20n8n&fontSize=38&fontColor=ffffff&fontAlignY=36&desc=Case%20study%20%E2%80%A2%20AI%20Agents%20%E2%80%A2%20Multi-agent%20orchestration&descAlignY=58&descSize=16&animation=fadeIn" width="100%" alt="Multi-Agent AI System in n8n" />

**A central AI agent in n8n that routes every request to specialist agents for email, Drive, content, social media, contacts, calendar and the web.**

<p>
  <img src="https://img.shields.io/badge/AI%20Agents-167dfe?style=flat-square" alt="AI Agents" />
  <img src="https://img.shields.io/badge/Multi--agent%20orchestration-9533fa?style=flat-square" alt="Multi-agent orchestration" />
  <img src="https://img.shields.io/badge/n8n-231f20?style=flat-square" alt="n8n" />
  <img src="https://img.shields.io/badge/OpenAI-231f20?style=flat-square" alt="OpenAI" />
  <img src="https://img.shields.io/badge/AI%20Agents-231f20?style=flat-square" alt="AI Agents" />
  <img src="https://img.shields.io/badge/Google%20Workspace-231f20?style=flat-square" alt="Google Workspace" />
  <img src="https://img.shields.io/badge/Telegram-231f20?style=flat-square" alt="Telegram" />
  <img src="https://img.shields.io/badge/REST%20APIs-231f20?style=flat-square" alt="REST APIs" />
</p>

<p>
  <a href="#overview">Overview</a> ·
  <a href="#how-it-works">How it works</a> ·
  <a href="#key-features">Key features</a> ·
  <a href="#results">Results</a> ·
  <a href="#screens">Screens</a> ·
  <a href="#tech-stack">Tech stack</a>
</p>

</div>

---

![n8n multi-agent AI system with a main agent and specialist agents](assets/cover.webp)

## Overview

Many AI agents and integrations had to work together in one workflow without becoming unmanageable. We built a multi-agent system in n8n where a main agent receives each request, decides what it needs and hands the work to specialist agents, each with its own tools and memory. New agents and tools can be added without rebuilding the workflow.

## The challenge

Email, file storage, content, social posting, contacts and calendar tasks each needed their own automation. Built as separate flows they were hard to maintain, and one combined flow quickly became unmanageable.

## The solution

A hub-and-spoke design: a main AI agent receives requests from Telegram and routes each task to specialist agents (email, Google Drive, creative, posting, contacts, calendar, web and social media) with conditional routing, logging and error handling.

## How it works

```mermaid
flowchart LR
    A(["A request comes<br/>in on Telegram"]) --> B
    B["The main<br/>agent decides"] --> C
    C["Specialist agents do<br/>the work"] --> D
    D["Contacts, calendar, web<br/>and social"] --> E
    E(["Results logged<br/>and confirmed"])

    classDef box fill:#1d1726,stroke:#167dfe,color:#e5e7eb
    classDef ends fill:#2e1065,stroke:#9533fa,color:#ffffff
    class B,C,D box
    class A,E ends
```

1. **A request comes in on Telegram.** Messages, files and voice notes from Telegram are received and sorted by type before anything else happens.
2. **The main agent decides.** The main AI agent understands the request and chooses which specialist agent, or agents, should handle it.
3. **Specialist agents do the work.** Email, Google Drive, creative and posting agents each use their own tools and memory to complete their part.
4. **Contacts, calendar, web and social.** More agents manage contacts, calendar events, web research and social media search on the same pattern.
5. **Results logged and confirmed.** Every run is logged to a sheet and the user gets a confirmation, or a clear error message if something fails.

## Key features

- Main agent that routes each task to the right specialist
- Email, Google Drive and content agents
- Social media, contacts and calendar agents
- Web research and conditional routing
- Logging and error messages for every run

## Results

- One central system instead of many separate automations
- New agents and tools added without rebuilding the workflow
- Every action logged with clear error messages

## Tech stack

![n8n](https://img.shields.io/badge/n8n-1d1726?style=for-the-badge) ![OpenAI](https://img.shields.io/badge/OpenAI-1d1726?style=for-the-badge) ![AI Agents](https://img.shields.io/badge/AI%20Agents-1d1726?style=for-the-badge) ![Google Workspace](https://img.shields.io/badge/Google%20Workspace-1d1726?style=for-the-badge) ![Telegram](https://img.shields.io/badge/Telegram-1d1726?style=for-the-badge) ![REST APIs](https://img.shields.io/badge/REST%20APIs-1d1726?style=for-the-badge)

## Screens

![How Multi-Agent AI System in n8n works: Telegram request, Main AI agent, Specialist agents, Google Workspace and APIs, Logged and confirmed](assets/screen-1.webp)

![Multi-Agent AI System in n8n: before and after](assets/screen-2.webp)

## Privacy

Client names and records are confidential. Every screen in this repository uses sample data, and source code that belongs to the client is not published.

## Links

- Case study on Lexvaxa: https://lexvaxa.com/work/multi-agent-ai-system-n8n

---

<div align="center">

**Built by [Ch Muhammad Samiullah](https://github.com/samiullah156-creator)** · AI Automation Engineer and Full-Stack Developer at [Lexvaxa](https://lexvaxa.com)

<a href="https://github.com/samiullah156-creator"><img src="https://img.shields.io/badge/More%20projects-181717?style=for-the-badge&logo=github&logoColor=white" alt="More projects" /></a>
<a href="https://lexvaxa.com/contact"><img src="https://img.shields.io/badge/Work%20with%20me-167dfe?style=for-the-badge&logo=googlecalendar&logoColor=white" alt="Work with me" /></a>
<a href="https://www.linkedin.com/in/sami-lexvaxa/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>

<sub>⭐ Star this repo if you found it useful</sub>

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:9533fa,50:167dfe,100:1d1726&height=110&section=footer" width="100%" alt="" />
