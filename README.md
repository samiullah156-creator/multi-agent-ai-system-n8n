# Multi-Agent AI System in n8n

**A central AI agent in n8n that routes every request to specialist agents for email, Drive, content, social media, contacts, calendar and the web.**

![AI Agents](https://img.shields.io/badge/AI%20Agents-167dfe?style=flat-square) ![Multi-agent orchestration](https://img.shields.io/badge/Multi--agent%20orchestration-9533fa?style=flat-square) ![n8n](https://img.shields.io/badge/n8n-231f20?style=flat-square) ![OpenAI](https://img.shields.io/badge/OpenAI-231f20?style=flat-square) ![AI Agents](https://img.shields.io/badge/AI%20Agents-231f20?style=flat-square) ![Google Workspace](https://img.shields.io/badge/Google%20Workspace-231f20?style=flat-square) ![Telegram](https://img.shields.io/badge/Telegram-231f20?style=flat-square) ![REST APIs](https://img.shields.io/badge/REST%20APIs-231f20?style=flat-square)

![n8n multi-agent AI system with a main agent and specialist agents](assets/cover.webp)

## Overview

Many AI agents and integrations had to work together in one workflow without becoming unmanageable. We built a multi-agent system in n8n where a main agent receives each request, decides what it needs and hands the work to specialist agents, each with its own tools and memory. New agents and tools can be added without rebuilding the workflow.

## The challenge

Email, file storage, content, social posting, contacts and calendar tasks each needed their own automation. Built as separate flows they were hard to maintain, and one combined flow quickly became unmanageable.

## The solution

A hub-and-spoke design: a main AI agent receives requests from Telegram and routes each task to specialist agents (email, Google Drive, creative, posting, contacts, calendar, web and social media) with conditional routing, logging and error handling.

## How it works

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

n8n · OpenAI · AI Agents · Google Workspace · Telegram · REST APIs

## Screens

![How Multi-Agent AI System in n8n works: Telegram request, Main AI agent, Specialist agents, Google Workspace and APIs, Logged and confirmed](assets/screen-1.webp)

![Multi-Agent AI System in n8n: before and after](assets/screen-2.webp)

## Privacy

Client names and records are confidential. Every screen in this repository uses sample data, and source code that belongs to the client is not published.

## Links

- Case study on Lexvaxa: https://lexvaxa.com/work/multi-agent-ai-system-n8n
- Built by **Ch Muhammad Samiullah** ([GitHub](https://github.com/samiullah156-creator)) at [Lexvaxa](https://lexvaxa.com)
