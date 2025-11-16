---
title: "Q-Adam-mini: Memory-Efficient 8-bit Quantized Optimizer for Large Language Model Training"
authors:
- Yizhou Han
- admin
- Congliang Chen
- Xingjian Wang
- Ruoyu Sun
date: "2025-05-31"
# doi: ""

# 添加这行来禁用标题的默认链接
url: ""

# Schedule page publish date (NOT publication's date).
# publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["paper-conference"]

# Publication name and optional abbreviated publication name.
# publication: ""
publication_short: In *ICML 2025 Workshop ES-FoMo-III*

abstract: "We propose Q-Adam-mini, a memory-efficient optimizer for Large Language Model (LLM) training that achieves 8x reduction in GPU memory usage while maintaining performance parity with full-precision AdamW. Building upon Adam-mini, which reduces memory footprint of optimizer states by 50% compared to AdamW, we further improve memory efficiency through states quantization. We achieve this by: (i) quantizing the first-order momentum (m) to INT8 and (ii) retaining the second-order momentum (v) in FP32, which occupies less than 1% of total memory. However, embedding layer exhibits weight norm instability. We analyze this issue and address it by applying stochastic rounding for momentum quantization exclusively to the embedding layer. We validate our approach on both pre-training and fine-tuning tasks, with the model size ranging from 60M to 8B. Our results demonstrate that Q-Adam-mini enables scalable LLM training with limited computational resources. Codes are available at: https://anonymous.4open.science/r/Q-Adam-mini-FD45/"

# Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

# tags:
# - Large Language Models

# featured: true

links:
- name: Openreview
  url: https://openreview.net/pdf?id=sa3uVJLEsR
# url_pdf: http://arxiv.org/pdf/1512.04133v1
# url_code: 'https://github.com/HugoBlox/hugo-blox-builder'
# url_dataset: '#'
# url_poster: '#'
# url_project: ''
# url_slides: ''
# url_source: '#'
# url_video: '#'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
# image:
#   caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/s9CC2SKySJM)'
#   focal_point: ""
#   preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
# projects:
# - internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
---

<!-- This work is driven by the results in my [previous paper](/publication/conference-paper/) on LLMs.

{{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}}

Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/). -->
