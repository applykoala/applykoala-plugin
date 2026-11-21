# ApplyKoala for Claude Code

Run your job search from Claude Code, Codex, Cursor, ChatGPT or Claude. Your AI finds jobs that fit your resume, researches each company, tracks every application and helps you practise for interviews. Everything it saves goes into [ApplyKoala](https://applykoala.com), a job application tracker, so you can see and change it on your board in the browser.

This repository is a Claude Code plugin. It connects the ApplyKoala MCP server (`https://applykoala.com/mcp`) and adds a short job-search skill.

## What your AI can do

- **Find jobs**: job alerts bring new postings from about 9,500 companies' own careers pages (Greenhouse, Lever and Ashby), checked every hour. Your AI reads each posting in full and saves it word for word.
- **Research companies**: ratings, visa sponsorship, funding and news, each with a source link and the date it was checked.
- **Judge fit honestly**: it quotes your own resume for each requirement you meet and lists the gaps.
- **Track applications**: status, next steps, recruiters, interviews and what was said.
- **Write**: cover letters and form answers from your real experience.
- **Practise interviews**: mock interviews for a saved job, with notes on how you did over time.

ApplyKoala's tools never submit an application or delete anything for good. If your AI has its own browser, it can fill in and submit forms for you, and whether it asks you first is up to you. The free [Chrome extension](https://applykoala.com/extension) fills forms and leaves the Submit button to you.

## Install

### Claude Code (this plugin)

```
claude plugin marketplace add applykoala/applykoala-plugin
claude plugin install applykoala@applykoala
```

Then type `/mcp` in Claude Code and sign in to ApplyKoala.

Or add only the MCP server, without the skill:

```
claude mcp add --scope user --transport http applykoala https://applykoala.com/mcp
```

### Codex

```
codex mcp add applykoala --url https://applykoala.com/mcp
codex mcp login applykoala
```

### Cursor

Add this to `~/.cursor/mcp.json`, then open Customize in Cursor's sidebar, turn applykoala on and sign in:

```json
{ "mcpServers": { "applykoala": { "url": "https://applykoala.com/mcp" } } }
```

### ChatGPT and Claude (no terminal)

- **ChatGPT**: in a web browser, open chatgpt.com/plugins, choose Add → Add custom MCP server, paste `https://applykoala.com/mcp`, keep OAuth and press Connect.
- **Claude** (web, desktop or phone): under Connectors, add a custom connector with `https://applykoala.com/mcp`.

New to Claude Code or Codex? [How to install them without a terminal](https://applykoala.com/install-claude-code-or-codex).

## Things to say

- "Here is my resume. Find software engineer jobs in Singapore that fit me."
- "Research this company before I apply: visa sponsorship, ratings, recent news."
- "I had an interview with Acme today. Here is how it went."
- "Give me a mock interview for the data analyst job I saved."

## Pricing

ApplyKoala is free in the browser, with no account. Sync between devices, which the MCP server needs, costs US$3.99 a month or US$29 a year, with a 7-day free trial and no card needed. See [pricing](https://applykoala.com/pricing).

## Links

- [Connect your AI](https://applykoala.com/mcp)
- [Privacy](https://applykoala.com/privacy) · [Security and your data](https://applykoala.com/security)
- [What's new](https://applykoala.com/changelog)

## License

MIT for the files in this repository. The ApplyKoala service has its own [terms](https://applykoala.com/terms).
