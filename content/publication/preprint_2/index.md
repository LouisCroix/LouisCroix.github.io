---
title: "Learning Word Embedding with Better Distance Weighting and Window Size Scheduling"
authors:
- admin
- Chris Ding
date: "2024-01-20"
# doi: ""

# Schedule page publish date (NOT publication's date).
# publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article"]

# Publication name and optional abbreviated publication name.
# publication: ""
# publication_short: ""

abstract: "Distributed word representation (a.k.a. word embedding) is a key focus in natural language processing (NLP). As a highly successful word embedding model, Word2Vec offers an efficient method for learning distributed word representations on large datasets. However, Word2Vec lacks consideration for distances between center and context words. We propose two novel methods, Learnable Formulated Weights (LFW) and Epoch-based Dynamic Window Size (EDWS), to incorporate distance information into two variants of Word2Vec, the Continuous Bag-of-Words (CBOW) model and the Continuous Skip-gram (Skip-gram) model. For CBOW, LFW uses a formula with learnable parameters that best reflects the relationship of influence and distance between words to calculate distance-related weights for average pooling, providing insights for future NLP text modeling research. For Skip-gram, we improve its dynamic window size strategy to introduce distance information in a more balanced way. Experiments prove the effectiveness of LFW and EDWS in enhancing Word2Vec's performance, surpassing previous state-of-the-art methods."

# Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

# tags:
# - Large Language Models

featured: true

# links:
# - name: Custom Link
#   url: http://example.org
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
