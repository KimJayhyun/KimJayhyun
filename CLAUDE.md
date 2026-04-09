# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a GitHub profile repository (`KimJayhyun/KimJayhyun`). The primary file is `README.md`, which GitHub renders as the public profile page for the user `KimJayhyun`.

There is no build system, test suite, or application code.

## README Structure

The README is organized into the following sections (top to bottom):

1. **Header** — Animated waving banner via `capsule-render.vercel.app` + typing SVG animation
2. **👋 About Me** — 5 years of experience, AI Engineer identity, SI + in-house background, contact info (Blog, Email)
3. **🛠 Tech Stack** — Divided into subsections:
   - 🤖 AI: LangChain, Google ADK, MCP, A2A
   - ⚙️ Backend: Python, FastAPI
   - 🐳 Infra: Kubernetes, Helm, Docker, Podman
   - 🚀 DevOps: Jenkins
4. **📡 On My Radar** — Divided into:
   - 🌱 Learning: React, Electron, Spring
   - 📚 Studied: GitHub Actions, Ansible
5. **💼 Projects** — Table with Period / Project / Description / Role / Stack (5 SI projects, latest first, company names anonymized)
6. **🏅 Certifications** — Badge-style: CKA, 정보처리기사, SQLD, 네트워크관리사 2급, +more
7. **📊 GitHub Stats** — Streak Stats + Top Languages (side by side) + Activity Graph (full width below)
8. **Footer** — Waving banner

## Key Design Decisions

- **Company names anonymized** — SI projects use domain labels (공공기관, 금융권, 은행권) instead of actual client names due to NDA concerns
- **A2A badge** — Uses official a2aproject/A2A SVG logo (white version, base64 encoded inline)
- **MCP badge** — Uses Anthropic logo from Simple Icons
- **Top Languages** — Uses `github-profile-summary-cards.vercel.app` (NOT `github-readme-stats.vercel.app` which is unreliable). Jupyter Notebook excluded via `exclude=jupyter%20Notebook` parameter
- **Activity Graph** — Uses `github-readme-activity-graph.vercel.app` with `tokyo-night` theme
- **On My Radar** — Separate section from Tech Stack to distinguish "currently learning/studied" from "hands-on experience"
- **Learning vs Studied** — Learning = currently studying, Studied = completed courses but not applied in production

## Assets

- `images/adk-logo.png` — Official Google ADK logo downloaded from google/adk-python repo
- `images/adk-logo.svg` — SVG wrapper around the PNG (not currently used in README, Google logo badge used instead due to size constraints)

## Pending / Future Work

- **Velog** — Blog linked but not actively updated. Needs content refresh around LLM Agent / A2A / MCP topics
- **LinkedIn / 리맴버** — Profiles exist but not filled in. README content can be used as source for populating them
- **Jupyter Notebook → Python** — Can add `.gitattributes` with `*.ipynb linguist-language=Python` to repos that contain notebooks, which will increase Python ratio in Top Languages card
- **CI/CD (GitHub Actions, Ansible)** — Studied but not applied in production. Kept in 📚 Studied section intentionally

## Common Tasks

- **Add/update Tech Stack badge**: Use shields.io `for-the-badge` style. Match existing color conventions per category
- **Update Projects table**: Keep latest-first order, use domain labels instead of company names
- **Change Stats theme**: All cards use `radical` theme except Activity Graph which uses `tokyo-night`
