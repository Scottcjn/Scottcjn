<div align="center">

# Elyan Labs

Scott / AutoJanitor builds open systems where vintage silicon still matters.

**Main bets:** a blockchain that rewards old hardware, a video platform for AI agents, and retro ports that make modern tooling run on machines nobody expects. **16+ machines preserved from e-waste.** Code merged into OpenSSL. Paper accepted at **CVPR 2026**.

[Website](https://rustchain.org) | [BoTTube](https://bottube.ai) | [RustChain](https://github.com/Scottcjn/Rustchain) | [Beacon Skill](https://github.com/Scottcjn/beacon-skill)

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
| [trashclaw](https://github.com/Scottcjn/trashclaw) | Zero-dep local LLM agent | Born from a rejected llama.cpp PR. 14 tools, plugin system, runs on anything |
| [legend-of-elya-n64](https://github.com/Scottcjn/legend-of-elya-n64) | N64 homebrew with on-device transformer inference | A good summary of this account: modern ideas, strange hardware, real implementation |

## Why This Account Exists

- Ship live systems instead of pitch decks
- Make old hardware economically useful again — [16+ machines preserved from e-waste](https://rustchain.org/preserved.html)
- Build public infrastructure for agents, creators, and weird machines
- Document ports and experiments for POWER8, PowerPC, SPARC, N64, and other neglected platforms
- Prove that the greenest computation is the one that already exists

## Cryptographic and Security Contributions

Security patches and performance work in libraries used by millions of systems worldwide:

| Library | PR | Fix | Status |
| --- | --- | --- | --- |
| **OpenSSL** | [#30437](https://github.com/openssl/openssl/pull/30437) | Integer truncation in PowerPC AES-GCM (`int` to `size_t`) | **Merged to master + 5 release branches** |
| **OpenSSL** | [#30452](https://github.com/openssl/openssl/pull/30452) | Incorrect error return in AES-GCM decrypt path | **Merged to master + 5 release branches** |
| **hacl-star** | [#1068](https://github.com/hacl-star/hacl-star/pull/1068) | Fix AltiVec `bool` keyword conflict on PowerPC (GCC) — Microsoft formal-verified crypto library | **Merged** |
| **libdeflate** | [#448](https://github.com/ebiggers/libdeflate/pull/448) | Enable UNALIGNED_ACCESS_IS_FAST for all PowerPC variants | **Merged** |
| **CPython** | [#146118](https://github.com/python/cpython/pull/146118) | BLAKE2 SIMD128 on POWER8 via VSX intrinsics | In review (65K-star repo) |
| **curl** | [#20984](https://github.com/curl/curl/pull/20984) | SHA-512/256 big-endian optimization | In review (36K-star repo) |
| **NSA Ghidra** | [#9036](https://github.com/NationalSecurityAgency/ghidra/pull/9036) | e200 VLE PowerPC language support for reverse engineering | In review (53K-star repo) |
| **vLLM** | [#35674](https://github.com/vllm-project/vllm/pull/35674) | IBM POWER8 (ppc64le) CPU backend support | In review (30K-star repo) |
| **wolfSSL** | [#9932](https://github.com/wolfSSL/wolfssl/pull/9932) | POWER8 hardware AES via `vcipher`/`vcipherlast` (13-20x faster) | In review (CLA signed) |

Also: [US Patent 10,579,974](https://patents.google.com/patent/US10579974) -- rapid transaction settlements in distributed digital asset networks.

## Portability and Performance Contributions

Merged work making widely-used libraries run correctly on vintage, big-endian, and non-x86 architectures:

| Library | PR | Fix | Project Scale |
| --- | --- | --- | --- |
| **libdragon** | [#849](https://github.com/DragonMinded/libdragon/pull/849) | Set `CC_FOR_TARGET` in newlib configure to fix macOS build — N64 homebrew SDK | **Merged** — the primary N64 SDK |
| **capstone** | [#2889](https://github.com/capstone-engine/capstone/pull/2889) | Avoid `strnlen()` in `cs_strndup` for Mac OS X 10.5 portability — multi-arch disassembly framework | **Merged** — 8K stars, used by IDA Pro, radare2, Ghidra |
| **c-blosc2** | [#723](https://github.com/Blosc/c-blosc2/pull/723) | Enable VSX shuffle on ppc64 big-endian with proper detection | **Merged** — the compression lib behind pandas/zarr/PyTables |
| **c-blosc2** | [#725](https://github.com/Blosc/c-blosc2/pull/725) | Add missing `pa_` variable in `sw32_` bswap fallback | **Merged** |
| **libdeflate** | [#448](https://github.com/ebiggers/libdeflate/pull/448) | Enable UNALIGNED_ACCESS_IS_FAST for all PowerPC variants | **Merged** — fast zlib replacement |
| **danifunker/rusty-backup** | [#13](https://github.com/danifunker/rusty-backup/pull/13) | PowerPC Tiger port for G3/G4/G5 Macs (Mac OS X 10.4) | **Merged** |

These contributions come from running modern tooling on PowerPC G3/G4/G5, POWER8, Mac OS X 10.5, and N64 hardware — platforms where the bugs are real and the fixes are load-bearing.

## Merged Upstream Work

**44+ PRs merged** into external repositories across security, portability, developer tools, and ecosystem registries.

### Major Libraries (Security, Crypto, Compression)
- **[openssl/openssl](https://github.com/openssl/openssl)**: 2 PRs merged — PowerPC AES-GCM integer truncation fix ([#30437](https://github.com/openssl/openssl/pull/30437)) and decrypt error return fix ([#30452](https://github.com/openssl/openssl/pull/30452)), both in master + branches 3.3-4.0
- **[hacl-star/hacl-star](https://github.com/hacl-star/hacl-star)**: AltiVec `bool` keyword conflict fix on PowerPC ([#1068](https://github.com/hacl-star/hacl-star/pull/1068)) — Microsoft's formal-verified cryptography library
- **[ebiggers/libdeflate](https://github.com/ebiggers/libdeflate)**: PowerPC unaligned access optimization ([#448](https://github.com/ebiggers/libdeflate/pull/448))
- **[Blosc/c-blosc2](https://github.com/Blosc/c-blosc2)**: 2 PRs merged — PowerPC VSX shuffle detection ([#723](https://github.com/Blosc/c-blosc2/pull/723)) + bswap fallback fix ([#725](https://github.com/Blosc/c-blosc2/pull/725)) — compression library behind pandas, zarr, PyTables

### Developer Tools, SDKs, and Game Development
- **[DragonMinded/libdragon](https://github.com/DragonMinded/libdragon)**: macOS build fix for newlib configure ([#849](https://github.com/DragonMinded/libdragon/pull/849)) — the primary Nintendo 64 homebrew SDK
- **[capstone-engine/capstone](https://github.com/capstone-engine/capstone)**: Mac OS X 10.5 portability fix ([#2889](https://github.com/capstone-engine/capstone/pull/2889)) — multi-architecture disassembly framework used by IDA Pro, radare2, Ghidra, 8K stars
- **[Joshkaki00/godotmark](https://github.com/Joshkaki00/godotmark)**: Temperature reading edge case fix ([#13](https://github.com/Joshkaki00/godotmark/pull/13)) — Godot engine benchmark tool
- **[danifunker/rusty-backup](https://github.com/danifunker/rusty-backup)**: PowerPC Tiger port for G3/G4/G5 Macs running Mac OS X 10.4 ([#13](https://github.com/danifunker/rusty-backup/pull/13))

### Security Tooling and Test Coverage
- **[kusari-oss/darnit](https://github.com/kusari-oss/darnit)**: 6 PRs merged — supply-chain security tool contributions including exception handling ([#121](https://github.com/kusari-oss/darnit/pull/121)), MCP server dev workflow docs ([#125](https://github.com/kusari-oss/darnit/pull/125)), plugin protocol unit tests ([#123](https://github.com/kusari-oss/darnit/pull/123)), gh CLI error messaging ([#126](https://github.com/kusari-oss/darnit/pull/126)), GitHub issue templates ([#127](https://github.com/kusari-oss/darnit/pull/127)), handler authoring guide ([#128](https://github.com/kusari-oss/darnit/pull/128))
- **[trajectly/trajectly](https://github.com/trajectly/trajectly)**: 12 merged PRs covering CLI test coverage ([#54](https://github.com/trajectly/trajectly/pull/54)-[#69](https://github.com/trajectly/trajectly/pull/69))
- **[learnhouse/learnhouse](https://github.com/learnhouse/learnhouse)**: 2 a11y fixes — decorative SVG hiding ([#669](https://github.com/learnhouse/learnhouse/pull/669)) + aria-label for placeholder-only inputs ([#672](https://github.com/learnhouse/learnhouse/pull/672))
- **[beumerr/tailwind-stash](https://github.com/beumerr/tailwind-stash)**: Semantic status role for EmptyState component ([#43](https://github.com/beumerr/tailwind-stash/pull/43))

### Ecosystem and Awesome Lists
- **[xlite-dev/Awesome-LLM-Inference](https://github.com/xlite-dev/Awesome-LLM-Inference)**: POWER8 inference + NUMA weight banking ([#161](https://github.com/xlite-dev/Awesome-LLM-Inference/pull/161)) + Grail-V non-bijunctive attention ([#159](https://github.com/xlite-dev/Awesome-LLM-Inference/pull/159)) — 5K-star repo
- **[command-tab/awesome-n64-development](https://github.com/command-tab/awesome-n64-development)**: Legend of Elya N64 neural network listing ([#63](https://github.com/command-tab/awesome-n64-development/pull/63))
- **[ellisonleao/magictools](https://github.com/ellisonleao/magictools)**: Legend of Elya game development listing ([#359](https://github.com/ellisonleao/magictools/pull/359))
- **[gauravfs-14/awesome-tinyml](https://github.com/gauravfs-14/awesome-tinyml)**: Legend of Elya on MIPS R4300i ([#1](https://github.com/gauravfs-14/awesome-tinyml/pull/1))
- **[transpiler/awesome-transpiler](https://github.com/transpiler/awesome-transpiler)**: rust-ppc-tiger listing ([#8](https://github.com/transpiler/awesome-transpiler/pull/8))
- **[ahmet/awesome-web3](https://github.com/ahmet/awesome-web3)**: RustChain listing ([#626](https://github.com/ahmet/awesome-web3/pull/626))
- **[nibzard/awesome-agentic-patterns](https://github.com/nibzard/awesome-agentic-patterns)**: economic-value-signaling pattern ([#25](https://github.com/nibzard/awesome-agentic-patterns/pull/25))
- **[jnv/lists](https://github.com/jnv/lists)**: awesome-agent-bounties listing ([#251](https://github.com/jnv/lists/pull/251))
- **[Piyushhbhutoria/awesome-hacktoberfest-2026](https://github.com/Piyushhbhutoria/awesome-hacktoberfest-2026)**: Elyan Labs project listing ([#21](https://github.com/Piyushhbhutoria/awesome-hacktoberfest-2026/pull/21))
- **[up-for-grabs/up-for-grabs.net](https://github.com/up-for-grabs/up-for-grabs.net)**: RustChain ecosystem listing, 4 repos ([#5592](https://github.com/up-for-grabs/up-for-grabs.net/pull/5592))
- **[firstcontributions/first-contributions](https://github.com/firstcontributions/first-contributions)**: Contributor listing ([#113035](https://github.com/firstcontributions/first-contributions/pull/113035))
- **MCP registries**: merged into [TensorBlock](https://github.com/TensorBlock/awesome-mcp-servers/pull/154), [AlexMili](https://github.com/AlexMili/Awesome-MCP/pull/36), [toolsdk-ai](https://github.com/toolsdk-ai/toolsdk-mcp-registry/pull/191)
- Full list with dates: [external-pr-portfolio.md](./external-pr-portfolio.md)

## Featured Weirdness

- [rust-ppc-tiger](https://github.com/Scottcjn/rust-ppc-tiger) - Rust-to-PowerPC transpiler for Mac OS X Tiger
- [llama-cpp-power8](https://github.com/Scottcjn/llama-cpp-power8) - POWER8 PSE vec_perm collapse for llama.cpp (8.8x speedup)
- [ram-coffers](https://github.com/Scottcjn/ram-coffers) - NUMA-aware weight banking for LLM inference
- [claude-code-power8](https://github.com/Scottcjn/claude-code-power8) - Claude Code CLI ported to IBM POWER8 / ppc64le
- [legend-of-elya-n64](https://github.com/Scottcjn/legend-of-elya-n64) - N64 game with 819K-parameter transformer on MIPS III
- [trashclaw](https://github.com/Scottcjn/trashclaw) - Zero-dep LLM agent with Boudreaux Rules, runs on Mac Pro trashcan
- [oculink-gpu-bypass](https://github.com/Scottcjn/oculink-gpu-bypass) - GPU bypass work for POWER systems and PowerPC Macs

## Current Focus

- RustChain network quality, miner onboarding, and payout integrity
- BoTTube distribution, embeds, notifications, and SDKs
- Beacon and agent-economy primitives that connect the stack
- Upstream security contributions to OpenSSL, wolfSSL, CPython, curl, and Ghidra (2 merged into OpenSSL)
- Retro-compatible tools that would normally never get ports
- [Machines Preserved](https://rustchain.org/preserved.html) — tracking the environmental impact of keeping hardware alive
