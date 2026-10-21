# ROCS ecosystem — general agent instructions

This is a GitHub profile/coordination repository, not a deployment root for every ROCS project. Never infer access to private Debian hosts, Cloudflare projects, n8n instances or missing repos. Use source evidence and explicit repository ownership; do not silently modify forks or unrelated upstream projects. Use project-specific instructions first, then the shared reference below.

## Optional AI routing — 2026-10-21

Reference: [ROCS canonical AI Gateway Policy](https://github.com/ronoc2020/revenue-factory/blob/main/docs/AI_GATEWAY_POLICY.md) and [Setup](https://github.com/ronoc2020/revenue-factory/blob/main/docs/AI_GATEWAY_SETUP.md). Check access to these references before relying on their contents.

- OmniRoute (https://github.com/diegosouzapw/OmniRoute) is an optional self-hosted **development** API gateway; reported token ceilings are estimates across independently eligible third-party free accounts, not guaranteed tokens or ChatGPT/Claude subscription boosts.
- FreeLLMAPI (https://github.com/tashfeenahmed/freellmapi) explicitly limits its intended use to personal experimentation; not approved for customer-facing/commercial production.
- Do **not** modify currently deployed model providers, credentials, deployments or pipelines automatically. Keep the gateway disabled unless an operator explicitly configures, verifies and approves it.
- No secrets, customer information, private telemetry, payment records, or vulnerability findings to unapproved third-party models; use public/synthetic data only for free-tier experiments.
- Never embed gateway API keys in browser JS, static assets, mobile bundles or git. Keep endpoints local or behind authenticated private access. Never assume a Docker/Node gateway runs in a Cloudflare Worker.
- Verify actual provider terms, quotas, latency, JSON/tool compatibility, timeout, 429 behavior, privacy, and reversible rollback before any opt-in change.
- Do not claim the gateway is installed or production-integrated merely because these instructions exist.

Project-to-agent routing guide: [docs/AI_AGENT_PROJECT_MATRIX.md](docs/AI_AGENT_PROJECT_MATRIX.md).
