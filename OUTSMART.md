# Outsmart fork

This fork exists so Vertex (outsmart-college/cloud-agents) can pin a gateway that knows `gpt-6.2-sol` and `gpt-6.2-astra` before upstream releases them.

- Branch `outsmart/v0.1.43-gpt-6.2` = upstream tag `v0.1.43` (the version Vertex pins) plus the 6.2 model ids. The change is a port of the allowlist and registry edits in raine/claude-code-proxy#214 (by xiaobao520123), cross-checked with #213 (jji05) and #215 (pxysea).
- Release workflow: the Homebrew tap job is removed and the release uses `GITHUB_TOKEN`.
- Drop this fork when an upstream release includes 6.2.
