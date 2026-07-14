---
layout: default
title: Frequently Asked Questions
---

[← Back to Home](.)

# Frequently Asked Questions

## Is this anti-AI?

**No.**

This principle encourages AI usage. It only separates AI tools from software.

For more context, see [Why This Principle Exists](why).

---

## Should we delete all AI files?

**No.**

If AI configuration affects the final product, keep it in the repository.

If it only helps developers write code, keep it outside.

See the [Principle](principle) for complete separation guidelines.

---

## Why not share Claude.md?

Because another developer may use Cursor, Copilot, or another system.

The repository should not require one AI personality.

---

## Isn't documentation important?

**Yes.**

Documentation describes the software. AI instructions describe how one person wants an AI to work.

See the [Principle](principle) for what belongs where.

---

## What about team-shared AI prompts?

If a prompt becomes part of the product (like a chatbot system prompt), it belongs in the repository.

If it's a development workflow prompt, it belongs outside.

See the [Adoption Guide](adoption) for more patterns.

---

## Does this slow down adoption?

**No.**

It actually speeds adoption by reducing friction. Developers can use their preferred AI tools immediately.

---

## What if my AI config is public?

Public or private doesn't change the principle.

If it helps you write code but isn't part of the product, keep it outside.

---

## How do I migrate existing AI files?

1. Identify what's product vs. workflow
2. Move workflow files to your developer environment
3. Keep product-related AI config in the repository
4. Update `.gitignore` as needed

See the [Adoption Guide](adoption) for a complete migration checklist.

---

## Related Documentation

- [Home](.) - Project overview
- [Principle](principle) - Core definition and separation guidelines
- [Why](why) - Reasoning and benefits
- [Manifesto](manifesto) - Philosophical foundation
- [Adoption](adoption) - Implementation guide

**GitHub:** [https://github.com/mshafiey/AI-Agnostic](https://github.com/mshafiey/AI-Agnostic)