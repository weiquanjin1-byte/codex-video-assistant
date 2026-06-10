# Release Checklist

## Allowed Public Files

These files are intended for the first public GitHub release:

- `README.md`
- `LICENSE`
- `.gitignore`
- `docs/`
- `examples/`
- `agents/`
- `skills/`
- `aesthetic-score.md`
- `PROJECT.md`
- `COMPLIANCE.md`
- `ROADMAP.md`

## Files Not Recommended For Public Release

Do not commit these files or directories unless they have been manually cleaned and approved:

- `evidence/`
- `learning/`
- `sources/`
- `reports/`
- `output/`
- `data/`
- `assets/`
- `materials/`
- Local generated videos
- Raw production materials
- Private learning records
- Private user records
- API keys, tokens, cookies, secrets, credentials, or account files
- Unlicensed video, image, font, BGM, sound effect, icon, or voice assets

## Pre-Release Checks

Before running `git add`, verify:

- No API Key, token, Cookie, password, secret, or private account data is present.
- No private evidence records are included.
- No real user data, private messages, comments, account dashboards, phone numbers, or emails are included.
- No unlicensed video, image, font, BGM, sound effect, icon, voice asset, or likeness is included.
- No document claims that this project can bypass platform restrictions.
- No document claims that unverified trend data is factual.
- No document claims that generated content is automatically safe to publish.
- All unknown license or source status is marked as pending manual confirmation.

## Recommended GitHub Push Steps

Run these commands from the project root after manual review:

```powershell
git init
git branch -M main
git add README.md LICENSE .gitignore docs examples agents skills aesthetic-score.md PROJECT.md COMPLIANCE.md ROADMAP.md
git status --short
git commit -m "Initial open source release"
git remote add origin https://github.com/<your-username>/codex-video-assistant.git
git push -u origin main
```

Do not run `git add .` for the first release.

## Privacy Risk

Current privacy risk is low if the recommended `git add` command is used. The main remaining risk is accidental manual staging of internal folders such as `evidence/`, `learning/`, `sources/`, or `reports/`.

## Copyright Risk

Current copyright risk is low for the documentation-only release. It becomes medium or high if video, image, BGM, font, icon, sound effect, or voice files are added without confirmed authorization.

## Platform Compliance Risk

Current platform compliance risk is low because the public documentation explicitly forbids bypassing platform restrictions and fabricating trend data. Future online trend research must use public, authorized, or user-provided sources only.

## Final Rule

If a file is private, generated, credential-bearing, or license-unclear, do not publish it.
