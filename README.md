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

## What Problem Do We Solve?

| Pain Point | Without A Busy Bee | With A Busy Bee |
|---|---|---|
| Token burnout | 10,000-15,000 per module | ~5,000 per module (60-70% savings) |
| Rate limits | Hit walls, wait forever | Smart retry + queuing |
| Context overflow | AI forgets mid-task | Auto-snapshot & fresh sessions |

---

## The 3-Tool Strategy

| Tool | Role | Token Cost | When to Use |
|---|---|---|---|
| **GSD** | Planning, checklists, docs, tracking | ~200-400 | Every organizational task |
| **Everything-Claude-Code** | Coding, review, security, memory | ~800-2,000 (via subagent) | Main development work |
| **Superpowers** | TDD, complex debugging, failure recovery | ~1,200-1,500 | Only when truly needed |
| **Mem** | Remember lessons, decisions across sessions | ~0 (file-based) | Persistent memory |

**Result: Save 60-70% of tokens while delivering better code quality.**

---

## Quick Start - 2 Minutes

```bash
# 1. Clone the hive
git clone https://github.com/Olympusxvn/a_busy_bee.git
cd a_busy_bee

# 2. Open Claude Code
claude .

# 3. Deploy the bee
"Hey Busy Bee, plan a new module following the workflow."
```

---

## Install the 3 Core Tools

| Tool | Command |
|---|---|
| **GSD** | `npx get-shit-done-cc@latest` (run in terminal, choose Claude Code) |
| **Everything** | Visit [everything-claude-code](https://github.com/affaan-m/everything-claude-code) and follow instructions |
| **Superpowers** | Inside Claude Code: `/plugin install superpowers@claude-plugins-official` |

> Even without installing the separate tools, you can use this repo as a configuration template - just clone and open in Claude Code.

---

## What's Inside

```
a_busy_bee/
├── .claude/
│   ├── settings.json           # Token & context warnings
│   ├── subagents/              # Planner, coder, debugger
│   └── skills/                 # gsd-optimized, token-saver, mem
├── docs/
│   ├── strategy.md             # The 3-tool strategy explained
│   └── mem/                    # Persistent memory store
├── templates/
│   ├── plan-template.md        # Copy-paste for any module
│   └── spec-template.md        # 5-10 line spec template
└── README.md                   # You are here
```

---

## Why Developers Love A Busy Bee

| Benefit | What It Means For You |
|---|---|
| **Save $ on tokens** | 60-70% token reduction = lower API costs |
| **Ship faster** | Subagents work in parallel, not sequential |
| **No more context crashes** | Auto-snapshot before overflow |
| **Learn once, apply forever** | Persistent memory across sessions |
| **Zero lock-in** | Just templates + configs - take them anywhere |

---

## Sample Workflow

```
GSD: plan → save to file
Everything (subagent): code according to spec
Everything (review): review code
Superpowers (if error): debug with TDD
Mem: save lessons learned
```

---

## Contributing

We welcome all forms of contribution - from typo fixes to new subagents. See [CONTRIBUTING.md](CONTRIBUTING.md) for details.

- Report bugs: [Open an issue](https://github.com/Olympusxvn/a_busy_bee/issues/new?template=bug_report.md)
- Feature requests: [Request a feature](https://github.com/Olympusxvn/a_busy_bee/issues/new?template=feature_request.md)
- Share stories: How did A Busy Bee save your tokens?

First-time contributors welcome. Start with our `good first issue` label.

---

## License

MIT - Busy but free.

---

<div align="center">

**If this saved you tokens, [star the repo](https://github.com/Olympusxvn/a_busy_bee) to help others find it.**

[![Star History](https://img.shields.io/github/stars/Olympusxvn/a_busy_bee?style=social)](https://github.com/Olympusxvn/a_busy_bee)

*Busy. Smart. Thrifty.*

</div>
