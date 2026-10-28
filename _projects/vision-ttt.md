---
layout: page
title: Vision-TTT
description: Vision-side fast-weight memory for long-video spatial intelligence.
importance: 1
category: research
---

Long-video spatial reasoning requires more than a longer language-model context. Once visual tokens are projected and flattened into a one-dimensional sequence, their 2D grid structure and cross-frame geometric relationships become difficult to preserve. Vision-TTT moves fast-weight memory to the vision side, where spatial structure is still explicit.

The model combines Qwen3-VL visual features with VGGT geometry and compresses streaming spatial evidence into a fixed-size recurrent state before language decoding. This design is intended to retain long-range spatial information without forcing the LLM to store the full visual history.

Vision-TTT is trained on VSI-590K and 15K long-video counting examples. It reaches 66.11 on VSI-Bench and 51.54 on ReVSI. On 10-minute videos, spatial recall improves from 38.3 to 48.3 over Spatial-TTT-2B, while counting improves from 31.8 to 41.8. Sustained counting over 30- and 60-minute videos remains an open challenge.

This project is ongoing.
