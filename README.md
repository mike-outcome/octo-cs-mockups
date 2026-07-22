# Octo — Customer Solutions Redesign Mockups

Interactive mockups for the rebuilt Customer Solutions area in Internal Octo.

**Live:** https://mike-outcome.github.io/octo-cs-mockups/

Based on the Andrew / Mike working session (Jul 21, 2026) and the whiteboard.

## Screens

| Screen | What it answers |
|---|---|
| **Landing page** | Global KPIs, projects grouped by client, each row showing timeline / current status / owners |
| **Project Overview** | Size, health score, generated status summary, to-dos, blockers, RACI, stakeholders |
| **Timeline** | Start → projected → revised → real end date, with required rationale per revision and time-in-phase |
| **Tasks** | Dev tasks (Linear sync) + CS tasks, blocker flags, assignees |
| **Summary Log** | Timestamped record of every published status update |
| **Documentation** | Required docs with missing-doc flagging, transcripts, HubSpot emails, Create-PRD action |

## Decisions reflected here

- Progress bars replaced with a real timeline.
- Start date auto-derived from the kickoff call (Slack/email); projected end date locked at scoping.
- Revised end dates are additive and each requires a free-text rationale — visible on hover and in the revision history.
- Real end date auto-filled from the deployment email.
- T-shirt sizing (S/M/L/XL) alongside $ ARR.
- Projects grouped by client.
- Blockers are a flag on any Dev or CS task, mirroring the Linear label.
- Required documentation is flagged when missing and pulls down the health score.
- Landing KPIs: $ ARR being deployed, $ ARR expected live this quarter, avg. time remaining, # live deployments, # healthy, # unhealthy.

## Notes

Single self-contained `index.html`. All data is illustrative. Hash routing: `#/`, `#/project/overview`, `#/project/timeline`, `#/project/tasks`, `#/project/log`, `#/project/docs`.
