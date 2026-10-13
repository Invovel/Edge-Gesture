# Project-driven learning path

[中文](README.md) | English

For each stage, record: question → principle → minimal experiment → observations → interpretation and limits.

## P01: Static-image inference

Pin SDK and model dependencies and build independently. Save input provenance, actual output, latency and memory measurements.

Explain inputs, outputs, failure conditions and design choices.

## P02: Live gestures

Test gestures, empty scenes and natural movements. Report a confusion matrix, false triggers per hour and trigger latency.

Explain inputs, outputs, failure conditions and design choices.

## P03: Stable events

Test held poses, exit and re-entry, duplicate packets and disconnection. One valid pose produces one intent.

Explain inputs, outputs, failure conditions and design choices.

## P04: Receiver validation

Use a standalone receiver test tool. Disabled mode emits no operation events; reconnecting must not replay expired actions. Recognition and transmission work without Internet access.

Explain inputs, outputs, failure conditions and design choices.

## P05: Model improvement

Separate training and test scenes; compare lighting, distance and backgrounds. Report accuracy, latency and resource trade-offs.

Explain inputs, outputs, failure conditions and design choices.

Add references for the current task rather than collecting a curriculum in advance.
