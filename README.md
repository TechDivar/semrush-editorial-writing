# Semrush Editorial Writing Framework

A reusable AI writing framework for producing clear, research-backed editorial guides with strong E-E-A-T signals.

It is packaged as a native Codex skill, but its instructions are plain Markdown and can also be used with ChatGPT, Claude, Gemini, Cursor, GitHub Copilot, and other AI assistants.

The framework applies editorial patterns observed in high-quality Semrush guides—without copying Semrush's wording, branding, or an individual writer's voice.

## What This Skill Does

Use this skill when you want an article that:

- answers the main question immediately;
- explains important terms in plain language;
- gives each section a clear, self-contained answer;
- uses primary sources, real examples, and transparent calculations;
- compares products using the same criteria;
- includes risks, limitations, methodology, and practical next steps; and
- recommends screenshots, diagrams, tables, or charts only when they help the reader.

It is especially useful for:

- explanatory guides;
- product and platform comparisons;
- tutorials and strategy articles;
- SEO, AEO, and GEO content;
- E-E-A-T content upgrades; and
- Pionex articles that need a richer editorial format.

## What “Semrush Style” Means Here

“Semrush style” refers to editorial structure—not copied content.

The skill uses these principles:

1. Start with a useful title and a direct introduction.
2. Define the subject before giving advanced advice.
3. Make every major section understandable on its own.
4. Move logically from understanding to action.
5. Support important claims with current, authoritative sources.
6. Use examples, calculations, screenshots, and data where they prove something.
7. State uncertainty, commercial relationships, risks, and limitations clearly.

The research behind these principles is documented in the [Semrush article format and E-E-A-T brief](references/semrush-article-format-and-eeat-brief.md).

## Use It With Your AI Assistant

### Codex

Ask Codex to install the skill from:

```text
https://github.com/TechDivar/semrush-editorial-writing
```

Or clone it manually into your Codex skills folder:

```bash
git clone https://github.com/TechDivar/semrush-editorial-writing.git ~/.codex/skills/semrush-editorial-writing
```

Restart or reopen Codex after installation if the skill does not appear immediately.

### ChatGPT, Claude, or Gemini

Download or attach these files to your chat, project, or custom assistant:

1. [`SKILL.md`](SKILL.md)
2. [`semrush-article-format-and-eeat-brief.md`](references/semrush-article-format-and-eeat-brief.md)
3. [`editorial-format.md`](references/editorial-format.md)
4. [`comparisons-eeat-and-pionex.md`](references/comparisons-eeat-and-pionex.md) when writing a comparison or Pionex article

Then prompt the assistant:

```text
Follow SKILL.md and its relevant reference files as the editorial instructions for this task. Write a source-backed guide about [topic] for [reader/brand].
```

### Claude Code, Gemini CLI, Cursor, or GitHub Copilot

Clone or copy the repository into your project. Tell the assistant to read `SKILL.md` and the relevant files in `references/` before drafting.

These tools use different names for project rules and agent instructions. The repository does not claim automatic installation on every platform; the Markdown instructions remain portable even when native skill discovery is unavailable.

### Any Other AI Tool

Paste `SKILL.md` into the tool's instruction area and provide the relevant reference files as context. If the tool accepts only one file, start with `SKILL.md` and the [full editorial brief](references/semrush-article-format-and-eeat-brief.md).

## How to Use It

In Codex, invoke the skill by name:

```text
Use $semrush-editorial-writing to write a source-backed guide about [topic].
```

The remaining example prompts work with any capable AI assistant after the files have been provided:

```text
Use $semrush-editorial-writing to compare three crypto cards. Show the fee calculations, risks, methodology, and visual recommendations.
```

```text
Rewrite this existing article in the Semrush editorial format. Preserve accurate information, verify changing claims, and flag unsupported statements.
```

```text
Use $semrush-editorial-writing for this Pionex article. Give it a distinct search intent, natural internal links, and useful image or chart instructions.
```

## Information That Improves the Result

The skill can begin with only a topic, but these inputs make the article stronger:

- target reader;
- website or brand;
- primary question or search intent;
- existing related articles;
- product or documentation links;
- approved claims and current data;
- original screenshots or test results; and
- desired call to action.

Missing facts should be researched and verified. First-hand experience, expert review, survey findings, or company-specific claims must never be invented.

## What the Skill Produces

The exact structure follows the topic, but a typical guide contains:

1. a benefit-led title;
2. a short answer-first introduction;
3. definitions and necessary context;
4. a process, framework, or normalized comparison;
5. source-backed examples or calculations;
6. costs, mistakes, risks, and limitations;
7. a practical checklist or decision framework;
8. methodology and primary sources; and
9. separate, actionable recommendations for images, charts, and screenshots.

It does not automatically add metadata, JSON-LD, social posts, or unrelated production assets unless requested.

## Repository Structure

```text
semrush-editorial-writing/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── semrush-article-format-and-eeat-brief.md
    ├── editorial-format.md
    └── comparisons-eeat-and-pionex.md
```

- [`SKILL.md`](SKILL.md) contains the reusable instructions. Its YAML header enables native discovery in skill-aware tools, while the Markdown body is readable by other assistants.
- [`semrush-article-format-and-eeat-brief.md`](references/semrush-article-format-and-eeat-brief.md) documents the analysis of the reference Semrush articles.
- [`editorial-format.md`](references/editorial-format.md) provides detailed article-structure guidance.
- [`comparisons-eeat-and-pionex.md`](references/comparisons-eeat-and-pionex.md) covers comparisons, calculations, disclosures, and Pionex-specific safeguards.

## Important Boundaries

- Do not copy Semrush's wording or visual identity.
- Do not invent experience, credentials, reviewers, quotes, or data.
- Do not describe a product as “best,” “safest,” or “highest” without current criteria and sufficient evidence.
- Do not use decorative visuals as substitutes for evidence.
- Treat changing fees, rates, availability, rules, and product features as time-sensitive.
- Apply the same scrutiny to the publisher's product and its competitors.

## Research Basis

The original editorial brief reviewed these Semrush articles on September 14, 2026:

- [Where does AI get its information? And how to get cited](https://www.semrush.com/blog/where-does-ai-get-its-information/)
- [Enterprise SEO: What it is & how to build a winning strategy](https://www.semrush.com/blog/enterprise-seo/)
- [Internal links: ultimate guide + strategies](https://www.semrush.com/blog/internal-links/)

This is an independent editorial-analysis project and is not affiliated with or endorsed by Semrush.
