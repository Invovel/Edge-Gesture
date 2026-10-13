# Design and modules

[中文](design.md) | English

## Goal

Capture, classify and stabilize gestures locally on a XIAO ESP32-S3 Sense, then emit discrete events over ESP-NOW. Normal operation requires neither PC inference nor Internet access. Validate independently with a receiver test tool first.

Data path: Camera → ROI / preprocessing → static classifier → stabilization and release state machine → event output

| Module | Responsibility |
| --- | --- |
| capture | Own frame acquisition and lifetime; record resolution, format and failure causes. |
| inference | Preprocess inputs and invoke the model; report class, confidence and model version. |
| stabilizer | DISABLED / ARMED / WAIT_RELEASE; a sustained pose emits only one event. |
| transport | Version, source, sequence, acknowledgement and timeout; delivery does not mean an action was executed. |

## Draft interface

Candidate semantic fields: protocol_version, source_id, boot_id, sequence, gesture, confidence, stable. Use fixed-length, versioned wire messages with explicit byte order; freeze encoding and acknowledgement policy in P03. Do not directly subtract timestamps from different devices.

This contract has no validated implementation yet. Add examples, edge cases and migration notes when freezing it.

## Scope

The first version classifies static gestures and emits events. Continuous air-mouse control, dynamic trajectories and application-side actions are outside this repository.

## Open decisions

- Pin dependency versions and confirm compatibility.
- Use initial measurements to set numerical acceptance thresholds.
- Confirm available hardware and resource budgets.
