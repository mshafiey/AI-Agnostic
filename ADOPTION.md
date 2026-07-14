---
layout: default
title: Adoption Guide
---

[← Back to Home](/)

# Adopting the AI-Agnostic Principle

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

For the complete principle, see [Principle](principle).

---

## Migration Checklist

- [ ] Identify all AI-related files in repository
- [ ] Classify: Does this define product behavior?
- [ ] Move workflow files to developer environment
- [ ] Update `.gitignore` for AI config patterns
- [ ] Document product-related AI configs
- [ ] Communicate changes to team
- [ ] Update onboarding documentation

---

## File Classification Guide

| File Type | Location | Reason |
|-----------|----------|--------|
| System prompts for chatbots | Repository | Part of product |
| Claude.md | Developer environment | Personal workflow |
| Cursor rules | Developer environment | Personal workflow |
| Copilot instructions | Developer environment | Personal workflow |
| AI agent memory | Developer environment | Personal context |
| MCP configuration | Developer environment | Personal setup |
| Personal prompts | Developer environment | Personal workflow |
| Product AI features | Repository | Defines product |

For more examples, see the [FAQ](faq).

---

## Team Adoption

### For Team Leads

- Establish the principle as team standard
- Don't require specific AI tools
- Allow diverse AI preferences
- Focus reviews on product, not tools

### For Individual Developers

- Keep your AI workflow personal
- Don't commit AI configurations
- Share product-related AI configs only
- Respect others' tool choices

---

## Common Patterns

### Pattern: Shared AI Prompts

**Problem:** Team wants to share effective prompts

**Solution:** Create a "prompts" directory for product-related prompts only

### Pattern: AI-Assisted Code Review

**Problem:** Different developers use different AI review tools

**Solution:** Keep review configurations personal, share only the code

### Pattern: AI Training Data

**Problem:** Project uses AI for data processing

**Solution:** Keep training configs in repository if they define product behavior

---

## Enforcement

### Automated Checks

Add to CI/CD:

```bash
# Check for common AI config files in repository
find . -name "claude.md" -o -name ".cursorrules" -o -name "copilot-instructions.md"
```

### Code Reviews

- Reject commits with personal AI configs
- Accept product-related AI configurations
- Document exceptions clearly

---

## Success Metrics

- Developers can use any AI tool
- No AI-related merge conflicts
- Repository remains tool-agnostic
- New team members onboard easily

---

## Related Documentation

- [Home](/) - Project overview
- [Principle](principle) - Core definition and separation guidelines
- [Why](why) - Reasoning and benefits
- [Manifesto](manifesto) - Philosophical foundation
- [FAQ](faq) - Common questions and answers

**GitHub:** [https://github.com/mshafiey/AI-Agnostic](https://github.com/mshafiey/AI-Agnostic)