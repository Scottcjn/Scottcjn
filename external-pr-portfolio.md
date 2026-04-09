# External PR Portfolio

Confirmed external PRs authored by `Scottcjn` and merged upstream. **44+ merged PRs as of 2026-04-09.**

## Merged Upstream Work

Recent accepted upstream contributions across external repositories:

### Major Libraries (Security, Crypto, Compression)
- `openssl/openssl`: 2 PRs merged — PowerPC AES-GCM integer truncation fix and decrypt error return fix, both in master + 5 release branches (3.3, 3.4, 3.5, 3.6, 4.0)
- `hacl-star/hacl-star`: AltiVec `bool` keyword conflict fix on PowerPC (GCC) — Microsoft's formal-verified cryptography library
- `ebiggers/libdeflate`: PowerPC unaligned access optimization
- `Blosc/c-blosc2`: 2 PRs merged — PowerPC VSX shuffle detection for ppc64 big-endian, and missing `pa_` variable in sw32 bswap fallback — compression library behind pandas, zarr, PyTables

### Developer Tools, SDKs, Game Development
- `DragonMinded/libdragon`: macOS build fix in newlib configure — the primary Nintendo 64 homebrew SDK
- `capstone-engine/capstone`: Mac OS X 10.5 portability fix (avoid `strnlen()` in `cs_strndup`) — multi-architecture disassembly framework (8K stars, used by IDA Pro, radare2, Ghidra)
- `Joshkaki00/godotmark`: Temperature reading edge case fix — Godot engine benchmark
- `danifunker/rusty-backup`: Real PowerPC Tiger port for G3/G4/G5 Macs running Mac OS X 10.4

### Security Tooling and Test Coverage
- `kusari-oss/darnit`: 6 PRs merged — supply-chain security tool contributions (exception handling, MCP server dev workflow, plugin protocol tests, gh CLI error messaging, issue templates, handler authoring guide)
- `trajectly/trajectly`: 12 focused Python test coverage improvements for CLI report rendering, regression output paths, and integration flows
- `learnhouse/learnhouse`: 2 accessibility fixes — decorative SVG hiding, and aria-label for placeholder-only inputs
- `beumerr/tailwind-stash`: Semantic status role for EmptyState component

### Ecosystem and Awesome Lists
- `xlite-dev/Awesome-LLM-Inference`: POWER8 inference + NUMA weight banking + Grail-V listing (2 PRs)
- `command-tab/awesome-n64-development`: Legend of Elya N64 neural network listing
- `ellisonleao/magictools`: Legend of Elya game development listing
- `gauravfs-14/awesome-tinyml`: Legend of Elya MIPS R4300i listing
- `transpiler/awesome-transpiler`: rust-ppc-tiger listing
- `ahmet/awesome-web3`: RustChain listing
- `nibzard/awesome-agentic-patterns`: economic-value-signaling pattern
- `jnv/lists`: awesome-agent-bounties listing
- `Piyushhbhutoria/awesome-hacktoberfest-2026`: Elyan Labs project listing
- `up-for-grabs/up-for-grabs.net`: RustChain ecosystem listing (4 repos)
- `firstcontributions/first-contributions`: contributor listing
- `TensorBlock/awesome-mcp-servers`, `AlexMili/Awesome-MCP`, `toolsdk-ai/toolsdk-mcp-registry`: RustChain MCP registry additions across multiple external MCP index repos

This section is suitable for a GitHub profile README, personal site, or funding/partnership outreach.

## 2026-04

