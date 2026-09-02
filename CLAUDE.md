# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repo is

The GLP ecosystem landing page — `README.md` (rendered as the repo's front page on GitHub) plus
`logo.svg`. There is no application code, no build, no tests, and no CI beyond Dependabot/CodeQL
housekeeping for the `.github` workflows. Editing this repo means editing `README.md` prose,
tables, or links, or replacing `logo.svg`.

## Purpose and audience

This is the *first thing a prospective user sees* — it links out to the four real GLP repos
(`gaggiuino-local-profiler`, `glp-integration`, `glp-lovelace-card`, `glp-order-card`) and gives
the one-page overview of what the ecosystem does and how to install all four pieces. It is not
where features, changelogs, or fixes live — those belong in the component repos.

## Keeping it in sync

Whenever a component gains/loses a feature, changes its install method, or a new component is
added to the ecosystem, this README's component list, feature table, and install steps need a
matching update — nothing here is auto-generated from the other repos.

## Pull requests

- **PR AI disclosure** — every PR fills the PR template's "AI assistance disclosure" section
  (`none`/`assisted`/`substantial`/`generated` + tool/model); every AI-assisted commit carries
  a `Co-Authored-By:` trailer. CI enforces it. See `CONTRIBUTING.md`.
