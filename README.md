# AetosAI Security Mentor

<p align="center">
  Voice-enabled Agentic AI Security Mentor for secure AI behavior, red-team practice, and public documentation
</p>

<p align="center">
  <a href="https://aetosai.io"><strong>Visit Us At AetosAI.io</strong></a>
</p>

## Product Overview

AetosAI Security Mentor is an Agentic AI Security Mentor built to teach, test, and operationalize secure AI behavior in one workflow.

It supports natural mentoring conversations through chat and voice, pairs scenario-driven learning with reference-grounded security guidance, and captures public-facing product information for review.

The platform is designed as a security-first AI application, not just a generic chatbot. It combines mentoring, incident-style thinking, red-team-oriented workflows, and operational visibility to help teams secure LLM-enabled and agentic systems.

## 🎥 Walkthroughs

### 🎙️ Voice Mentor Demo

Hands-free voice mentoring with live audio, talk-to-text, and transcript capture. This walkthrough shows how the voice path works alongside standard chat so users can move between spoken and typed guidance without losing session context.

See: [Voice Mentor Demo](docs/walkthroughs.md#voice-mentor-demo)

### Chat Prompt Demo

Guided prompt coaching for agentic AI security. This walkthrough shows how users can ask follow-up questions, stay anchored to a selected scenario, and use the mentor to think through secure decisions in chat.

See: [Chat Prompt Demo](docs/walkthroughs.md#chat-prompt-demo)

### Common AI Security Questions

A practical question library for common AI security scenarios. This walkthrough shows the scenario engine, prompt selection flow, and the kinds of security questions users can practice against, including prompt injection, tool boundaries, incident response, and validation.

See: [Common AI Security Questions](docs/walkthroughs.md#common-ai-security-questions)

### AI Security Reference Library

A searchable reference library for common AI security guidance and framework language during mentoring and review.

See: [AI Security Reference Library](docs/walkthroughs.md#ai-security-reference-library)

### Compliance Evidence & Red-Team Audit Flow

A combined compliance and red-team evidence view. This walkthrough shows how the app captures review records, preserves evidence, and summarizes validation outcomes for follow-up.

See: [Compliance Evidence And Review](docs/walkthroughs.md#compliance-evidence-and-review)

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

The public documentation keeps the architecture explanation at a high level and points readers to supporting markdown pages for the product story and security posture.

See: [Overview](docs/overview.md) and [Security Posture](docs/security-posture.md)

## 🛡️ Security-by-Design Approach

Security controls are embedded directly into product behavior across mentoring, scenario workflows, and evidence collection.

Mentor responses are constrained by security-first rules and guardrails to reinforce practical defensive reasoning, not just generic answer generation.

The application emphasizes trust boundaries between user input, model behavior, tool invocation, and backend control paths.

Its architecture is built to support operational evidence and traceability, not just policy statements.

Security misses and risky patterns are treated as learning and review opportunities, helping teams improve defensive posture over time.

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

This project is designed to support public product documentation and review narratives. It is not a formal compliance certification.

## Public Documentation

The supporting markdown pages live under [docs/](docs/index.md).

- [Overview](docs/overview.md)
- [Getting Started](docs/getting-started.md)
- [Walkthroughs](docs/walkthroughs.md)
- [Security Posture](docs/security-posture.md)
- [Publishing Process](docs/process.md)

These pages are written for public viewing and do not include source code, private repository links, or internal automation details.