# AGENTS.md: gitea-phorge-theme

Instructions for anyone working in this repository, human or AI assistant. The organization-wide rules (issues, pull requests, time tracking, security reporting) are in [phorge-fr/.github](https://github.com/phorge-fr/.github/blob/main/AGENTS.md) and [GOVERNANCE.md](https://github.com/phorge-fr/.github/blob/main/GOVERNANCE.md).

## What this repository is

A small theme for Gitea/Forgejo, served by the Phorge Forgejo instance: templates in `templates/` and static assets in `public/`. See the [README](README.md) for how it is applied.

## Workflow

One issue per change, a short branch from the current `origin/main`, one pull request with `Closes #N`; never commit to `main`; text in English. The pull request needs `governance / pr-governance`.

## Rules

- Serve first-party assets only: no third-party CDN fonts, scripts or images (see the GDPR notes in `phorge-fr/Hangar` `docs/gdpr.md`).
- Check a change against the Forgejo version that the Hangar `svc` cluster runs before opening the pull request; a template that does not match the upstream structure breaks pages.
