---
title: "Q-Adam-mini: Memory-Efficient 8-bit Quantized Optimizer for Large Language Model Training"
authors:
- Yizhou Han
- admin
- Congliang Chen
- Xingjian Wang
- Ruoyu Sun
date: "2025-05-31"
publication_types: ["paper-conference"]
publication_short: In *ICML 2025 Workshop ES-FoMo-III*
abstract: "We propose Q-Adam-mini, a memory-efficient optimizer for Large Language Model (LLM) training that achieves 8x reduction in GPU memory usage while maintaining performance parity with full-precision AdamW. Building upon Adam-mini, which reduces memory footprint of optimizer states by 50% compared to AdamW, we further improve memory efficiency through states quantization. We achieve this by: (i) quantizing the first-order momentum (m) to INT8 and (ii) retaining the second-order momentum (v) in FP32, which occupies less than 1% of total memory. However, embedding layer exhibits weight norm instability. We analyze this issue and address it by applying stochastic rounding for momentum quantization exclusively to the embedding layer. We validate our approach on both pre-training and fine-tuning tasks, with the model size ranging from 60M to 8B. Our results demonstrate that Q-Adam-mini enables scalable LLM training with limited computational resources."
url_pdf: https://openreview.net/forum?id=sa3uVJLEsR
---
