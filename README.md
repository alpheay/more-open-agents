# OpenCode Agents

This repository contains a collection of specialized agents for the OpenCode environment. These agents are designed to handle specific software engineering tasks with expert-level proficiency.

## Agent Modes

- **Agent**: Primary assistants designed for direct user interaction and high-level reasoning.
- **Subagent**: Specialized tools typically delegated to by other agents for specific tasks.
- **Both**: Flexible agents that can function as primary assistants or specialized subagents.

## Available Agents

### 🏗️ Architecture & Planning

| Agent | Mode | Description |
|-------|------|-------------|
| **[System Architect](agents/architect.md)** | `Agent` | Principal architect for high-level system design, patterns, and technical strategy. |
| **[Planner](agents/planner.md)** | `Agent` | Project lead that breaks down complex goals into actionable, dependency-aware plans. |
| **[API Designer](agents/api-designer.md)** | `Agent` | REST & GraphQL architect that designs intuitive, consistent, and evolving APIs. |

### 🔍 Analysis & Exploration

| Agent | Mode | Description |
|-------|------|-------------|
| **[Codebase Explorer](agents/codebase-explorer.md)** | `Both` | Navigator that maps project structure, entry points, and data flow in unfamiliar code. |
| **[Debug](agents/debug.md)** | `Both` | Diagnostic specialist that systematically isolates and identifies bugs without guessing. |
| **[Security Audit](agents/security-audit.md)** | `Subagent` | Security engineer that audits code for vulnerabilities (OWASP/CWE) and compliance. |
| **[Perf Optimizer](agents/perf-optimizer.md)** | `Both` | Performance engineer that identifies bottlenecks and prescribes optimizations. |

### 🛠️ Development & Maintenance

| Agent | Mode | Description |
|-------|------|-------------|
| **[Refactor](agents/refactor.md)** | `Both` | Architect that improves code structure and maintainability without altering behavior. |
| **[Test Writer](agents/test-writer.md)** | `Both` | QA specialist that writes comprehensive unit, integration, and E2E test suites. |
| **[Docs Writer](agents/docs-writer.md)** | `Both` | Technical writer that creates clear, practical, and well-structured documentation. |
| **[Dependency Manager](agents/dependency-manager.md)** | `Both` | Specialist for keeping dependencies healthy, secure, and up-to-date. |

### 🧰 Specialized Skills

| Agent | Mode | Description |
|-------|------|-------------|
| **[Git Wizard](agents/git-wizard.md)** | `Both` | Version control expert for complex workflows, history rewriting, and recovery. |
| **[SQL Expert](agents/sql-expert.md)** | `Both` | Database engineer for optimized query writing and schema design. |
| **[Migrator](agents/migrator.md)** | `Subagent` | Specialist for safe database, API, and codebase migrations. |
| **[Regex Master](agents/regex-master.md)** | `Subagent` | Expert at crafting, explaining, and optimizing regular expressions. |
| **[Review](agents/review.md)** | `Subagent` | Senior engineer that conducts thorough code reviews for quality and correctness. |

## Usage

To use an agent in OpenCode, reference it by name:

```
@planner Help me breakdown the task of migrating our auth system
@debug Analyze why the login form is freezing
@architect specificy a microservices architecture for this app
```
