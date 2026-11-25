# Claude Skills by Pionarius

**Practical skills for Claude Code and Claude: SEO, GEO (getting cited by ChatGPT, Perplexity and AI Overviews), WordPress content, and checking third-party skills before you install them.**

Built and used every day at [Pionarius](https://pionarius.com), an AI consulting and training firm in France that has trained 547+ people on AI since 2023. Every skill is plain `SKILL.md`: no scripts, no API keys, nothing that runs on your machine.

English versions live in [`skills/`](skills). French versions live in [`skills-fr/`](skills-fr).

## The skills

| Skill | What it does | Use it when |
|---|---|---|
| [`seo-content`](skills/seo-content/SKILL.md) | Three modes in one: refresh an article against the top 5 Google results, rewrite titles and meta descriptions from the live SERP, and map the questions buyers actually type into ChatGPT and Google | A post is stuck on page 2, titles get cut off, or you don't know what to write next |
| [`seo-geo-audit`](skills/seo-geo-audit/SKILL.md) | One-pass SEO + GEO audit scored out of 100, with the 3 actions for this week and ready-to-paste robots.txt, llms.txt and JSON-LD | You want to know why Google or AI assistants ignore a site |
| [`wordpress-seo-geo-writer`](skills/wordpress-seo-geo-writer/SKILL.md) | Writes a WordPress-ready article built to rank on Google and to be quoted by AI search engines, with FAQ and schema | You need a blog post that both Google and ChatGPT will pick up |
| [`skill-security-check`](skills/skill-security-check/SKILL.md) | Reviews a skill, plugin or MCP server before install: hidden instructions, key theft, exfiltration, shady install scripts. Verdict in one line | Someone shares a skill in a reel, a tweet or a comment |
| [`prepare-clear`](skills/prepare-clear/SKILL.md) | Saves rules, state and deadlines to a file before you type `/clear`, with the exact sentence to resume | You want a fresh context without losing the plan |
| [`prepare-compact`](skills/prepare-compact/SKILL.md) | Tidies and archives the tracking file before you type `/compact`, so no instruction or deadline is lost | A long session is getting heavy |

## Install

**Claude Code, with the skills CLI** (all skills, or pick one):

```bash
npx skills add equipepionarius-collab/claude-skills
npx skills add equipepionarius-collab/claude-skills --skill seo-content
```

**Claude Code, as a plugin:**

```
/plugin marketplace add equipepionarius-collab/claude-skills
/plugin install pionarius-skills@pionarius
```

**Claude Code, by hand:**

```bash
git clone https://github.com/equipepionarius-collab/claude-skills.git
cp -r claude-skills/skills/* ~/.claude/skills/
```

**Claude (web, desktop, mobile):** download a skill folder, zip it, then add it in your Claude settings under Skills.

## Try it

```
Use seo-content to refresh https://yoursite.com/blog/your-post
Run seo-geo-audit on https://yoursite.com
Run skill-security-check on https://github.com/someone/some-skill before I install it
```

## How these skills behave

- **Real research, never memory.** They search Google, Reddit and Quora live, and they say "not measured" instead of guessing.
- **No invented numbers.** Every figure is dated and sourced, or left out.
- **No live changes without you.** Audits produce fixes to paste; rewrites wait for your approval of the plan.
- **Plain text only.** Easy to read, fork and adapt to your own brand rules.

## Credits

`seo-content` adapts `blog-refresher`, `seo-title-optimization` and `customer-journey` from [Illyism/seo-skills](https://github.com/Illyism/seo-skills) (MIT). `seo-geo-audit` draws on [AgriciDaniel/claude-seo](https://github.com/AgriciDaniel/claude-seo), [Auriti-Labs/geo-optimizer-skill](https://github.com/Auriti-Labs/geo-optimizer-skill) and [every-app/open-seo](https://github.com/every-app/open-seo) (MIT). `skill-security-check` follows the attack categories of [NVIDIA/SkillSpector](https://github.com/NVIDIA/skillspector) (Apache-2.0).

## License

MIT. If a skill helps you, a star helps others find it.

Need AI training or an AI rollout for your team? [pionarius.com](https://pionarius.com)
