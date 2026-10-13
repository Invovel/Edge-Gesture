# Implementation roadmap

[中文](roadmap.md) | English

Advance on deliverables and acceptance evidence, not assumed calendar progress.

| Stage | Task | Completion criteria | Status |
| --- | --- | --- | --- |
| P01 | Static-image inference | Pin SDK and model dependencies and build independently. Save input provenance, actual output, latency and memory measurements. | Not started |
| P02 | Live gestures | Test gestures, empty scenes and natural movements. Report a confusion matrix, false triggers per hour and trigger latency. | Not started |
| P03 | Stable events | Test held poses, exit and re-entry, duplicate packets and disconnection. One valid pose produces one intent. | Not started |
| P04 | Receiver validation | Use a standalone receiver test tool. Disabled mode emits no operation events; reconnecting must not replay expired actions. Recognition and transmission work without Internet access. | Not started |
| P05 | Model improvement | Separate training and test scenes; compare lighting, distance and backgrounds. Report accuracy, latency and resource trade-offs. | Not started |

Research extension: Establish whether natural movements cause false triggers before pursuing personalized models. Compare single-frame thresholds and multi-frame stabilization on the same test set.

Update learning notes, results and next steps after each iteration. Preserve failures and their conditions.
