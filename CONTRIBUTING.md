# Contributing

This repo is the **GLP ecosystem landing page** — `README.md` (the repo's GitHub front page)
plus `logo.svg`. There is no application code here.

Bugs or feature requests for a **component** (the app, the integration, or either card)
belong in that component's own repo — see the "Links" table in the README. Open an issue
here only when it is about the landing page itself (wrong/outdated info, broken link, logo).

## Pull requests

Every PR must:

- **Link an issue** — `Closes #N` in the description (no PRs without a linked issue)
- **Do one thing** — keep the diff focused; split unrelated changes
- **Use a Conventional Commits title in English** — `feat:` `fix:` `docs:` `chore:` `refactor:` `test:` `build:`
- **Explain what and why** in the description, not just what
- **Pass CI** — checks green before requesting review
- **Keep the README in sync** — component list, feature table and install steps must match
  the actual state of the ecosystem; nothing here is auto-generated
- **Disclose AI assistance** — see below
- **No real names** in commit messages, PR text or docs

### AI assistance

Be transparent about AI tool use so reviewers know what they are reviewing.

- **Per commit (machine-readable, required):** every commit an AI tool helped write carries a
  trailer, e.g. `Co-Authored-By: Claude <noreply@anthropic.com>` or
  `Co-Authored-By: Copilot <198982749+Copilot@users.noreply.github.com>`. Claude Code also
  adds a `Claude-Session:` trailer. The Claude trailer names the specific model, e.g.
  `Co-Authored-By: Claude Sonnet 5 <noreply@anthropic.com>` (see [CLAUDE.md](CLAUDE.md)).
- **Per PR (summary, required):** the "AI assistance disclosure" section of the PR template —
  one of `none` / `assisted` / `substantial` / `generated`, plus the tool and model names.

CI blocks the PR until the disclosure section is filled in, and fails on a contradiction
(commits carry an AI trailer while the PR claims `none`).

## Reporting a bug

For a problem with the landing page itself, open an issue with:

- What is wrong (outdated info, broken link, rendering issue) and where
- Expected vs. actual content
- For an install-steps problem: the app / card version you were following the steps with,
  and any relevant Home Assistant log output (`Settings → System → Logs`)
