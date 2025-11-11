---
title: Home
layout: home
nav_order: 1
description: "Just the Docs is a responsive Jekyll theme with built-in search that is easily customizable and hosted on GitHub Pages."
permalink: /
---


# Welcome to Prigen  
{: .fs-9 }
Dataset of Fine-grained Annotations of Privacy Behaviors in Android Applications
{: .fs-6 .fw-300 }

<a href="https://zenodo.org/records/17523926" class="btn btn-primary fs-5 mb-4 mb-md-0 mr-2" target="_blank" rel="noopener noreferrer">
  Download Data
</a>

---

This dataset contains **fine-grained human annotations of privacy behaviors in Android applications**. Each annotation identifies three source code statements most relevant to a given privacy behavior. This dataset supports research in **feature localization**, **retrieval-augmented generation (RAG)**, and **model attention alignment**. 

---

## Dataset Overview

- **2,426 Android methods** annotated by **18 software developers** via Prolific  
- **259 methods** with *two annotations* (two independent annotators)  
- Each annotation includes **three code statements** most relevant to the privacy behavior  
- Focused on four *“purpose”* categories from Jain *et al.* (2022)  

| File | Description |
|------|--------------|
| `prigen_data_one_annotation.pkl` | All methods with one annotation |
| `prigen_data_two_annotation.pkl` | Methods with two annotations |
| `prigen_two_annotation_fids.pkl` | IDs of functions with two annotations |

---

## Key Findings

- **Expressions** are the most common statement type linked to privacy behaviors, followed by **declarations** and **if statements**  
- The **privacy label type** has minimal influence on statement relevance  

---

## About Prigen

**Prigen** dataset is curated by [Chia-Yi Su](https://chiayisu.github.io/), [Aakash Bansal](https://aakashba.github.io/), [Vijayanta Jain](https://sites.google.com/maine.edu/vijayantajain/home), [
Sepideh Ghanavati](https://www.sepidehghanavati.com/), [Sai Teja Peddinti](https://sites.google.com/site/psaiteja/home), and [Collin McMillan](https://sdf.org/~cmc/). The project aims to provide open, fine-grained datasets for advancing software engineering and AI research.


If you have questions or would like to collaborate, please contact us.

---

## Citation
```bibtex
@software{su2025prigen,
  author = {Chia-Yi Su, Aakash Bansal, Vijayanta Jain, Sepideh Ghanavati, Sai Teja Peddinti, and Collin McMillan},
  doi = {10.5281/zenodo.1234},
  month = {11},
  title = {Dataset of Fine-grained Annotations of Privacy Behaviors in Android Applications},
  url = {https://zenodo.org/records/17523926},
  version = {0.1.0},
  year = {2025}
}
```
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
