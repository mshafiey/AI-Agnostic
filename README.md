---
layout: default
title: Home
---

# The AI-Agnostic Principle

> The brain that creates software should not be permanently attached to the software it creates.

## Overview

The AI-Agnostic Principle is a software development practice that separates AI development tools from software repositories.

Modern development increasingly relies on AI assistants like Claude, Cursor, Copilot, and others. While powerful, these tools introduce personal configurations that should remain separate from the shared codebase.

## Core Principle

> AI development configurations, instructions, memories, and workflows belong to the developer environment, not the software repository, unless they directly define the behavior of the software itself.

See the full [Principle Definition](PRINCIPLE.md).

## Why This Matters

Software projects outlast development tools. A repository created today may be maintained by developers using different AI systems in the future.

The source code should not depend on any specific AI workflow.

Read more in [Why This Principle Exists](WHY.md).

## Repository vs. Developer Environment

### Belongs in Repository

- Source code
- Tests
- Documentation
- Architecture decisions
- Product requirements
- Deployment configuration

### Belongs in Developer Environment

- Claude.md
- Cursor rules
- Copilot instructions
- Personal prompts
- AI agent memory
- MCP configuration
- Personal workflows

## Quick Start

### New Projects

1. Create your repository with standard structure
2. Add AI-related files to `.gitignore`
3. Keep AI configurations in your developer environment
4. Document product-related AI configs separately

### Existing Projects

1. Audit current AI files in the repository
2. Classify each as product vs. workflow
3. Move workflow files outside
4. Update `.gitignore`
5. Document the transition

See the full [Adoption Guide](ADOPTION.md).

## The Exception

AI configuration belongs in the repository **only when it becomes part of the product**.

**Example:** A chatbot application requires a system prompt. That prompt is software. A developer's Claude workflow is not software.

## Documentation

- [Principle](PRINCIPLE.md) - Core definition and separation guidelines
- [Why](WHY.md) - Reasoning and benefits
- [Manifesto](MANIFESTO.md) - Philosophical foundation
- [FAQ](FAQ.md) - Common questions and answers
- [Adoption](ADOPTION.md) - Implementation guide

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome. Please read the principle and manifesto before submitting changes.

The goal is to promote a development practice that allows humans and AI to collaborate freely without locking projects into specific artificial minds.