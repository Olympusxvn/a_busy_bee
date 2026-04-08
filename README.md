# 🐝 A Busy Bee

> *Only 3 tools. No complexity. Save tokens.*

| Tool | Use for | Token |
|------|---------|-------|
| **GSD** | Planning, checklists, documentation | ~200–400 |
| **Everything** | Coding, review, security (via subagent) | ~800–2,000 |
| **Superpowers** | Hard debugging, TDD | ~1,200–1,500 |

## How to use
1. Clone this repo
2. Open Claude Code
3. Say: *"Hey Busy Bee, plan a module for me"*

## Sample workflow
- GSD: plan → save to file
- Everything (subagent): code according to spec
- Everything (review): review code
- Superpowers (if error): debug
  
🐝 A Busy Bee – Installation Guide
1. Prerequisites
Claude Code installed (latest version)

A GitHub account (to clone the repo)

2. Clone the repository
Open your terminal and run:

git clone https://github.com/olympusxvn/a_busy_bee.git
cd a_busy_bee

3. Install the 3 core tools (recommended)
To fully benefit from the strategy, install these tools:
  1. GSD: npx get-shit-done-cc@latest (run in terminal, choose Claude Code)
  2. Everything-Claude-Code: Visit github.com/affaan-m/everything-claude-code and follow instructions
  3. Superpowers: Inside Claude Code, type: /plugin install superpowers@claude-plugins-official

4. Usage
Open Claude Code inside the a_busy_bee folder:
bash
claude .

Claude will automatically read the configuration from .claude/ and the subagents.

Start by saying:

"Hey Busy Bee, plan a module for me"

5. Verify installation
Check that subagents appear in Claude Code (type /subagent to list them).
Run a small planning task using GSD.

💡 Quick tips
Even without installing the separate tools, you can use this repo as a configuration template – just clone and open in Claude Code to get the 3‑tool strategy ready.
Sample files in templates/ help you create plans and specs quickly.

🔗 Example repo
If you don't have the repo yet, you can fork from: https://github.com/example/a_busy_bee (link to be updated once you create it).

Happy coding with A Busy Bee – thrifty, effective, and simple! 🐝✨

   
