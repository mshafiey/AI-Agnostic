---
layout: default
title: The Principle
---

[← Back to Home](.)

# The AI-Agnostic Principle

## Core Definition

> AI development configurations, instructions, memories, and workflows belong to the developer environment, not the software repository, unless they directly define the behavior of the software itself.

For more context, see [Why This Principle Exists](why) and the [Manifesto](manifesto).

---

## Visual Separation

```
┌─────────────────────────────────────────────────────────────┐
│                    SOFTWARE REPOSITORY                      │
│                                                             │
│  • Source code          • Tests             • Documentation  │
│  • Architecture decisions   • Product requirements          │
│  • Deployment configuration                                 │
└─────────────────────────────────────────────────────────────┘
                              │
                              │ SHARED REALITY
                              │
┌─────────────────────────────────────────────────────────────┐
│                  DEVELOPER ENVIRONMENT                      │
│                                                             │
│  • Claude.md           • Cursor rules       • Copilot       │
│  • Personal prompts    • AI agent memory    • MCP config    │
│  • Personal workflows                                        │
└─────────────────────────────────────────────────────────────┘
```

---

## What Belongs Where

### Inside the Repository

These items define the **product** itself:

- **Source code** - The implementation of the software
- **Tests** - Verification of correct behavior
- **Documentation** - Descriptions of the software's purpose and usage
- **Architecture decisions** - Structural choices that affect the product
- **Product requirements** - Specifications for what the software should do
- **Deployment configuration** - Settings for running the software in production

### Outside the Repository

These items define **how developers work**:

- **Claude.md** - Personal AI assistant configuration
- **Cursor rules** - Personal IDE AI settings
- **Copilot instructions** - Personal code completion preferences
- **Personal prompts** - Individual developer workflows
- **AI agent memory** - Personal context for AI assistants
- **MCP configuration** - Personal tool connections
- **Personal workflows** - Individual development practices

---

## The Exception

AI configuration belongs in the repository **only when it becomes part of the product**.

**Example:**

A chatbot application requires a system prompt → that prompt is software.

A developer's Claude workflow is not software.

For more examples and clarification, see the [FAQ](faq).

---

## Related Documentation

- [Home](.) - Project overview
- [Why](why) - The reasoning behind this principle
- [Manifesto](manifesto) - Philosophical foundation
- [FAQ](faq) - Common questions and answers
- [Adoption](adoption) - Implementation guide

**GitHub:** [https://github.com/mshafiey/AI-Agnostic](https://github.com/mshafiey/AI-Agnostic)