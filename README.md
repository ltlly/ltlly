<div align="center">

# 洛天琉璃依 / ltlly

**Reverse Engineering · Binary Analysis · Android Runtime Research**

I build tools that connect static analysis with runtime truth.

[![Rust](https://img.shields.io/badge/Rust-111111?style=flat-square&logo=rust)](https://www.rust-lang.org/)
[![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org/)
[![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white)](https://isocpp.org/)
[![Android](https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=111111)](https://www.android.com/)
[![Frida](https://img.shields.io/badge/Frida-20232A?style=flat-square)](https://frida.re/)
[![Binary Ninja](https://img.shields.io/badge/Binary_Ninja-E84A5F?style=flat-square)](https://binary.ninja/)

</div>

## About

逆向工程与二进制分析工具开发者，关注 Android ARM64、动态插桩、控制流去混淆、
中间表示变换，以及面向 AI coding agents 的无头分析接口。

Most of my current work sits at the boundary between static and dynamic analysis:
recovering control flow, preserving semantic evidence, and making reverse-engineering
results available through reproducible command-line workflows.

## Selected Work

| Project | What it does |
| --- | --- |
| [MikuTrace](https://github.com/ltlly/MikuTrace) | Android ARM64 instruction-level tracing with Frida Stalker, a Rust analysis core, Web UI, taint/memory provenance, and agent-friendly queries. |
| [MikuCffHelper](https://github.com/ltlly/MikuCffHelper) | Binary Ninja workflow for recovering OLLVM control-flow flattening at LLIL/MLIL/HLIL layers with semantic verification. |
| [bn-cli](https://github.com/ltlly/bn-cli) | Headless Binary Ninja CLI designed for coding agents, daemon workflows, compact output, and broad analysis coverage. |
| [ida-rs-cli](https://github.com/ltlly/ida-rs-cli) | Rust-based headless IDA Pro CLI with daemon IPC, multi-target analysis, and context-aware output for agents. |
| [miku-shield](https://github.com/ltlly/miku-shield) | eBPF-based Android observer for studying anti-Frida behavior and mitigation strategies. |
| [ghidra_rust](https://github.com/ltlly/ghidra_rust) | Experimental Rust work around Ghidra-compatible decompilation, analysis, emulation, and headless services. |
| [il2cpp_bn](https://github.com/VNRev/il2cpp_bn) | Binary Ninja plugin for importing IL2CPP metadata and efficiently recovering symbols from large Unity targets. |

## Research Threads

```text
Runtime truth       Frida Stalker · register/memory traces · provenance
Static recovery     CFG reconstruction · OLLVM CFF · indirect branches
Analysis platforms  Binary Ninja · IDA Pro · Ghidra
System visibility   Android kernel · eBPF · ftrace · kprobes
Agent interfaces    stable CLI/JSON contracts · headless analysis · compact output
```

## Engineering Principles

- Prefer evidence from real traces over assumptions about runtime behavior.
- Treat deobfuscation as a semantics-preservation problem, not just prettier pseudocode.
- Build repeatable CLI workflows before adding another integration layer.
- Publish failure modes, compatibility limits, and benchmarks alongside features.

## Elsewhere

- Blog: [cnblogs.com/FW-ltlly](https://www.cnblogs.com/FW-ltlly/)
- Organization: [VNRev](https://github.com/VNRev)

<div align="center">

清风明月不渡我，人间荒唐多消磨。

</div>
