---
layout: default
title: Home
---

<div class="hero">
  <h1>The AI-Agnostic Principle</h1>
  <p class="hero-subtitle">A principle for separating software from the artificial intelligence used to create it.</p>
  <p class="hero-quote">"The brain that creates software should not be permanently attached to the software it creates."</p>
  <div class="project-links">
    <a href="https://github.com/mshafiey/AI-Agnostic" class="project-link">GitHub Repository</a>
    <a href="https://mshafiey.github.io/AI-Agnostic/" class="project-link">Documentation</a>
  </div>
</div>

<div class="overview">
  <h2>Overview</h2>
  <p>Modern software development increasingly uses AI agents such as Claude, Cursor, GitHub Copilot, and other autonomous development systems. These tools introduce a new type of project artifact that should remain separate from the software repository itself.</p>
  
  <div class="principle-definition">
    <blockquote>
      <strong>The AI-Agnostic Principle states:</strong><br>
      AI development configurations, instructions, memories, and workflows belong to the developer environment, not the software repository, unless they directly define the behavior of the software itself.
    </blockquote>
  </div>
</div>

<div class="visual-separation">
  <h2>Visual Separation</h2>
  <div class="diagram">
    <div class="repository-box">
      <h3>SOFTWARE REPOSITORY</h3>
      <ul>
        <li>Source code</li>
        <li>Tests</li>
        <li>Documentation</li>
        <li>Architecture decisions</li>
        <li>Product requirements</li>
        <li>Deployment configuration</li>
      </ul>
    </div>
    
    <div class="arrow">
      <span>SHARED REALITY</span>
    </div>
    
    <div class="environment-box">
      <h3>DEVELOPER ENVIRONMENT</h3>
      <ul>
        <li>Claude.md</li>
        <li>Cursor rules</li>
        <li>Copilot instructions</li>
        <li>Personal prompts</li>
        <li>AI agent memory</li>
        <li>MCP configuration</li>
        <li>Personal workflows</li>
      </ul>
    </div>
  </div>
</div>

<div class="exception">
  <h2>The Exception</h2>
  <p>AI configuration belongs in the repository <strong>only when it becomes part of the product</strong>.</p>
  <p><strong>Example:</strong> A chatbot application requires a system prompt → that prompt is software. A developer's Claude workflow is not software.</p>
</div>

<div class="documentation">
  <h2>Documentation</h2>
  <div class="doc-grid">
    <a href="principle" class="doc-card">
      <h3>Principle</h3>
      <p>Core definition and separation guidelines</p>
    </a>
    
    <a href="why" class="doc-card">
      <h3>Why</h3>
      <p>Reasoning and benefits of the principle</p>
    </a>
    
    <a href="manifesto" class="doc-card">
      <h3>Manifesto</h3>
      <p>Philosophical foundation</p>
    </a>
    
    <a href="faq" class="doc-card">
      <h3>FAQ</h3>
      <p>Common questions and answers</p>
    </a>
    
    <a href="adoption" class="doc-card">
      <h3>Adoption</h3>
      <p>Implementation guide</p>
    </a>
  </div>
</div>

<div class="cta">
  <h2>Get Started</h2>
  <p>Ready to adopt the AI-Agnostic Principle in your projects?</p>
  <a href="adoption" class="cta-button">Read the Adoption Guide</a>
</div>

<div class="github">
  <h2>GitHub</h2>
  <p>View the source code and contribute on GitHub:</p>
  <a href="https://github.com/mshafiey/AI-Agnostic" class="github-button">GitHub Repository</a>
</div>