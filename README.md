# PaperBanana Built-in Figures

一个用于 Codex 的科研配图 skill：借鉴 PaperBanana 的检索、规划、风格设计、绘制和评审思路，使用当前环境提供的 GPT 内置生图工具制作示意图；实验统计图使用真实数据和本地代码精确绘制。

This is an independent, PaperBanana-inspired workflow, not the PaperBanana runtime or an official integration. It does not require the PaperBanana package or an API key. Built-in image generation must be available in the active Codex environment; installation does not supply the tool or guarantee access. If unavailable, the skill does not silently fall back to an API.

## 安装 / Install

在 Codex 中直接说：

> 使用 skill-installer 安装 https://github.com/YanYihann/paperbanana-builtin-figures/tree/main/skills/paperbanana-builtin-figures

或者使用本机自带的 skill-installer 脚本：

```bash
python ~/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py --repo YanYihann/paperbanana-builtin-figures --path skills/paperbanana-builtin-figures
```

安装后在下一轮对话使用。如果同名 skill 已存在，安装器会停止以防覆盖；先检查现有文件，再决定如何更新。

## 使用 / Use

在 Codex 中输入：

> 使用 $paperbanana-builtin-figures，阅读我的论文方法和图注，用 PaperBanana 的流程规划一张模型架构图，并使用内置生图制作；核对组件、箭头和文字，保存最终图片与提示词。

也可以提供整篇论文、参考图、目标期刊、数据及原始照片，请求一组配图。对涉及真实实验值的面板，skill 会使用数据绘图；不能把生成图当作实际数据或真实样本。需要可编辑矢量文件时，请明确提出；生成位图嵌入 PDF 并不等于矢量化。

## Attribution

Inspired by [PaperBanana](https://github.com/dwzhu-pku/PaperBanana). This repository contains original workflow instructions and does not bundle its code or models. PaperBanana is a separate project with its own license.

## License

MIT; see [LICENSE](LICENSE).

