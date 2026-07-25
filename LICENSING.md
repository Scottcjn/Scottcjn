# Elyan Labs Licensing Policy

One page, so you never have to guess. Three tiers, chosen so that building *on* the ecosystem is frictionless while the network itself stays open forever.

## The tiers

| Tier | License | Why |
| --- | --- | --- |
| **Libraries, SDKs, crates, MCP servers, agent skills** | MIT | Zero friction for commercial adopters. Embed them in anything, closed or open. |
| **RustChain core (node, consensus)** | Apache-2.0 | Permissive plus an explicit patent grant — the right base for consensus infrastructure. |
| **Platforms, inference engines, network tools** | AGPL-3.0 | If you run our stuff as a service, your improvements come back to the community. |

## Where each repo sits

**MIT (adopt freely):**
[clawrtc-rs](https://github.com/Scottcjn/clawrtc-rs) · [beacon-skill](https://github.com/Scottcjn/beacon-skill) · [beacon-skill-rs](https://github.com/Scottcjn/beacon-skill-rs) · [grazer-skill](https://github.com/Scottcjn/grazer-skill) · [grazer-skill-rs](https://github.com/Scottcjn/grazer-skill-rs) · [rustchain-mcp](https://github.com/Scottcjn/rustchain-mcp) · [grazer-mcp](https://github.com/Scottcjn/grazer-mcp) · [iota-agent-mcp](https://github.com/Scottcjn/iota-agent-mcp) · [bounty-concierge](https://github.com/Scottcjn/bounty-concierge) · [bottube](https://github.com/Scottcjn/bottube) · [legend-of-elya-n64](https://github.com/Scottcjn/legend-of-elya-n64)

**Apache-2.0 (patent-safe core):**
[Rustchain](https://github.com/Scottcjn/Rustchain)

**AGPL-3.0 (copyleft, network-aware):**
[ram-coffers](https://github.com/Scottcjn/ram-coffers) · [rpi-inference](https://github.com/Scottcjn/rpi-inference) · [can-it-run-ai](https://github.com/Scottcjn/can-it-run-ai) · [rustchain-monitor](https://github.com/Scottcjn/rustchain-monitor)

Repos not listed follow the license in their own `LICENSE` file; when in doubt, that file is authoritative.

## Practical answers

- **Can I build a commercial product on the crates/SDKs/MCP servers?** Yes. MIT, no strings.
- **Can I run my own RustChain node commercially?** Yes. Apache-2.0 includes a patent grant.
- **Can I fork the AGPL tools into a hosted service?** Yes, if your modifications are published under AGPL too. That's the deal.
- **Who holds copyright?** Scott Boudreaux / Elyan Labs LLC unless a file says otherwise. Contributions are accepted under each repo's license with DCO sign-off.

Questions about licensing for a specific use case: open an issue on the repo in question, or see [CONSULTING](https://github.com/Scottcjn/Rustchain/blob/main/CONSULTING.md).