| Merged | Repository | PR | Title |
|---|---|---|---|
| 2026-04-08 | `capstone-engine/capstone` | [#2889](https://github.com/capstone-engine/capstone/pull/2889) | fix: avoid strnlen() in cs_strndup for Mac OS X 10.5 portability |
| 2026-04-06 | `DragonMinded/libdragon` | [#849](https://github.com/DragonMinded/libdragon/pull/849) | fix: set CC_FOR_TARGET in newlib configure to fix macOS build |
| 2026-04-04 | `kusari-oss/darnit` | [#128](https://github.com/kusari-oss/darnit/pull/128) | docs: add handler authoring guide |
| 2026-04-04 | `kusari-oss/darnit` | [#127](https://github.com/kusari-oss/darnit/pull/127) | infra: add GitHub issue templates |
| 2026-04-04 | `kusari-oss/darnit` | [#126](https://github.com/kusari-oss/darnit/pull/126) | fix: show actionable error when gh CLI is missing |
| 2026-04-04 | `kusari-oss/darnit` | [#123](https://github.com/kusari-oss/darnit/pull/123) | test: add plugin protocol unit coverage |
| 2026-04-02 | `gauravfs-14/awesome-tinyml` | [#1](https://github.com/gauravfs-14/awesome-tinyml/pull/1) | Add Legend of Elya -- LLM inference on Nintendo 64 (MIPS R4300i) |

## 2026-03

| Merged | Repository | PR | Title |
|---|---|---|---|
| 2026-03-31 | `kusari-oss/darnit` | [#125](https://github.com/kusari-oss/darnit/pull/125) | docs: add MCP server development workflow to CONTRIBUTING |
| 2026-03-27 | `Blosc/c-blosc2` | [#725](https://github.com/Blosc/c-blosc2/pull/725) | fix: add missing pa_ variable in sw32_ bswap fallback |
| 2026-03-26 | `ellisonleao/magictools` | [#359](https://github.com/ellisonleao/magictools/pull/359) | Add Legend of Elya to Complete Game Sources |
| 2026-03-24 | `Blosc/c-blosc2` | [#723](https://github.com/Blosc/c-blosc2/pull/723) | fix: enable VSX shuffle on ppc64 big-endian with proper detection |
| 2026-03-23 | `hacl-star/hacl-star` | [#1068](https://github.com/hacl-star/hacl-star/pull/1068) | Fix AltiVec bool keyword conflict on PowerPC (GCC) |
| 2026-03-23 | `learnhouse/learnhouse` | [#672](https://github.com/learnhouse/learnhouse/pull/672) | fix: add aria-label to inputs that only have placeholder text |
| 2026-03-23 | `kusari-oss/darnit` | [#121](https://github.com/kusari-oss/darnit/pull/121) | Narrow remediation executor exception handling |
| 2026-03-21 | `jnv/lists` | [#251](https://github.com/jnv/lists/pull/251) | Add awesome-agent-bounties |
| 2026-03-20 | `beumerr/tailwind-stash` | [#43](https://github.com/beumerr/tailwind-stash/pull/43) | Add semantic status role to EmptyState |
| 2026-03-18 | `transpiler/awesome-transpiler` | [#8](https://github.com/transpiler/awesome-transpiler/pull/8) | Add rust-ppc-tiger -- Rust to PowerPC assembly transpiler |
| 2026-03-18 | `xlite-dev/Awesome-LLM-Inference` | [#161](https://github.com/xlite-dev/Awesome-LLM-Inference/pull/161) | Add POWER8 LLM inference and NUMA weight banking projects |
| 2026-03-16 | `ebiggers/libdeflate` | [#448](https://github.com/ebiggers/libdeflate/pull/448) | Enable UNALIGNED_ACCESS_IS_FAST for all PowerPC variants |
| 2026-03-16 | `ahmet/awesome-web3` | [#626](https://github.com/ahmet/awesome-web3/pull/626) | Add RustChain to Protocol section |
| 2026-03-15 | `up-for-grabs/up-for-grabs.net` | [#5592](https://github.com/up-for-grabs/up-for-grabs.net/pull/5592) | Add RustChain ecosystem projects (4 repos) |
| 2026-03-15 | `learnhouse/learnhouse` | [#669](https://github.com/learnhouse/learnhouse/pull/669) | Hide decorative SVGs and carets from assistive tech |
| 2026-03-14 | `trajectly/trajectly` | [#60](https://github.com/trajectly/trajectly/pull/60)--[#69](https://github.com/trajectly/trajectly/pull/69) | 10 PRs: CLI integration test coverage (report rendering, regression, baseline, repro) |
| 2026-03-13 | `Joshkaki00/godotmark` | [#13](https://github.com/Joshkaki00/godotmark/pull/13) | Handle unavailable temperature readings without showing 0 C |
| 2026-03-12 | `trajectly/trajectly` | [#55](https://github.com/trajectly/trajectly/pull/55) | Add markdown renderer branch tests |
| 2026-03-12 | `trajectly/trajectly` | [#54](https://github.com/trajectly/trajectly/pull/54) | Add PR comment renderer fallback tests |
| 2026-03-11 | `Piyushhbhutoria/awesome-hacktoberfest-2026` | [#21](https://github.com/Piyushhbhutoria/awesome-hacktoberfest-2026/pull/21) | Add Elyan Labs open source projects |
| 2026-03-11 | `danifunker/rusty-backup` | [#13](https://github.com/danifunker/rusty-backup/pull/13) | Add PowerPC Tiger port (Mac OS X 10.4) |
| 2026-03-10 | `TensorBlock/awesome-mcp-servers` | [#154](https://github.com/TensorBlock/awesome-mcp-servers/pull/154) | Add RustChain MCP to Finance & Crypto |
| 2026-03-09 | `AlexMili/Awesome-MCP` | [#36](https://github.com/AlexMili/Awesome-MCP/pull/36) | Add RustChain MCP server (Python, blockchain + video) |
| 2026-03-09 | `toolsdk-ai/toolsdk-mcp-registry` | [#191](https://github.com/toolsdk-ai/toolsdk-mcp-registry/pull/191) | Add RustChain MCP server to Finance & Fintech |
| 2026-03-06 | `firstcontributions/first-contributions` | [#113035](https://github.com/firstcontributions/first-contributions/pull/113035) | Add Scott Boudreaux (Elyan Labs) |
| 2026-03-01 | `nibzard/awesome-agentic-patterns` | [#25](https://github.com/nibzard/awesome-agentic-patterns/pull/25) | Add: economic-value-signaling-multi-agent |

## 2026-02

| Merged | Repository | PR | Title |
|---|---|---|---|
| 2026-02-27 | `command-tab/awesome-n64-development` | [#63](https://github.com/command-tab/awesome-n64-development/pull/63) | Add Legend of Elya - nano-GPT neural network on N64 |
| 2026-02-27 | `xlite-dev/Awesome-LLM-Inference` | [#159](https://github.com/xlite-dev/Awesome-LLM-Inference/pull/159) | Add Grail-V: Non-bijunctive attention on POWER8 (8.8x speedup) |

## Pending Review (High-Value Targets)

| Repository | PR | Title | Stars |
|---|---|---|---|
| `python/cpython` | [#146118](https://github.com/python/cpython/pull/146118) | BLAKE2 SIMD128 on POWER8 via VSX | 65K |
| `NationalSecurityAgency/ghidra` | [#9036](https://github.com/NationalSecurityAgency/ghidra/pull/9036) | e200 VLE PowerPC language support | 53K |
| `curl/curl` | [#20984](https://github.com/curl/curl/pull/20984) | SHA-512/256 big-endian optimization | 36K |
| `vllm-project/vllm` | [#35674](https://github.com/vllm-project/vllm/pull/35674) | POWER8 CPU backend | 30K |
| `wolfSSL/wolfssl` | [#9932](https://github.com/wolfSSL/wolfssl/pull/9932) | POWER8 hardware AES (13-20x faster) | 2K |

## Notes

- Scope here is external upstream merges only, not PRs merged in repositories owned by `Scottcjn`.
- Source of truth is GitHub search plus direct PR checks.
- Update this file whenever a new external PR merges.
