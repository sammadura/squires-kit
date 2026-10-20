---
name: squires-kit
description: Set up a local AI workspace around the user's work, with a guided interview, project folders, memory, reusable procedures, and upkeep rules. Use when the user asks to set up Squires Kit or create a new personal or business workspace.
disable-model-invocation: true
license: MIT
---

# Squires Kit

This is a free, open-source setup kit. Your AI application supplies the model and tools; this kit supplies instructions and templates. There is no payment, activation server, telemetry, or account check in this kit. Keep the MIT LICENSE with redistributed copies.

## Install the skill

If the user asked to install the downloaded kit, inspect its files first. Install this directory, including templates/ and LICENSE, as `~/.claude/skills/squires-kit/` for Claude Code. Never overwrite a different existing skill or workspace. If the same kit is already installed, compare files and ask before replacing changes. Report the actual installed path after reading the files back. Tell the user they can run `/squires-kit` in Claude Code, or ask to start Squires setup in plain language. If the current app cannot attach a zip, ask the user to unzip it and open the extracted folder locally. Do not claim an attachment alone installed anything.

## Start a workspace

1. Read this entire file. Ask whether this is for personal work or a business, and where the user wants their new workspace. Use a new dedicated folder; never overwrite or bootstrap the kit source directory or a folder holding unrelated work. If there is already a Squires workspace, help open that workspace and resume its progress instead of reinstalling.
2. Read `templates/personal.md` or `templates/business.md` in full. These include the complete setup interview, templates, connection guidance, safety rules, checkpoints and maintenance procedures. Do not blend the two editions.
3. Confirm the actual local host and filesystem access. Cloud-only chat is not a local installation. Create the chosen new folder using exclusive creation, copy the selected template to `CLAUDE.md`, and copy LICENSE. Read both back to verify them. For another supported local-file host, create `AGENTS.md` containing only a pointer to CLAUDE.md; do not change the host's permissions.
4. Help the user open the new folder as their actual local project. A shell directory change alone does not establish the app's active project. Give the exact folder path if they need to select it themselves.
5. Once the active local folder is verified, follow the selected template beginning at Phase 0. Ask the user before connecting services, sending messages or modifying external accounts. Do not make paid model choices or enable recurring jobs without their instruction. Preserve progress so setup can resume.
6. Complete the template's first real task and handoff checks. Distinguish copied files, configured connections, and verified completed work. Keep all personal records in the user's workspace, never in this distributable skill directory.

Installation and setup can use the host's existing file tools. No terminal commands, API keys or payments to Squires are required from the user. Claude Code and connected services have their own access requirements and pricing.
