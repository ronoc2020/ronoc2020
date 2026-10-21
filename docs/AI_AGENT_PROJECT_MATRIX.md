# ROCS — optional AI gateway integration matrix

Last updated: 2026-10-21. **All rows below are design instructions, not evidence of runtime integration.**

Canonical rules: [Revenue Factory AI gateway policy](https://github.com/ronoc2020/revenue-factory/blob/main/docs/AI_GATEWAY_POLICY.md) and [setup/diagnostics](https://github.com/ronoc2020/revenue-factory/blob/main/docs/AI_GATEWAY_SETUP.md). If access to a linked private repo is unavailable, apply the explicit security rules in this matrix without assuming its contents.

| Project/workstream | Agent usage | API deployment decision |
| --- | --- | --- |
| Revenue Factory (CORE/COMMAND/TRUST/INTELLIGENCE/REVENUE) | Optional public/synthetic coding analysis and drafting; TRUST approval, RF low-write guardrails | **No live switch**; preserve approved Cloudflare provider/Workers AI, D1, financial state |
| ROCyber NEXT / nROCS site / 3D Spider OSINT | Use optional gateway for frontend coding and public/mock data evaluation only | No embedded browser API key; no unapproved external transmission of scanned targets, private security telemetry, client audit outputs |
| JEV / ROCS AI / OpenClaw / ROCSLAB Crew | Use a tested OpenAI-compatible model provider only if the selected agent supports tools/JSON; preserve existing local and remote backend configuration | May connect to local gateway only after isolated test, ToS approval, health checks and server capacity assessment |
| ROCS-LAB Debian 12 | Scripts, defensive rule ideas, sanitized docs | No blind gateway install; resource inventory first, no changes to ssh/fail2ban/firewall/monitoring, avoid destructive cleanup |
| DNA NCRY / n8n production pipeline | Public/synthetic prompts for storyboards, lyrics planning and workflow documentation; model support for image/audio is endpoint-specific | Never expose keys in browser or Git repo; no auto publishing to YouTube/TikTok until output QA, rights review, authentication, working n8n credentials |
| Poland Privé | Draft public travel descriptions and translated copy without guest PII | Commercial customer details, inquiries, booking/payment decisions stay on approved backend only; no live third-party inference without verified commercial ToS |
| Cyber//Crisis | Code assistance, game testing and synthetic narrative previews | No unreviewed runtime provider switch; preserve gameplay, privacy and competition build constraints |
| Shuttle Flow | Synthetic workflow/test data only | No passenger, driver, trip, expense or salary data on unapproved free gateway |
| KiwiKids Games / Plan lekcji | Development on public/synthetic examples | Child data must remain local/private; no client-side API keys or inference |
| New webdesign/portfolio projects | Prototype code, public documentation, design wording | Keep client contracts, private requirements and secrets out; static site should not call a local development gateway in production |

## Standard agent implementation process

1. Locate this project's actual repository/host and existing AI adapter. Do not assert access to a host based on its name.
2. Inventory provider, model, commercial permission, key storage, egress, timeout, budget, privacy and memory usage.
3. For an optional test, configure exactly **one** main gateway. OmniRoute is preferred for developer tooling; FreeLLMAPI is personal-experiment-only, not part of the production chain.
4. Test model discovery with no prompt. Then use public/synthetic benchmark prompts to verify tool calls, structured output, 429/5xx failover and no secret leakage.
5. Keep the existing provider unchanged until a separate reviewed code patch and documented stage tests. An agent-instructions file is not a deployment.
6. Document actual model IDs, runtime evidence, provider limits and fallback. Never label estimated aggregate tokens as an account grant.

## Current access/implementation status

- Agent instructions were added to accessible GitHub repos on 2026-10-21.
- The primary repo includes a read-only model-list checker.
- No direct SSH or n8n/ROCS-LAB management session was established in this workflow.
- No gateway container/process, provider key or paid/free quota has been verified in the runtime.
- Accordingly, nROCS, JEV, DNA NCRY and Poland Privé **do not become integrated merely from this matrix**.

**Security invariant:** no unauthenticated public proxy, no browser-side secret, no unapproved sensitive prompt egress, no subscription-limit bypass claims.
