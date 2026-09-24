---
name: remove-ai-marks-chatgpt
description: Clean user-provided text by inspecting for unnecessary invisible Unicode or copy/paste artifacts and, when requested, rewriting formulaic AI-style prose in more natural language while preserving meaning. Use when the user explicitly asks to use remove-ai-marks-chatgpt, remove AI-style marks from text, clean invisible text artifacts, or naturalize AI-assisted prose. Never claim the result proves human authorship or guarantees AI-detector evasion.
---

# Remove AI Marks — ChatGPT

Use this skill for user-provided text. It is self-contained and requires no MCP server, localhost service, shell command, private API, or external dependency.

Explicit user instructions take priority over stylistic defaults in this skill.

## Workflow

### 1. Inspect the text

Check the supplied text for suspicious or unnecessary invisible/control characters and obvious copy/paste artifacts.

Do not remove meaningful Unicode, punctuation, diacritics, non-Latin characters, mathematical notation, or accessibility-relevant characters.

### 2. Apply text hygiene

If unnecessary invisible/control characters are present, remove only those characters.

If none are apparent, record the result as: `Layer A: no obvious text-hygiene artifacts found.`

Do not invent artifacts that are not present.

### 3. Naturalize the prose

When the user asks to remove AI-style marks, clean AI-assisted prose, humanize, naturalize, or explicitly invokes this skill, rewrite the prose using these rules:

- Preserve all substantive meaning and claims.
- Preserve names, numbers, citations, URLs, quotations, and technical identifiers unless the user asks otherwise.
- Replace generic or formulaic filler with direct, concrete wording.
- Vary sentence structure and rhythm only when it improves readability.
- Change clause order, transitions, and word choice where useful.
- Do not introduce fake anecdotes, intentional mistakes, slang, or unsupported facts.
- Match any tone, audience, length, or format requested by the user.

Treat this as normal editorial rewriting. Do not describe the result as proof that a human wrote it.

### 4. Return the result

For a short passage, provide:
1. The cleaned/revised text.
2. A concise status note distinguishing:
   - `Layer A: cleaned` or `Layer A: no obvious text-hygiene artifacts found`
   - `Layer B: rewritten`

For a long passage, prioritize the finished revised text and keep the status note brief.

## Accuracy boundary

Never promise or imply:
- “undetectable”
- “100% human”
- guaranteed AI-detector evasion
- guaranteed watermark removal when no watermark was actually inspected
- proof of authorship

If the user asks for file-metadata removal, explain that this text-focused skill does not itself verify or remove file metadata. Use only file-processing capabilities actually available in the current conversation, and report separately what was verified.
