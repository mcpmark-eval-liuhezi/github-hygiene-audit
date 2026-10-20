# GitHub hygiene audit

Account: **HeziLiu** (https://github.com/HeziLiu)
Audit scope: every repository found under the account (including forks).

## 1. Per-repository findings

| Repository | Type | Open PRs | Workflows | Discussions | Open issues |
|---|---|---|---|---|---|
| HeziLiu/Little-rookie | Source (Java) | 0 | none | disabled | 0 |
| HeziLiu/Big-Buzzard | Source | 0 | none | disabled | 0 |
| HeziLiu/CodingInterviewChinese2 | Fork (C++) | 0 | none | disabled | 0 |
| HeziLiu/awesome-chatgpt-prompts-zh | Fork | 0 | none | disabled | 0 |

### HeziLiu/Little-rookie
- Description: "Undergraduate coursework" — Java, created 2018-05-15, last pushed 2019-06-02.
- Open pull requests: 0 (none).
- GitHub Actions workflows: none defined.
- Discussions: disabled (no categories).
- Open issues: 0.
- Verdict: dormant.

### HeziLiu/Big-Buzzard
- Description: "For future...." — created 2018-05-15, last pushed 2018-05-17.
- Open pull requests: 0 (none).
- GitHub Actions workflows: none defined.
- Discussions: disabled (no categories).
- Open issues: 0.
- Verdict: dormant.

### HeziLiu/CodingInterviewChinese2
- Fork of the "Sword Points to Offer" (《剑指Offer》) second-edition C++ source code — created 2019-03-12.
- Open pull requests: 0 (none).
- GitHub Actions workflows: none defined.
- Discussions: disabled (no categories).
- Open issues: 0.
- Verdict: dormant fork.

### HeziLiu/awesome-chatgpt-prompts-zh
- Fork of the ChatGPT Chinese prompt guide — created 2023-04-14.
- Open pull requests: 0 (none).
- GitHub Actions workflows: none defined.
- Discussions: disabled (no categories).
- Open issues: 0.
- Verdict: dormant fork.

## 2. Oldest open issue

No open issues exist in any repository under the account, so there is no oldest-open-issue record to report (no body, labels, or assignees to summarize).

## 3. Organization repository security advisories

- Organizations the account belongs to: **mcpmark-eval-liuhezi** (no teams).
- Attempted to list the organization's published repository security advisories; the request was rejected with `403 Resource not accessible by personal access token`, so this audit could not verify whether any advisories are published. No advisory data was accessible.

## 4. Cleanup actions taken

### Cleanup job 1 — workflow run logs older than 90 days
No GitHub Actions workflows are defined in any repository under the account, therefore there are no workflow runs at all and no run logs to delete. Nothing was old enough to bother; no logs were cleaned.

### Cleanup job 2 — mute dormant repositories (notifications → ignore)
All four repositories qualify as dormant (no open pull requests, no workflows, no open issues): Little-rookie, Big-Buzzard, CodingInterviewChinese2, and awesome-chatgpt-prompts-zh. The request to set each repository's notifications to "ignore" was rejected with `403 Resource not accessible by personal access token`, so no repository was successfully muted. None are muted as a result of this audit.

## 5. Publication notes

- Repository creation under the personal account (HeziLiu) was rejected with the same `403 Resource not accessible by personal access token` error, so this audit was published to the organization instead: **mcpmark-eval-liuhezi/github-hygiene-audit**, with AUDIT.md pushed to `main`.
- The notification "ignore" request for this audit repository was also rejected with `403 Resource not accessible by personal access token`, so the audit repository itself is not muted either.

## 6. Tooling limitation summary

All notification-mutating and org-repository-creation operations on the personal account require token scopes that the current personal access token does not grant. Everything read-only (repos, PRs, workflows, discussions, issues, advisories attempt) succeeded, and file writes to the organization succeeded.
