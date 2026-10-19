---
type: Fact
title: Stale text to fix for the observatory event
description: "Earlier-delivery leftovers (ISS/Codespaces text, the HCI demo, the Discussions link, old contacts) were fixed by 2026-10-18; the pyproject name is kept as is."
tags: [todo, docs, cleanup]
generated: { by: "claude-code:claude-opus-5-5", at: "2026-10-19T04:43:05Z" }
status: stable
code_refs: [docs/workshop-outline.md, .github/ISSUE_TEMPLATE/config.yml, pyproject.toml]
---

## Known stale references (as of 2026-10-18)

- `pyproject.toml` project name is `coding-with-agents-workshop`; only
  `pixi.toml` uses `viss-observatory-workshop-2026`. A rename was scrapped
  on 2026-10-18 (Anshul Tambay), so the name stays as is for now.

## Fixed (2026-10-16)

- The Codespaces + Copilot Chat assumptions in README, the block READMEs,
  slides, notebooks, docs, rules and `.devcontainer/` were rewritten for
  Claude Code on the JupyterHub, and the outline's event, prerequisites and
  Block 3 description were updated. Copilot still appears where it is
  compared with other tools (Block 1 landscape, audience Q&A, resources).
- The outline no longer names the ISS/Raleigh event or the schmidt-sciences
  team link.

## Fixed (2026-10-18)

- The HCI text-entry demo, its five statistical-loop skills, the stats
  reference doc and the `research-data-scientist` subagent were removed, and
  every reference to them updated (see
  [the Block 3 decision](../decisions/block3-fits-to-zarr-example.md)).
- Remaining participant-facing Copilot/VS Code/Codespaces leftovers were
  fixed: Block 4 resources and the audience Q&A no longer claim the repo
  keeps Copilot copies of the gallery, the pre-block checklist says
  "JupyterHub terminal", and the devcontainer comment no longer mentions
  Codespaces.
- `.github/ISSUE_TEMPLATE/config.yml` no longer links GitHub Discussions
  (disabled on this repo).
- The Contact section of `docs/workshop-outline.md` lists only Anshul Tambay
  (Tina Dang removed at Anshul Tambay's request).

## Sources

Repo inspection and repo-history research, 2026-10-15; Anshul Tambay, 2026-10-18 (repo cleanup on branch `cleanup-stale-content`).

# Related Concepts
- [Repository lineage and past deliveries](repo-lineage.md): leftovers from earlier deliveries
- [Deliver the Florence tutorial on the Schmidt JupyterHub, not Codespaces](../decisions/delivery-on-jupyterhub.md): text that assumes the superseded Codespaces delivery
