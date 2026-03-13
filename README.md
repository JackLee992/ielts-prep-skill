# IELTS Prep Skill Repository

This repository contains two variants of the same IELTS preparation skill:

- `codex/ielts-prep/` for Codex
- `openclaw/ielts-prep/` for OpenClaw

## Install for Codex

```bash
git clone https://github.com/JackLee992/ielts-prep-skill ~/ielts-prep-skill
rm -rf ~/.codex/skills/ielts-prep
ln -s ~/ielts-prep-skill/codex/ielts-prep ~/.codex/skills/ielts-prep
```

## Install for OpenClaw

```bash
git clone https://github.com/JackLee992/ielts-prep-skill ~/ielts-prep-skill
rm -rf ~/.openclaw/skills/ielts-prep
ln -s ~/ielts-prep-skill/openclaw/ielts-prep ~/.openclaw/skills/ielts-prep
```

## Contents

- `codex/ielts-prep/`
  - Codex skill with `agents/openai.yaml`
- `openclaw/ielts-prep/`
  - OpenClaw skill with ClawHub-compatible metadata in `SKILL.md`
