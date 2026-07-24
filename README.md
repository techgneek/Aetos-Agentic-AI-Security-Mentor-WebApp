<h1 align="center">AetosAI Security Mentor</h1>
<p align="center">
   Voice-enabled Agentic AI Security Mentor for secure AI behavior, red-team practice, and compliance evidence
</p>

<p align="center">
   <img src="https://img.shields.io/badge/Status-Portfolio%20Ready-0B5FFF?style=for-the-badge" alt="Status Portfolio Ready" />
   <img src="https://img.shields.io/badge/Focus-Agentic%20AI%20Security-0A7D5A?style=for-the-badge" alt="Focus Agentic AI Security" />
   <img src="https://img.shields.io/badge/Stack-React%20%2F%20Vite%20%2F%20TypeScript-1F2937?style=for-the-badge" alt="Stack React Vite TypeScript" />
   <img src="https://img.shields.io/badge/Security-CI%20%2B%20Gitleaks%20%2B%20CodeQL-9A3412?style=for-the-badge" alt="Security CI Gitleaks CodeQL" />
   <img src="https://img.shields.io/badge/Deployment-Production%20Hosted-4C1D95?style=for-the-badge" alt="Deployment Production Hosted" />
</p>

<p align="center">
   <img width="1774" height="887" alt="aetos-ai-security-mentor-hero-banner" src="https://github.com/user-attachments/assets/d1b99112-f04f-421f-81ab-998e57714c8c" />
</p>
<p align="center">
   <a href="https://aetosai.io"><strong>Visit Us At AetosAI.io</strong></a>
</p>

## Product Overview

AetosAI Security Mentor is an Agentic AI Security Mentor built to teach, test, and operationalize secure AI behavior in one workflow.

It supports natural mentoring conversations through chat and voice, pairs scenario-driven learning with reference-grounded security guidance, and captures compliance-oriented evidence and security outcomes for review.

The platform is designed as a security-first AI application, not just a generic chatbot. It combines mentoring, incident-style thinking, red-team-oriented workflows, and operational visibility to help teams secure LLM-enabled and agentic systems.

## 🎥 Walkthroughs

### 🎙️ Voice Mentor Demo

https://github.com/user-attachments/assets/abaa73ec-a809-4d4c-8f3f-8b1edf272c39

Hands-free voice mentoring with live audio, talk-to-text, and transcript capture. This walkthrough shows how the voice path works alongside standard chat so users can move between spoken and typed guidance without losing session context.

### Chat Prompt Demo

https://github.com/user-attachments/assets/944ef81e-89c7-46c0-8c64-17a31ba2235b

Guided prompt coaching for agentic AI security. This walkthrough shows how users can ask follow-up questions, stay anchored to a selected scenario, and use the mentor to think through secure decisions in chat.

### Common AI Security Questions

https://github.com/user-attachments/assets/cfc2663c-709b-432a-b9a0-be12e4762507

A practical question library for common AI security scenarios. This walkthrough shows the scenario engine, prompt selection flow, and the kinds of security questions users can practice against, including prompt injection, tool boundaries, incident response, and validation.

### AI Security Reference Library

https://github.com/user-attachments/assets/a875f54e-6854-4fe8-8feb-de19fde026b7

A searchable reference library for OWASP LLM, OWASP Agentic AI, MITRE ATLAS, and related guidance. This walkthrough shows how users map questions back to controls, mitigations, and framework language during mentoring and review.

### Compliance Evidence & Red-Team Audit Flow

https://github.com/user-attachments/assets/1f47d79a-28a2-494a-89ed-28b2e0bcbc60

A combined compliance and red-team evidence view. This walkthrough shows how the app captures audit records, preserves evidence, and summarizes validation outcomes for review and follow-up.

## 🧭 How the Application Works

1. User opens AetosAI Security Mentor.
2. User asks a security question or launches a guided scenario.
3. Mentor responds using security-first rules and guardrails.
4. User interacts through chat or voice.
5. Session and transcript activity is captured for review.
6. Security misses or risky patterns can be logged.
7. Compliance and red-team evidence can be reviewed.
8. Health and deployment checks confirm operational status.

## 🏗️ Architecture

<img width="1774" height="887" alt="aetos-ai-security-architecture" src="https://github.com/user-attachments/assets/a90bde85-6278-4b58-97cf-23ae0d5c1bb4" />

## 🔌 API-Backed Security Architecture

The platform uses API-backed workflows to connect mentoring, scenario execution, evidence visibility, and operational security checks.

| Capability | Purpose | Implementation |
| --- | --- | --- |
| Chat | Mentor Q&A and security guidance | `/api/chat` |
| Scenarios | Guided security learning workflows | `/api/scenarios` |
| Health | Availability and deployment validation | `/api/health` |
| Compliance Evidence | Audit-ready evidence retrieval | `/api/compliance/evidence` |
| Red-Team Audit | Offensive-security exercise tracking | `/api/redteam/audit`, `/api/redteam/history` |
| Voice / WebSocket | Real-time or hands-free mentor interaction | `/api/live` (WebSocket bridge in backend runtime) |

Additional API-backed security capabilities include:

