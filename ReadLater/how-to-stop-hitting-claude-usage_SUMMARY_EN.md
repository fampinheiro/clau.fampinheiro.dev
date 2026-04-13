---
title: "Summary — How to stop hitting Claude usage limits"
source_url: "https://ruben.substack.com/p/how-to-stop-hitting-claude-usage"
author: "Ruben Hassid"
date_added: 2026-04-13
language: en
tags:
  - read-later
  - summary
  - Claude
  - token-usage
  - productivity
notes: "Personal summary for later reference."
---

Related link note: [[how-to-stop-hitting-claude-usage_EN]]

## Core idea

- Claude usage is dominated by **tokens** (roughly words). In long chats, each new message can become expensive because the model effectively **re-reads the full conversation history** before answering.

## Practical ways to reduce usage (high-level)

- **Keep conversations short**: long threads become “token furnaces.” Start a fresh chat when the topic changes.
- **Avoid unnecessary rework**: ask to redo *only the section* that’s wrong; avoid “redo the whole thing.”
- **Batch tasks into one prompt**: 1 message with 3 tasks is cheaper than 3 separate prompts (fewer full context reloads).
- **Use the Edit feature (Chat)**: edit the original prompt instead of sending follow-up corrections (“No, I meant…”), which adds more history.

## File + image handling

- Uploading documents/images can be very token-heavy (PDF pages, screenshots, DOCX/PPTX metadata).
- Prefer **extracting and pasting only the relevant text** into a clean text/markdown file.
- **Crop screenshots tightly** to the specific region needed.
- Avoid re-uploading the same docs into multiple chats.

## Pick the right tool / model for the job

- Use lighter/cheaper options for quick tasks; reserve heavyweight modes (e.g., extended thinking / top models) for tasks that truly need them.
- Plan the structure in cheaper chat first; then execute the build in the more expensive workspace feature (the article uses “Cowork” as the example).

## Manage context intentionally (projects, notes, restarts)

- If you must carry context, ask for **session notes** (key decisions + next steps), then start a new session using those notes as the seed.
- Use **Projects** (where supported) to keep frequently used files available/cached and reduce repeated tokenization.
- In long sessions where editing isn’t possible, **restart from an earlier message** or begin a new session with a one-line summary.

## Feature toggles

- Search/tools/connectors/research modes can increase token usage; turn them on only when needed.
- If using connectors, be specific (narrow queries reduce retrieval and context).

## Workflow tips

- Use more specific, context-rich prompts upfront (the article suggests voice dictation can help you provide better one-shot context).
- Remember usage limits can be a rolling window; splitting work across multiple sessions can help.
