# OpenCode Agents

This repository provides a collection of specialized agents tailored for the OpenCode ecosystem. Each agent is designed with a specific focus, enabling them to handle complex software engineering tasks with expert-level proficiency and precision.

## Agent Modes

Agents within this repository operate in three distinct modes:

- **Agent**: Primary assistants designed for direct user interaction, high-level reasoning, and project management.
- **Subagent**: Specialized tools intended to be called by other agents to perform specific, narrow tasks.
- **Both**: Versatile agents that can function as either a primary assistant or a delegated subagent depending on the context.

## Available Agents

### Architecture and Planning

| Agent | Mode | Description |
| :--- | :--- | :--- |
| **[System Architect](agents/architect.md)** | Agent | Principal expert for high-level system design, architectural patterns, and long-term technical strategy. |
| **[Planner](agents/planner.md)** | Agent | Lead strategist that breaks down complex project goals into manageable, actionable, and dependency-aware execution plans. |
| **[API Designer](agents/api-designer.md)** | Agent | Specialist in designing intuitive, consistent, and scalable RESTful and GraphQL APIs following industry best practices. |

### Analysis and Exploration

| Agent | Mode | Description |
| :--- | :--- | :--- |
| **[Codebase Explorer](agents/codebase-explorer.md)** | Both | Navigation expert that maps project structures, identifies key entry points, and understands data flow across unfamiliar codebases. |
| **[Debug Specialist](agents/debug.md)** | Both | Diagnostic expert that uses systematic analysis to isolate, identify, and resolve complex bugs without trial and error. |
| **[Security Auditor](agents/security-audit.md)** | Subagent | Security-focused engineer that audits codebases for vulnerabilities (OWASP/CWE) and ensures compliance with security standards. |
| **[Performance Optimizer](agents/perf-optimizer.md)** | Both | Performance engineer dedicated to identifying performance bottlenecks and implementing efficient optimizations. |

### Development and Maintenance

| Agent | Mode | Description |
| :--- | :--- | :--- |
| **[Frontend Specialist](agents/frontend.md)** | Both | UI/UX expert for component architecture, state management, accessibility, styling, and frontend performance optimization. |
| **[Refactoring Expert](agents/refactor.md)** | Both | Specialist in improving code structure, readability, and maintainability while ensuring original behavior remains intact. |
| **[Test Writer](agents/test-writer.md)** | Both | QA automation expert focused on creating comprehensive test suites including unit, integration, and end-to-end tests. |
| **[Documentation Writer](agents/docs-writer.md)** | Both | Technical writer who creates clear, practical, and well-structured documentation for developers and users. |
| **[Dependency Manager](agents/dependency-manager.md)** | Both | Specialist in managing project dependencies, handling upgrades, auditing for security holes, and optimizing package footprints. |

### Specialized Skills

| Agent | Mode | Description |
| :--- | :--- | :--- |
| **[AI/ML Specialist](agents/ai-ml.md)** | Both | Machine learning engineer for LLM integration, prompt engineering, RAG pipelines, model training, and MLOps. |
| **[Git Wizard](agents/git-wizard.md)** | Both | Version control expert for managing complex Git workflows, history management, and repository recovery. |
| **[SQL Expert](agents/sql-expert.md)** | Both | Database engineer specializing in writing optimized SQL queries, designing efficient schemas, and tuning database performance. |
| **[Migration Specialist](agents/migrator.md)** | Subagent | Expert in managing safe migrations for database schemas, API versions, and large-scale codebase upgrades. |
| **[Regex Master](agents/regex-master.md)** | Subagent | Specialist in crafting, explaining, and optimizing complex regular expression patterns for data processing and validation. |
| **[Code Reviewer](agents/review.md)** | Subagent | Senior engineer that provides thorough code reviews, focusing on quality, correctness, and adherence to best practices. |

## Usage

To utilize these agents within OpenCode, you can reference them by their name using the `@` symbol:

```bash
@planner Help me break down the task of migrating our authentication system.
@debug Analyze why the login form is freezing during submission.
@architect Specify a microservices architecture for this application.
@sql-expert Optimize this query for the orders table.
```

Each agent is configured with its own set of tools and permissions to ensure they can work effectively while maintaining system security. For more details on a specific agent, please refer to its individual documentation file in the `agents/` directory.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
