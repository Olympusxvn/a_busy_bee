<div align="center">

# A Busy Bee

**Smart token orchestration for Claude Code**

[![Stars](https://img.shields.io/github/stars/Olympusxvn/a_busy_bee?style=flat)](https://github.com/Olympusxvn/a_busy_bee/stargazers)
[![Forks](https://img.shields.io/github/forks/Olympusxvn/a_busy_bee?style=flat)](https://github.com/Olympusxvn/a_busy_bee/network/members)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-Ready-blue)](https://claude.ai)

*Plan. Execute. Learn. Never waste a token.*

</div>

---

**A Busy Bee** is a strategic framework that orchestrates the best Claude Code tools into a seamless, token-efficient workflow. It automatically selects the cheapest tool for every job, spawns subagents to keep context clean, and learns from every session.

---

## What Problem Do We Solve?

| Pain Point | Without A Busy Bee | With A Busy Bee |
|---|---|---|
| Token burnout | 10,000-15,000 per module | ~5,000 per module (60-70% savings) |
| Rate limits | Hit walls, wait forever | Smart retry + queuing |
| Context overflow | AI forgets mid-task | Auto-snapshot & fresh sessions |

---

## The 3-Tool Strategy

A Busy Bee orchestrates three strategic tool groups, always picking the cheapest one that gets the job done:

| Tool | Role | Token Cost | When to Use |
|---|---|---|---|
| **GSD** | Planning, checklists, docs, tracking | ~200-400 | Every organizational task |
| **Everything-Claude-Code** | Coding, review (verdict and fix plan), security, rules | ~800-2,000 (via subagent) | Main development work |
| **Superpowers** | TDD, complex debugging, failure recovery | ~1,200-1,500 | Only when truly needed |
| **Mem** | Persistent memory across sessions | ~0 (file-based) | Lessons learned, decisions |

**Result: Save 60-70% of tokens while delivering better code quality.**

---

## Quick Start

```bash
# 1. Clone the hive
git clone https://github.com/Olympusxvn/a_busy_bee.git
cd a_busy_bee

# 2. Open Claude Code
claude .

# 3. Deploy the bee
"Hey Busy Bee, plan a new module following the workflow." or cd "your_project"
```

---

## Install the 3 Core Tools

| Tool | Command |
|---|---|
| **GSD** | `npx get-shit-done-cc@latest` (run in terminal, choose Claude Code) |
| **Everything** | Visit [everything-claude-code](https://github.com/affaan-m/everything-claude-code) and follow instructions |
| **Superpowers** | Inside Claude Code: `/plugin install superpowers@claude-plugins-official` |

> Even without installing the separate tools, you can use this repo as a configuration template -- just clone and open in Claude Code.

---

## What's Inside

```
a_busy_bee/
├── .claude/
│   ├── settings.json              # Token & context config
│   ├── agents/                    # Planner (Opus) + Code Reviewer (Sonnet)
│   ├── common/                    # 10 shared rules (security, testing, git, etc.)
│   ├── typescript/                # 5 TS-specific rules
│   ├── subagents/                 # Planner, Coder, Debugger
│   └── skills/                    # gsd-workflow, token-saver, mem
├── .github/
│   └── ISSUE_TEMPLATE/            # Bug report, feature request, question
├── docs/
│   ├── strategy.md                # The 3-tool strategy explained
│   └── mem/                       # Persistent memory store
├── templates/
│   ├── plan-template.md           # Copy-paste for any module
│   └── spec-template.md           # 5-10 line spec template
├── CONTRIBUTING.md                # How to contribute
└── README.md                      # You are here
```

---

## The Workflow

```
GSD: plan --> save to file
Everything (subagent): code according to spec
Everything (review): review code with code-reviewer agent
Superpowers (if error): debug with TDD
Mem: save lessons learned
```

---

## Integrated Rules & Agents

A Busy Bee ships with curated rules from [everything-claude-code](https://github.com/affaan-m/everything-claude-code):

**Rules** (`.claude/common/` and `.claude/typescript/`):
coding-style, security, testing, performance, patterns, git-workflow, code-review, hooks, agents, development-workflow

**Agents** (`.claude/agents/`):
- **Planner** -- creates comprehensive implementation plans with phases, risk assessment, and testing strategies
- **Code Reviewer** -- confidence-based review covering security, code quality, performance, and best practices

---

## Why Developers Love A Busy Bee

| Benefit | What It Means For You |
|---|---|
| **Save $ on tokens** | 60-70% token reduction = lower API costs |
| **Ship faster** | Subagents work in parallel, not sequential |
| **No more context crashes** | Auto-snapshot before overflow |
| **Learn once, apply forever** | Persistent memory across sessions |
| **Zero lock-in** | Just templates + configs -- take them anywhere |

---

## Contributing

We welcome all forms of contribution -- from typo fixes to new subagents. See [CONTRIBUTING.md](CONTRIBUTING.md) for details.

- Report bugs: [Open an issue](https://github.com/Olympusxvn/a_busy_bee/issues/new?template=bug_report.md)
- Feature requests: [Request a feature](https://github.com/Olympusxvn/a_busy_bee/issues/new?template=feature_request.md)
- Share stories: How did A Busy Bee save your tokens?

First-time contributors welcome. Start with our `good first issue` label.

---

## License

MIT -- Busy but free.

---

<div align="center">

**If this saved you tokens, [star the repo](https://github.com/Olympusxvn/a_busy_bee) to help others find it.**

[![Star History](https://img.shields.io/github/stars/Olympusxvn/a_busy_bee?style=social)](https://github.com/Olympusxvn/a_busy_bee)

*Busy. Smart. Thrifty.*

</div>
