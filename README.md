# Skill From Masters

> **Stand on the shoulders of giants** — Create AI skills built on proven methodologies from domain experts.

A skill that helps you discover and incorporate frameworks, principles, and best practices from recognized masters before generating any new skill. Works with Claude Code, Codex, and other AI agent platforms.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Claude Code Skill](https://img.shields.io/badge/Claude%20Code-Skill-blue)](https://docs.anthropic.com/en/docs/agents-and-tools/claude-code/skills)

---

## Why This Skill?

Most professional domains have outstanding practitioners who have codified their methods through books, talks, interviews, and frameworks. A skill built on these proven methodologies is far more valuable than one created from scratch.

**The Problem:** When creating a new skill, it's easy to reinvent the wheel or miss well-established best practices.

**The Solution:** This skill acts as a "methodology curator" — it identifies relevant experts and frameworks, helps you select the right approaches, then hands off to skill-creator to generate a high-quality skill.

## How It Works

```
1. You: "I want to create a skill for user interviews"

2. Skill-from-masters surfaces relevant experts:
   - Rob Fitzpatrick (The Mom Test)
   - Steve Portigal (Interviewing Users)
   - Indi Young (Mental Models)
   - Clayton Christensen (Jobs to be Done)

3. You select which methodologies to incorporate

4. Skill-from-masters extracts actionable principles

5. Hands off to skill-creator to generate the final skill
```

## Methodology Database

The skill includes a curated database covering 15+ domains:

| Domain | Example Experts |
|--------|-----------------|
| Writing | Barbara Minto, William Zinsser, Amazon 6-pager |
| Product | Marty Cagan, Teresa Torres, Gibson Biddle |
| Sales | Neil Rackham (SPIN), Challenger Sale, MEDDIC |
| Hiring | Laszlo Bock, Geoff Smart, Lou Adler |
| User Research | Rob Fitzpatrick, Steve Portigal, JTBD |
| Engineering | Martin Fowler, Robert Martin, Kent Beck |
| Leadership | Kim Scott, Ray Dalio, Andy Grove |
| Negotiation | Chris Voss, Fisher & Ury |
| Startups | Eric Ries, Paul Graham, YC |

Plus an "Oral Tradition" section for experts who share primarily through talks and interviews (Steve Jobs, Elon Musk, Jensen Huang, etc.)

## Installation

### Option 1: Clone directly (Recommended)

```bash
# Navigate to your Claude Code skills directory
cd ~/.claude/skills  # or your custom skills path

# Clone this skill
git clone https://github.com/anthropics/skill-from-masters.git
```

### Option 2: Manual installation

1. Download or copy the `skill-from-masters` folder
2. Place it in your skills directory:
   - macOS/Linux: `~/.claude/skills/`
   - Windows: `%USERPROFILE%\.claude\skills\`

### Dependency

This skill works in conjunction with **skill-creator**. Make sure skill-creator is also available in your environment.

## Usage

Once installed, the skill automatically activates when you:

- Ask to create a new skill
- Mention wanting to build on best practices
- Request a skill for any domain covered in the methodology database

### Example

**You:** "Help me create a skill for writing product requirement documents"

**Skill-from-masters:**
> PRD writing spans several domains where experts have codified best practices:
>
> **Product Management:**
> - Marty Cagan: Problem-first PRDs, separating problem space from solution space
> - Teresa Torres: Continuous discovery, outcome-focused requirements
>
> **Business Writing:**
> - Barbara Minto: Pyramid Principle - lead with conclusion, MECE structure
> - Amazon: Working backwards, 6-page narrative format
>
> Which approaches resonate with how you want PRDs written?

**You:** "I like Amazon's approach combined with Cagan's problem-first thinking."

**Skill-from-masters:** *extracts key principles from both, then generates skill via skill-creator*

## File Structure

```
skill-from-masters/
├── skill-from-masters/
│   ├── SKILL.md                              # Core instructions
│   └── references/
│       └── methodology-database.md           # Curated expert frameworks
├── README.md
├── LICENSE
└── .gitignore
```

## Extending the Database

The methodology database can be extended. If a domain isn't covered:

1. Search for recognized experts in that field
2. Identify their core frameworks or methodologies
3. Add to the appropriate section in `methodology-database.md`
4. Submit a pull request!

## Contributing

Contributions welcome! Especially:

- Adding new domains and experts to the methodology database
- Improving existing framework descriptions
- Adding source links and references

Please:
1. Fork the repository
2. Create a feature branch
3. Submit a pull request

## License

MIT License — feel free to use, modify, and distribute.

---

**Philosophy:** The best skills aren't invented from scratch — they're built on the accumulated wisdom of masters who came before.
