# Edge-Gesture · 离线视觉手势交互

如何把自然手势稳定转换成一次明确的操作意图？

XIAO ESP32-S3 Sense 本地采集、识别和稳定化，经 ESP-NOW 向桌面终端发送离散事件。日常运行不依赖 PC 推理或互联网。

状态：2026-10-13，设计起始库。尚未实现新固件、训练模型或开展硬件验收。

## 从这里开始

1. [执行入口](CODEX_START.md)：下一步任务。
2. [设计与边界](docs/design.md)：把构想分解为模块。
3. [实施路线](docs/roadmap.md)：阶段与完成条件。
4. [硬件和历史基线](hardware/baseline.md)。
5. [学习路径](learning/README.md)。
6. [首个实验](experiments/P01.md)与[记录模板](experiments/template.md)。
7. [来源与取舍](references/origin.md)。

## 独特性

不实现桌面 HID、不维护 CSI 算法、不控制电机；暂不做连续空中鼠标和动态轨迹手势。

本库保存设计、学习过程和后续实现；不通过复制整套历史文件伪造完整工程。实验完成后才更新状态。