- Runtime checks through health and service telemetry endpoints.
- Deployment and availability checks using health status and operational diagnostics.
- Evidence retrieval and control visibility through compliance endpoints.
- Red-team audit and history support for repeatable adversarial exercise review.
- Voice backend and WebSocket support for live interaction where deployment topology supports WebSocket upgrades.

## 🛡️ Security-by-Design Approach

Security controls are embedded directly into product behavior across mentoring, scenario workflows, API boundaries, and operational evidence collection.

Mentor responses are constrained by security-first rules and guardrails to reinforce practical defensive reasoning, not just generic answer generation.

The application emphasizes trust boundaries between user input, model behavior, tool invocation, and backend control paths.

Its architecture is built to support operational evidence and traceability, not just policy statements.

Security misses and risky patterns are treated as learning and audit opportunities, helping teams improve defensive posture over time.

The system encourages reasoning before tool usage, with guardrails that prioritize containment, validation, and evidence.

Core security principles include:

- Least privilege
- Human-in-the-loop review
- Prompt injection awareness
- Agent tool boundary awareness
- Secure API behavior
- Auditability
- Evidence capture
- Operational monitoring

## 📚 Framework Alignment

| Project Area | Security / Compliance Alignment |
| --- | --- |
| Prompt injection and mentor guardrails | OWASP LLM Top 10 |
| Agent behavior and tool boundaries | OWASP Agentic AI guidance |
| Adversarial AI testing | MITRE ATLAS |
| Evidence and control operation | SOC 2-style audit readiness |
| Security monitoring and incident review | Detection and response maturity |
| Secure delivery pipeline | DevSecOps and software supply chain security |

This project is designed to support audit narratives and control evidence patterns. It is not a formal compliance certification.

## 🔐 CI/CD Security Pipeline

The repository uses a security-first CI/CD pipeline to validate build integrity, reduce software supply chain risk, and enforce phased control maturity.

Pipeline controls include:

- Type checks and static build validation in CI.
- Production build verification before merge and deploy pathways.
- Software composition and dependency checks via npm audit artifacts and summaries.
- Gitleaks secret scanning in CI with soft-gate enforcement.
- Local pre-commit and pre-push secret guardrails to shift detection left.
- CodeQL analysis with enforcement toggle for phased rollout.
- Security artifacts and evidence outputs for findings triage.
- Branch governance and production-protection runbooks.
- Phase-based vulnerability gate evolution from observation to enforcement.

Security maturity is managed through a phased enforcement model:

1. Observe
2. Warn
3. Enforce
4. Mature and operationalize

This model supports practical DevSecOps adoption by incrementally tightening controls while preserving delivery reliability and evidence quality.

Related security governance and implementation references:

- `docs/security/governance/SECURITY_PHASES.md`
- `docs/security/governance/SECURITY_FINDINGS.md`
- `.github/workflows/security-ci.yml`
- `docs/security/runbooks/PHASE3_BRANCH_PROTECTION.md`
- `docs/security/runbooks/PHASE3_ENVIRONMENT_PROTECTION.md`
- `docs/security/runbooks/PHASE4_OPERATIONAL_MATURITY.md`

## Run Locally

**Prerequisites:**  Node.js


1. Install dependencies:
   `npm install`
2. Set the `GEMINI_API_KEY` in **.env.local** to your Gemini API key
3. Run the app:
   `npm run dev`

## Security Automation

Security controls are enforced through the repository pipeline so the app stays protected without exposing rollout internals on the front page.

- CI workflow: `.github/workflows/security-ci.yml`
- Secret scanning and local pre-push hooks are enabled for hardcoded secret prevention.
- Dependency and build checks gate merges when critical issues are detected.
- Compliance records capture the evidence trail for key actions and audit events.

## Shadow Containment / Honeypot Protection

The app includes a defensive-deception layer that steers suspicious prompts and tool probes into shadow paths instead of real systems. It uses decoy routes, memory anchors, and reverse honeyprompt markers to record hostile behavior, preserve evidence, and keep legitimate mentoring traffic on the normal path.

## Future Enhancements

- Expand the architecture overview into a separate visual map.
- Add more linked examples between walkthroughs and controls.
- Provide downloadable summaries for the main mentoring paths.
- Add more guided comparisons between safe and unsafe agent behaviors.

## Wave 2.5 Local Secret Guardrails

Local guardrails block hardcoded secrets before CI and before push.

What was done:

- Added local git hooks for pre-commit and pre-push secret scanning.
- Wired the hook installer to use `gitleaks` locally or fetch a pinned binary when needed.
- Kept the emergency bypass path documented for incident recovery only.

For the exact commands and install flow, see [docs/security/guides/local-secret-guardrails/README.md](docs/security/guides/local-secret-guardrails/README.md).

## Phase 4 Operations

Phase 4 focuses on recurring drills, dependency review, and tabletop readiness.

What was done:

- Added scaffolds for monthly drill records and monthly dependency/CI reviews.
- Added a quarterly tabletop drill scaffold.
- Kept the evidence location and generated artifacts under a dedicated operations folder.

For the exact commands and usage notes, see [docs/security/runbooks/phase-4-operations/README.md](docs/security/runbooks/phase-4-operations/README.md).
