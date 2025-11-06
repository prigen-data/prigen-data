---
title: Home
layout: home
nav_order: 1
description: "Just the Docs is a responsive Jekyll theme with built-in search that is easily customizable and hosted on GitHub Pages."
permalink: /
---


# Welcome to Prigen  
{: .fs-9 }

A Fine-Grained Annotation of Privacy Behaviors in Android Apps  
{: .fs-6 .fw-300 }

<a href="https://zenodo.org/records/17523926" class="btn btn-primary fs-5 mb-4 mb-md-0 mr-2" target="_blank" rel="noopener noreferrer">
  Download Data
</a>

---

**Prigen** is a curated dataset containing **fine-grained human annotations of privacy behaviors in Android applications**.  
Each annotation identifies three source code statements most relevant to a given privacy behavior—providing a detailed understanding of how and why applications use personal information.

This dataset supports research in **feature localization**, **retrieval-augmented generation (RAG)**, and **model attention alignment**, where accurate mappings between human reasoning and model focus are crucial.  
While previous datasets have annotated Android privacy behaviors only at the *function level*, **Prigen** is the first to provide **statement-level annotations**.

---

## Dataset Overview

- **2,426 Android methods** annotated by **18 professional programmers** via Prolific  
- **259 methods** with *double annotations* (two independent annotators)  
- Each annotation includes **three code statements** most relevant to the privacy behavior  
- Focused on four *“purpose”* categories from Jain *et al.* (2022)  
- Distributed as `.pkl` files for easy loading in Python  

| File | Description |
|------|--------------|
| `xxx.pkl` | All annotated Android methods (2,426 total) |
| `yyy.pkl` | Methods with double annotations |
| `zzz.pkl` | IDs of functions with double annotations |

---

## Key Findings

- **Expressions** are the most common statement type linked to privacy behaviors, followed by **declarations** and **if statements**  
- The **privacy label type** (purpose) has minimal influence on statement relevance  
- **Double annotations** enable comparison between **human and model attention**  

---

## About Prigen

**Prigen** is developed by [Chia-Yi Su](https://chiayisu.github.io/) and [Collin McMillan](https://sdf.org/~cmc/) at the **University of Notre Dame**.  
The project aims to provide open, fine-grained datasets for advancing software engineering and AI research.

This dataset is **original** and **has not been used in any published paper**.

If you have questions or would like to collaborate, please contact us.

---

## Citation
```bibtex
@article{su2025prigen,
  title     = {Prigen: A Fine-Grained Dataset of Privacy Behaviors in Android Apps},
  author    = {Chia-Yi Su and Collin McMillan},
  journal   = {xxx},
  volume    = {xxx},
  pages     = {xxx},
  year      = {2025}
}
---






[Jekyll]: https://jekyllrb.com
[Markdown]: https://daringfireball.net/projects/markdown/
[Liquid]: https://github.com/Shopify/liquid/wiki
[Front matter]: https://jekyllrb.com/docs/front-matter/
[Jekyll configuration]: https://jekyllrb.com/docs/configuration/
[source file for this page]: https://github.com/just-the-docs/just-the-docs/blob/main/index.md
[Just the Docs Template]: https://just-the-docs.github.io/just-the-docs-template/
[Just the Docs]: https://just-the-docs.com
[MIND repo]: https://github.com/apcl-research/CMIND
[Just the Docs README]: https://github.com/just-the-docs/just-the-docs/blob/main/README.md
[GitHub Pages]: https://pages.github.com/
[Template README]: https://github.com/just-the-docs/just-the-docs-template/blob/main/README.md
[GitHub Pages / Actions workflow]: https://github.blog/changelog/2022-07-27-github-pages-custom-github-actions-workflows-beta/
[use the template]: https://github.com/just-the-docs/just-the-docs-template/generate
