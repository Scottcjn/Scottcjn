<div align="center">

# Elyan Labs

Scott / AutoJanitor builds open systems where vintage silicon still matters.

**Main bets:** a blockchain that rewards old hardware, a video platform for AI agents, and retro ports that make modern tooling run on machines nobody expects.

[Website](https://rustchain.org) • [BoTTube](https://bottube.ai) • [RustChain](https://github.com/Scottcjn/Rustchain) • [Beacon Skill](https://github.com/Scottcjn/beacon-skill)

![GitHub followers](https://img.shields.io/github/followers/Scottcjn?style=flat-square&label=followers)
![RustChain stars](https://img.shields.io/github/stars/Scottcjn/Rustchain?style=flat-square&label=RustChain)
![BoTTube stars](https://img.shields.io/github/stars/Scottcjn/bottube?style=flat-square&label=BoTTube)
![Beacon stars](https://img.shields.io/github/stars/Scottcjn/beacon-skill?style=flat-square&label=Beacon)

</div>

## Start Here

| Project | What it is | Why it matters |
| --- | --- | --- |
| [RustChain](https://github.com/Scottcjn/Rustchain) | Proof-of-Antiquity blockchain | Real miners, nodes, explorer, payouts, and a model where older hardware can outperform newer machines |
| [BoTTube](https://github.com/Scottcjn/bottube) | AI-native video platform | Agents and humans upload, watch, comment, tip, and build an actual content graph |
| [beacon-skill](https://github.com/Scottcjn/beacon-skill) | Agent coordination toolkit | Presence, inbox, relay, trust, and cross-platform agent plumbing |
| [rustchain-bounties](https://github.com/Scottcjn/rustchain-bounties) | Public bounty board | Open work tied to RTC rewards, contributor onboarding, and ecosystem growth |
| [legend-of-elya-n64](https://github.com/Scottcjn/legend-of-elya-n64) | N64 homebrew with on-device transformer inference | A good summary of this account: modern ideas, strange hardware, real implementation |

## Why This Account Exists

- Ship live systems instead of pitch decks
- Make old hardware economically useful again
- Build public infrastructure for agents, creators, and weird machines
- Document ports and experiments for POWER8, PowerPC, SPARC, N64, and other neglected platforms

## Cryptographic & Security Contributions

Merged security patches in libraries used by millions of systems worldwide:

| Library | PR | Fix | Status |
| --- | --- | --- | --- |
| **OpenSSL** | [#30437](https://github.com/openssl/openssl/pull/30437) | Integer truncation in PowerPC AES-GCM (`int` → `size_t`) | **Merged to master + 5 release branches** |
| **OpenSSL** | [#30452](https://github.com/openssl/openssl/pull/30452) | Silent decrypt error swallow in PPC GCM path | In review |
| **wolfSSL** | [#9932](https://github.com/wolfSSL/wolfssl/pull/9932) | POWER8 hardware AES via `vcipher`/`vcipherlast` (13-20x faster) | In review (CLA signed) |
| **NSA Ghidra** | [#9036](https://github.com/NationalSecurityAgency/ghidra/pull/9036) | e200 VLE PowerPC language support for reverse engineering | In review |
| **libdeflate** | [#448](https://github.com/ebiggers/libdeflate/pull/448) | Enable UNALIGNED_ACCESS_IS_FAST for all PowerPC variants | **Merged** |
| **vLLM** | [#35674](https://github.com/vllm-project/vllm/pull/35674) | IBM POWER8 (ppc64le) CPU backend support | In review |
| **Anthropic SDK** | [#1247](https://github.com/anthropics/anthropic-sdk-python/pull/1247) | Skip no-op recursive transform for types without PropertyInfo | In review |

Also: [US Patent 10,579,974](https://patents.google.com/patent/US10579974) — rapid transaction settlements in distributed digital asset networks.

## Merged Upstream Work

Recent accepted external contributions:

- **[openssl/openssl](https://github.com/openssl/openssl)**: merged PowerPC AES-GCM integer truncation fix to all supported branches ([#30437](https://github.com/openssl/openssl/pull/30437))
- **[ebiggers/libdeflate](https://github.com/ebiggers/libdeflate)**: merged PowerPC unaligned access optimization ([#448](https://github.com/ebiggers/libdeflate/pull/448))
- **[ahmet/awesome-web3](https://github.com/ahmet/awesome-web3)**: merged RustChain listing ([#626](https://github.com/ahmet/awesome-web3/pull/626))
- [up-for-grabs/up-for-grabs.net](https://github.com/up-for-grabs/up-for-grabs.net): merged RustChain ecosystem listing ([#5592](https://github.com/up-for-grabs/up-for-grabs.net/pull/5592))
- [learnhouse/learnhouse](https://github.com/learnhouse/learnhouse): merged accessibility fix ([#669](https://github.com/learnhouse/learnhouse/pull/669))
- [trajectly/trajectly](https://github.com/trajectly/trajectly): merged CLI and report test coverage ([#54](https://github.com/trajectly/trajectly/pull/54), [#55](https://github.com/trajectly/trajectly/pull/55), and 8 more)
- MCP registries: merged into [TensorBlock](https://github.com/TensorBlock/awesome-mcp-servers/pull/154), [AlexMili](https://github.com/AlexMili/Awesome-MCP/pull/36), [toolsdk-ai](https://github.com/toolsdk-ai/toolsdk-mcp-registry/pull/191)
- Full list: [external-pr-portfolio.md](./external-pr-portfolio.md)

## Featured Weirdness

- [rust-ppc-tiger](https://github.com/Scottcjn/rust-ppc-tiger) - Rust-to-PowerPC transpiler for Mac OS X Tiger
- [llama-cpp-power8](https://github.com/Scottcjn/llama-cpp-power8) - POWER8 PSE vec_perm collapse for llama.cpp (8.8x speedup)
- [ram-coffers](https://github.com/Scottcjn/ram-coffers) - NUMA-aware weight banking for LLM inference
- [claude-code-power8](https://github.com/Scottcjn/claude-code-power8) - Claude Code CLI ported to IBM POWER8 / ppc64le
- [legend-of-elya-n64](https://github.com/Scottcjn/legend-of-elya-n64) - N64 game with 819K-parameter transformer on MIPS III
- [oculink-gpu-bypass](https://github.com/Scottcjn/oculink-gpu-bypass) - GPU bypass work for POWER systems and PowerPC Macs

## Current Focus

- RustChain network quality, miner onboarding, and payout integrity
- BoTTube distribution, embeds, notifications, and SDKs
- Beacon and agent-economy primitives that connect the stack
- Cryptographic contributions to OpenSSL, wolfSSL, and other foundational libraries
- Retro-compatible tools that would normally never get ports
