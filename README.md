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

## Audio Companion Stack

This repository focuses on coaching and planning, but the current audio workflow depends on companion skills:

- `ielts-audio-analysis`
- `ielts-audio-director`
- `video-skills`

The companion audio stack now supports:

- English IELTS speaking and listening review
- Japanese study-audio review
- Local Japanese ASR comparison through:
  - `ja-kotoba`
  - `ja-whisper-large-v3`
  - `ja-reazonspeech`

When the task is mainly audio routing or model choice, route to `ielts-audio-director` first, then return to `ielts-prep` for study planning or drill follow-up.
