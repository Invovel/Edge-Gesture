# Edge-Gesture · 离线视觉手势交互

中文 | [English](README.en.md)

如何把自然手势稳定转换成一次明确的操作意图？

XIAO ESP32-S3 Sense 本地采集、识别和稳定化，经 ESP-NOW 输出离散手势事件。日常运行不依赖 PC 推理或互联网；先用接收测试工具独立验收。

状态：2026-10-13，设计起始库。尚未实现新固件、训练模型或开展硬件验收。

## 从这里开始

1. [执行入口](CODEX_START.md)。
2. [设计与边界](docs/design.md)。
3. [实施路线](docs/roadmap.md)。
4. [硬件与基线](hardware/baseline.md)。
5. [学习路径](learning/README.md)。
6. [首个实验](experiments/P01.md)与[记录模板](experiments/template.md)。
7. [设计来源与资料管理](references/origin.md)。

## 独特目标与范围

首版只识别静态手势并输出事件；连续空中鼠标、动态轨迹手势和应用端动作执行不在本库范围。

本库可独立推进，包含自身的设计、学习路径与实验计划。通过测量积累实现证据，未做过的实验不写成成果。
