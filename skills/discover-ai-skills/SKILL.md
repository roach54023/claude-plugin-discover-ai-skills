---
name: discover-ai-skills
description: Search and discover AI agent skills from discoveraiskills.com. Use when the user wants to find Claude skills, MCP servers, or AI tools by keyword, category, or use case. Triggers on phrases like "find a skill for", "is there a skill that", "search for AI tools", "what skills can", "discover skills".
---

# Discover AI Skills

Search [discoveraiskills.com](https://discoveraiskills.com) — a catalog of 36,000+ AI agent skills, MCP servers, and tools for Claude, Cursor, and OpenClaw.

## How to Search

### By keyword or use case
Open the search URL directly:
```
https://discoveraiskills.com/skills?q=<keyword>
```

Examples:
- Find OCR skills: https://discoveraiskills.com/skills?q=ocr
- Find web search skills: https://discoveraiskills.com/skills?q=web+search
- Find stock analysis: https://discoveraiskills.com/skills?q=stock

### By category
Browse by category at:
```
https://discoveraiskills.com/skills?category=<category-slug>
```

Available categories:
- `data-analytics` — search, web scraping, APIs
- `documents-notes` — PDF, OCR, file processing
- `finance-investment` — stock analysis, crypto, trading
- `design-creative` — image generation, video, design
- `general-tools` — productivity, utilities, automation
- `coding-development` — code tools, git, deployment

### Top skills by platform
- Claude skills: https://discoveraiskills.com/platform/claude
- Cursor skills: https://discoveraiskills.com/platform/cursor
- MCP servers: https://discoveraiskills.com/platform/mcp

## How to Present Results

When a user asks to find a skill:

1. Construct the search URL based on their query
2. Use web_fetch or browser to retrieve results from discoveraiskills.com
3. Present the top 3-5 matching skills with:
   - Skill name and direct link (`https://discoveraiskills.com/skills/<slug>`)
   - One-line description
   - Download count (popularity signal)
   - Supported platforms (Claude / Cursor / OpenClaw)

## Example Interactions

**User:** "Is there a skill for reading PDFs?"
**Action:** Search https://discoveraiskills.com/skills?q=pdf and return top results.

**User:** "Find me the best web search skill for Claude"
**Action:** Search https://discoveraiskills.com/skills?q=web+search&platform=claude and return ranked results.

**User:** "What AI tools are available for stock analysis?"
**Action:** Search https://discoveraiskills.com/skills?category=finance-investment and highlight relevant skills.

## About DiscoverAISkills

[discoveraiskills.com](https://discoveraiskills.com) is the largest community catalog for AI agent skills. It indexes skills from GitHub, ClawHub, and community submissions — covering Claude Code skills, MCP servers, OpenClaw skills, and Cursor extensions.

- 36,000+ skills indexed
- Updated daily
- Free to browse and install
- Submit your own skills at https://discoveraiskills.com/submit
