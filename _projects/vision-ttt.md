---
layout: page
title: Vision-TTT
description: Vision-side fast-weight memory for long-video spatial intelligence.
importance: 1
category: research
---

Long-video memory is usually written inside the language model, after visual tokens have already been flattened. Vision-TTT moves fast-weight memory to the vision side of Qwen3-VL-4B: three hybrid layers and one anchor sit before the language model, and VGGT geometry is fused into that memory.

The model is pre-trained on VSI-590K and then mixed with about 15K long-video counting examples. VSI-Bench average is 66.11 and ReVSI is 51.54. At 10 minutes, spatial recall is 48.3 against 38.3 for Spatial-TTT-2B, and counting is 41.8 against 31.8. Counting at 30 and 60 minutes still trails Spatial-TTT.
