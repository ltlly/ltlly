<div align="center">

# 洛天琉璃依 / ltlly

**逆向工程 · 二进制分析 · Android 运行时研究**

致力于连接静态分析与运行时真实行为的逆向工具。

[![Rust](https://img.shields.io/badge/Rust-111111?style=flat-square&logo=rust)](https://www.rust-lang.org/)
[![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org/)
[![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white)](https://isocpp.org/)
[![Android](https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=111111)](https://www.android.com/)
[![Frida](https://img.shields.io/badge/Frida-20232A?style=flat-square)](https://frida.re/)
[![Binary Ninja](https://img.shields.io/badge/Binary_Ninja-E84A5F?style=flat-square)](https://binary.ninja/)

</div>

## 关于我

逆向工程与二进制分析工具开发者，关注 Android ARM64、动态插桩、控制流去混淆、
中间表示变换，以及面向 AI coding agents 的无头分析接口。

目前的工作主要位于静态分析与动态分析的交界处：恢复程序控制流、保留可验证的语义证据，
并通过可复现的命令行工作流输出逆向分析结果。

## 代表项目

| 项目 | 简介 |
| --- | --- |
| [MikuTrace](https://github.com/ltlly/MikuTrace) | Android ARM64 指令级追踪工具链，包含 Frida Stalker 采集、Rust 分析核心、Web UI、污点分析、内存来源追踪与 AI 友好查询接口。 |
| [MikuCffHelper](https://github.com/ltlly/MikuCffHelper) | 基于 Binary Ninja LLIL/MLIL/HLIL 的 OLLVM 控制流平坦化恢复工作流，并提供多层语义等价性验证。 |
| [bn-cli](https://github.com/ltlly/bn-cli) | 面向 coding agents 的无头 Binary Ninja CLI，支持守护进程、多目标分析、紧凑输出和广泛的分析命令。 |
| [ida-rs-cli](https://github.com/ltlly/ida-rs-cli) | Rust 实现的无头 IDA Pro CLI，支持守护进程 IPC、多目标分析和上下文友好的输出。 |
| [miku-shield](https://github.com/ltlly/miku-shield) | 基于 eBPF 的 Android 观测工具，用于研究 anti-Frida 检测行为及缓解策略。 |
| [il2cpp_bn](https://github.com/VNRev/il2cpp_bn) | Binary Ninja IL2CPP 元数据导入插件，用于从大型 Unity 目标中高效恢复符号。 |

## 研究方向

- **运行时真相**：Frida Stalker、寄存器与内存轨迹、数据来源追踪
- **静态恢复**：CFG 重建、OLLVM CFF、间接跳转解析
- **分析平台**：Binary Ninja、IDA Pro、Ghidra
- **系统观测**：Android 内核、eBPF、ftrace、kprobes
- **Agent 接口**：稳定的 CLI/JSON 契约、无头分析、紧凑输出

## 工程原则

- 优先相信真实轨迹提供的证据，而不是对运行时行为的假设。
- 将去混淆视为语义保持问题，而不只是生成更好看的伪代码。
- 在增加新的集成层之前，先建立可重复执行的命令行工作流。
- 发布功能的同时，也公开失败模式、兼容性边界和基准数据。

## 其他链接

- 博客：[cnblogs.com/FW-ltlly](https://www.cnblogs.com/FW-ltlly/)
- 组织：[VNRev](https://github.com/VNRev)

<div align="center">

清风明月不渡我，人间荒唐多消磨。

</div>
