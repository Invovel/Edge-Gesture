# Edge-Gesture · Offline Visual Gesture Interaction

[中文](README.md) | English

How can natural gestures become stable, single-shot operation intents?

Capture, classify and stabilize gestures locally on a XIAO ESP32-S3 Sense, then emit discrete events over ESP-NOW. Normal operation requires neither PC inference nor Internet access. Validate independently with a receiver test tool first.

Status: October 13, 2026 — a design starting point. No new firmware, model training or hardware acceptance has been completed.

## Start here

1. [Next task](CODEX_START.en.md).
2. [Design and scope](docs/design.en.md).
3. [Implementation roadmap](docs/roadmap.en.md).
4. [Hardware and baseline](hardware/baseline.en.md).
5. [Learning path](learning/README.en.md).
6. [First experiment](experiments/P01.en.md) and [record template](experiments/template.en.md).
7. [Design origin and reference management](references/origin.en.md).

## Distinct goal and scope

The first version classifies static gestures and emits events. Continuous air-mouse control, dynamic trajectories and application-side actions are outside this repository.

This repository stands on its own, with its own design, learning path and experiments. Build evidence through measurements; do not present unperformed experiments as results.
