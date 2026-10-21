# GitHub Hygiene Audit — HeziLiu

**Audit date:** 2026-10-21
**Account:** https://github.com/HeziLiu (Hezi Liu)
**Purpose:** Pre–performance-review sweep of the entire GitHub presence; consolidated record of findings per repository.
**Durable record:** this file (github-hygiene-audit.md) + issues #1–#4 in this repository.

---

## 1. Repositories audited (4)

| # | Repository | Type | Language | Created | Last pushed | Open issues |
|---|------------|------|----------|---------|-------------|-------------|
| 1 | [Little-rookie](https://github.com/HeziLiu/Little-rookie) | Source (own) | Java | 2018-05-15 | 2019-06-02 | 0 |
| 2 | [CodingInterviewChinese2](https://github.com/HeziLiu/CodingInterviewChinese2) | Fork | C++ | 2019-03-12 | 2018-12-28 | 0 |
| 3 | [awesome-chatgpt-prompts-zh](https://github.com/HeziLiu/awesome-chatgpt-prompts-zh) | Fork | — | 2023-04-14 | — | 0 |
| 4 | [Big-Buzzard](https://github.com/HeziLiu/Big-Buzzard) | Source (own, empty) | — | 2018-05-15 | 2018-05-17 | 0 |

All four repositories are public; none archived.

## 2. Per-repository findings

### 2.1 Little-rookie
- **Secret scanning alerts:** could not be verified — API returned `403 Resource not accessible by personal access token` (token lacks `security_events` scope). Not confirmed clear.
- **Open pull requests:** none found.
- **Review comments on open PRs:** none found (no open PRs exist).
- **Discussions:** none found.
- **Releases:** none found — no release has ever been published (`releases/latest` → 404). No newest-release tag name or release notes to report.

### 2.2 CodingInterviewChinese2 (fork)
- **Secret scanning alerts:** could not be verified — same `403` token-scope limitation. Not confirmed clear.
- **Open pull requests:** none found.
- **Review comments on open PRs:** none found (no open PRs exist).
- **Discussions:** none found.
- **Releases:** none found (`releases/latest` → 404). No tag name or release notes to report.

### 2.3 awesome-chatgpt-prompts-zh (fork)
- **Secret scanning alerts:** could not be verified — same `403` token-scope limitation. Not confirmed clear.
- **Open pull requests:** none found.
- **Review comments on open PRs:** none found (no open PRs exist).
- **Discussions:** none found.
- **Releases:** none found (`releases/latest` → 404). No tag name or release notes to report.

### 2.4 Big-Buzzard
- **Secret scanning alerts:** could not be verified — same `403` token-scope limitation. Not confirmed clear.
- **Open pull requests:** none found.
- **Review comments on open PRs:** none found (no open PRs exist).
- **Discussions:** none found.
- **Releases:** none found (`releases/latest` → 404). No tag name or release notes to report.

## 3. Organization team memberships

- **Organization:** mcpmark-eval-liuhezi
- **Teams:** none found — the account belongs to the organization but is a member of no team within it.

## 4. Tracking issues (durable record)

**Location:** https://github.com/mcpmark-eval-liuhezi/github-hygiene-audit/issues

| Issue | Repository audited |
|-------|--------------------|
| [#1 Audit: Little-rookie](https://github.com/mcpmark-eval-liuhezi/github-hygiene-audit/issues/1) | Little-rookie |
| [#2 Audit: CodingInterviewChinese2](https://github.com/mcpmark-eval-liuhezi/github-hygiene-audit/issues/2) | CodingInterviewChinese2 |
| [#3 Audit: awesome-chatgpt-prompts-zh](https://github.com/mcpmark-eval-liuhezi/github-hygiene-audit/issues/3) | awesome-chatgpt-prompts-zh |
| [#4 Audit: Big-Buzzard](https://github.com/mcpmark-eval-liuhezi/github-hygiene-audit/issues/4) | Big-Buzzard |

Each issue body summarizes that repository's findings and carries a follow-up comment with concrete recommended next steps.

**Note on location:** the request was to file these in a private `github-hygiene-audit` repository under the personal account. Creating a repository under `HeziLiu` was rejected with `403 Resource not accessible by personal access token` (verified afterwards that no `HeziLiu/github-hygiene-audit` exists). The durable record was therefore filed in the existing audit repository `mcpmark-eval-liuhezi/github-hygiene-audit` — the organization the account belongs to — which is the location an earlier audit session also fell back to for the same reason (see `AUDIT.md`, publication notes).

**Publication note:** the request also asked for a secret gist named `github-hygiene-audit.md`. Gist creation was likewise rejected with `403 Resource not accessible by personal access token`, so the consolidated report was committed to this repository as `github-hygiene-audit.md` instead (this file).

## 5. Executive summary

- **4 repositories audited**, all public, all dormant (no open PRs, no discussions, no releases anywhere).
- **Security-relevant:** no open pull requests (hence no review comments) on any repo; no releases; no discussions. **Secret scanning could not be verified via API** (token scope limitation) — this is the single outstanding verification gap; check each repo's Security tab in the web UI.
- **Team memberships:** member of organization `mcpmark-eval-liuhezi`, **no teams**.
- **Tracking:** one issue per audited repository in `mcpmark-eval-liuhezi/github-hygiene-audit` (issues #1–#4 above), each with a recommended-next-steps comment.

## 6. Recommended next steps

1. Verify secret scanning manually in each repo's Security tab (the only unverified category).
2. Delete or archive the two dormant forks and the empty Big-Buzzard repo to shrink future audit surface.
3. Read through Little-rookie (2018–2019 coursework) for any sensitive content.
4. If a private audit repo under the personal account is desired, create `HeziLiu/github-hygiene-audit` via the web UI with a fully-scoped token or by hand, and re-point the tracking issues there.
5. If a secret gist is the required deliverable format, create it manually with the content of this file (gist creation was blocked by the token's scopes).

---

*Methodology: repositories enumerated via GitHub search including forks (4 total, matching the profile's public-repo count); secret scanning, open PRs (plus their review comments), discussions, and latest release queried per repository; team memberships queried for the authenticated user. All "none found" statements are backed by empty API results; items that could not be verified due to permissions are explicitly labeled rather than reported as clear.*