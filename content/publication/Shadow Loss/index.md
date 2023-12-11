---
title: "Shadow Loss in Siamese Networks"
authors:
- admin
- Mohammad Junayed Hasan
- Humayra Anjum
- Nabeel Mohammed
author_notes:
date: "2023-10-02T00:00:00Z"
doi: "https://doi.org/10.48550/arXiv.2311.14012"

# Schedule page publish date (NOT publication's date).
#publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article-journal"]

# Publication name and optional abbreviated publication name.
publication: "*(Submitted for Publication)*"
publication_short: ""

abstract: "Despite significant recent advances in similarity detection tasks, existing approaches pose substantial challenges under memory constraints. One of the primary reasons for this is the use of computationally expensive metric learning loss functions such as Triplet Loss in Siamese networks. In this paper, we present a novel loss function called Shadow Loss that compresses the dimensions of an embedding space during loss calculation without loss of performance. The distance between the projections of the embeddings is learned from inputs on a compact projection space where distances directly correspond to a measure of class similarity. Projecting on a lower-dimension projection space, our loss function converges faster, and the resulting classified image clusters have higher inter-class and smaller intra-class distances. Shadow Loss not only reduces embedding dimensions favoring memory constraint devices but also consistently performs better than the state-of-the-art Triplet Margin Loss by an accuracy of 5%-10% across diverse datasets. The proposed loss function is also model agnostic, upholding its performance across several tested models. Its effectiveness and robustness across balanced, imbalanced, medical, and non-medical image datasets suggests that it is not specific to a particular model or dataset but demonstrates superior performance consistently while using less memory and computation."

# Summary. An optional shortened abstract.
summary: 

tags:
- AI
featured: false

# links:
# - name: ""
#   url: ""
url_pdf: 'https://arxiv.org/abs/2311.14012'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: ''
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
#slides: example
---


