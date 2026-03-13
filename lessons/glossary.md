---
title: "Glossary"
slug: glossary
description: "Definitions of common terms used in OpenCode School."
---

## Agent

An AI assistant that can read files, write code, run commands, and perform tasks on your behalf. OpenCode's built-in agents include "build" (for making changes) and "plan" (for thinking through problems without making changes). You can also create custom agents for specialized tasks.

## AGENTS.md

A plain text file containing custom instructions that OpenCode reads at the start of every session. Think of it as a set of standing orders for the AI. Can exist globally (`~/.config/opencode/AGENTS.md`) or per-project (in the project root). The global one is personal to you; the project one is typically committed to Git and shared with your team.

## CLI

**Command-Line Interface.** A way to interact with software by typing text commands. OpenCode has a CLI for running one-off tasks, like `opencode run "explain this function"`. Unlike the [TUI](#tui), the CLI runs a single command and exits.

## Command

A slash-prefixed action you can run inside OpenCode, like `/models` to switch AI models, `/share` to share a conversation, or `/undo` to revert the last change. You can also create custom commands for repetitive tasks.

## Config

Short for configuration. A file (usually `opencode.jsonc`) where you define preferences for how OpenCode behaves — which [model](#model) to use, what [permissions](#permissions) to grant, which [MCP servers](#mcp) to connect, and more. Config files can be global (applying to all sessions) or per-project.

## GUI

**Graphical User Interface.** A visual interface with windows, buttons, and menus that you interact with using a mouse and keyboard. OpenCode Desktop is a GUI. Compare with [TUI](#tui) and [CLI](#cli).

## MCP

**Model Context Protocol.** An open standard that lets OpenCode connect to external tools and services. For example, you can add an MCP server that gives OpenCode access to your GitHub issues, Sentry error logs, or documentation search. MCP servers can be local (running on your machine) or remote (hosted on the internet).

## Mode

OpenCode has different operating modes. **Build mode** lets the agent make changes to your files. **Plan mode** restricts it to only reading and suggesting — useful for thinking through a problem before committing to changes. Switch between them with the Tab key in the TUI, or through the mode selector in Desktop.

## Model

The AI brain that powers OpenCode. Models are created by companies like Anthropic (Claude), OpenAI (GPT), and Google (Gemini). Different models have different strengths, speeds, and costs. You choose which model to use, and you can switch between them at any time.

## Permissions

Rules that control what OpenCode is allowed to do on your machine. Each action can be set to `allow` (run without asking), `ask` (prompt for approval), or `deny` (block entirely). For example, you might allow file reads but require approval before deleting files.

## Prompt

The message or instruction you type into OpenCode. A good prompt gives the AI enough context to do what you want. For example: "Add a dark mode toggle to the settings page" or "Explain how authentication works in this project."

## Provider

A company or service that hosts AI [models](#model). Anthropic, OpenAI, and Google are providers. OpenCode supports 75+ providers, including self-hosted options like Ollama for running models locally.

## Session

A single conversation with OpenCode. Each session has its own context and history. You can run multiple sessions in parallel, and you can share sessions with others using the `/share` command.

## Skill

A reusable set of instructions packaged as a `SKILL.md` file. Skills are loaded on-demand by OpenCode when they're relevant to the current task. Think of them as specialized knowledge packs — for example, a skill that knows how to draft release notes or set up a new React component.

## Tool

A capability that OpenCode's AI agent can use. Built-in tools include reading files, editing code, running shell commands, searching the web, and more. [MCP servers](#mcp) can add additional tools from external services.

## TUI

**Terminal User Interface.** A text-based interface that runs inside your terminal. OpenCode's TUI looks like a chat app but runs entirely in the terminal — no mouse needed. It's the original way to use OpenCode, and it's popular with developers who are comfortable in the terminal. Compare with [GUI](#gui) and [CLI](#cli).
