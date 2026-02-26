# AI Brain Template Lite (v0.1.1)

> **Minimalist AI Agent workflow template, optimized for Google Antigravity and Codex Web.**

[中文版本 (Chinese Version)](./README.md)

## 🎯 Project Philosophy

This template standardizes the AI Agent development process through a "Command-first" and "Specification-first" mindset, making the development process more controllable and traceable.

- **Correctness First**: Correctness overrides performance or complexity. Unverifiable behavior is considered unsafe.
- **Think Before Code**: Plan first, implement later. Avoid blind coding.
- **Context Hygiene**: Maintain minimal context to reduce noise and costs.

> **References**
> The philosophy of this template is inspired by the [Superpowers project](https://github.com/obra/superpowers).

## 🚀 Quick Start

1. **Deploy to Project**: Copy the `.agent`, `.agents`, `.antigravity`, and `AGENTS.md` folders/files to your project root.
2. **Initial Command**: At the start of a new conversation, enter:

   ```text
   Please follow the specifications in AGENTS.md and .agent/CONSTITUTION_EN.md.
   Start with /bootstrap.
   ```

## 🛠️ Core Commands (Slash Commands)

| Command | Description |
| :--- | :--- |
| `/bootstrap` | Set task goals, constraints, and acceptance criteria. |
| `/plan` | List file changes, implementation steps, and risks. |
| `/implement` | Implement based on the confirmed plan. |
| `/test` | Execute verification commands and record results. |
| `/handoff` | Generate a handoff summary (progress, risks, next steps). |

## 🧩 File Structure

- `.agent/CONSTITUTION_EN.md`: Core engineering specifications (English).
- `.agent/workflows/`: Antigravity workflow definitions (Slash Commands).
- `.agents/skills/`: Codex Web command entry points (Pointer files).
- `AGENTS.md`: Cross-platform general command definitions.

## 🌐 Language Settings

By default, this template is set up for Traditional Chinese. To use it in **English**:

1. Use `/bootstrap` and add "Please respond in English" to your prompt.
2. Update `.agent/AGENT.md` and change the language setting to English.
