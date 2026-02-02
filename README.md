# TRP 1 – MCP Setup Challenge Documentation

## Overview

This repository documents my work for the **TRP 1 – MCP Setup Challenge**, a 1-hour assessment designed to evaluate my ability to configure a modern AI-assisted development environment using MCP tools, rules, and agent guidance.

The primary goal of this challenge was to demonstrate:
- Technical comprehension of MCP setup
- Openness and curiosity toward AI-powered developer tooling
- Motivation, effort, and structured problem-solving under time constraints

---

## Task 1: MCP Setup

### What I Did

- Selected **Cursor** as my primary IDE.
- Followed the **Tenx MCP Analysis Documentation** to configure and connect to the Tenx MCP server.
- Verified that the MCP connection was active and running during the assessment period.
- Ensured that my IDE was properly configured so that interactions with the coding agent could be logged automatically by the MCP server.

### Outcome

- MCP server connection was successfully established.
- The coding agent was able to respond within the Cursor environment while MCP logging remained active.

---

## Task 2: Research & Rules Configuration

### Rules File Location

- **IDE:** Cursor  
- **Rules File:** `.cursor/rules/agent.mdc`

### Research Conducted

To improve my rules file, I researched:
- Boris Cherny’s workflow and guidance on controlling AI coding agents
- Community best practices for:
  - Prompt discipline
  - Agent behavior constraints
  - Reducing hallucinations
  - Improving reasoning transparency
  - Aligning AI output with developer intent

The goal was not only to write rules, but to **understand how rules influence agent behavior** across different LLM-backed coding assistants.

### Changes Made to the Rules File

Key improvements included:
- Explicit instructions on how the agent should reason before responding
- Clear constraints on assumptions, uncertainty handling, and verbosity
- Guidance on preferred coding style, structure, and explanations
- Emphasis on step-by-step thinking for complex tasks
- Instructions for asking clarifying questions when requirements are ambiguous

Each update was tested by modifying the rules incrementally and observing how the agent’s behavior changed in response.

---

## Task 3: Documentation & Reflection

### What Worked

- Adding explicit reasoning and behavior constraints significantly improved response quality.
- The agent became more aligned with my thought process when rules were concrete and specific.
- Incremental testing of rules helped identify which instructions had meaningful impact versus those that were ignored.

### What Didn’t Work / Challenges Faced

- Overly generic rules had little to no effect on agent behavior.
- Some constraints conflicted depending on the underlying model, requiring refinement.
- Initial MCP setup required careful attention to environment configuration and verification.
- **Network Issue:** Initially, the MCP server would not connect over my primary Wi-Fi network. I identified this issue during testing and resolved it by switching to a different network, which allowed the MCP connection to work successfully.

### Troubleshooting Approach

- Broke problems into smaller steps instead of changing multiple variables at once
- Used test prompts to validate rule effectiveness after each modification
- Reviewed documentation and community references when expected behavior did not occur
- Switched networks to resolve connectivity issues with the MCP server

---

## Insights Gained

- AI agent rules act as a **behavioral contract**, not just preferences.
- Well-written rules dramatically reduce hallucination, improve reasoning clarity, and align output with developer expectations.
- The effectiveness of rules depends on:
  - Clarity
  - Specificity
  - Compatibility with the selected IDE and LLM
- Treating AI agents as configurable collaborators—not black boxes—leads to better outcomes.

---

## Artifacts in This Repository

- MCP setup and configuration files
- Final AI agent rules file (`.cursor/rules/agent.mdc`)
- This documentation report
- Additional notes and artifacts generated during experimentation

---

## Final Notes

This challenge reinforced the importance of:
- Structured experimentation
- Curiosity-driven learning
- Clear communication with AI systems

I approached the task with the mindset of building a **repeatable, professional AI-assisted development environment**, rather than simply completing a checklist.
