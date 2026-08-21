---
name: pstack playbooks
description: Use before a crewmate drives a Cursor cloud agent for the first time on a project, or when a run is not converging.
---

# pstack playbooks

pstack is a Cursor plugin whose poteto-mode carries detailed playbooks for driving cloud agents: kicking off runs, following up on pull requests, checking run status, reading comments, and making sure work converges.

Grok Ship does not bundle or duplicate those playbooks. Read them at the source so they never go stale:

- Guide: https://github.com/cursor/plugins/blob/main/pstack/docs/guide/README.md
- Plugin source: https://github.com/cursor/plugins/tree/main/pstack
- Marketplace: https://cursor.com/marketplace/cursor/pstack

## When to read

- Before a crewmate drives its first Cursor cloud agent on a project, skim the guide and apply the playbook that matches the task (kickoff, PR follow-up, convergence).
- When a run is drifting - repeated red checks, an agent looping on the same fix, a PR sitting without progress - reread the convergence playbook before replying to the agent.

## Rules

- If pstack / poteto-mode is installed in the user's Cursor, prefer its playbooks when driving runs.
- If it is not installed, use the guide as reference only. Do not install it without a yes from the user.
- The playbooks inform how a run is driven. They do not replace Grok Ship factory rules: scout never opens a PR, ship still goes through adversarial review, and only the captain's word merges.

## Do not

- Do not copy playbook content into charters or skills - link, read, apply
- Do not treat the guide as authorization to skip the adversarial review or the captain's merge word
