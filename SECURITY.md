# Security

This repository is public by design and must contain only update metadata and
encrypted release assets.

Do not commit private keys, API tokens, source code, customer information, or
machine telemetry. The private Capgo V2 key belongs in the private app workspace
and a secure backup only.

Report a suspected release-channel compromise privately to La Macchini. Until
review is complete, set `enabled` to `false` in `stable.json` and do not publish
new assets.
