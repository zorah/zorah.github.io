---
title: "Synchronous Diffusion for Unsupervised Smooth Non-Rigid 3D Shape Matching"
collection: publications
permalink: /publication/2024-eccv-synchronous-diffusion
excerpt: 'Most recent unsupervised non-rigid 3D shape matching methods are based on the functional map framework due to its efficiency and superior performance. Nevertheless, respective methods struggle to obtain spatially smooth pointwise correspondences due to the lack of proper regularisation. In this work, inspired by the success of message passing on graphs, we propose a synchronous diffusion process which we use as regularisation to achieve smoothness in non-rigid 3D shape matching problems. The intuition of synchronous diffusion is that diffusing the same input function on two different shapes results in consistent outputs. Using different challenging datasets, we demonstrate that our novel regularisation can substantially improve the state-of-the-art in shape matching, especially in the presence of topological noise.'
date: 2024-10-01
venue: 'European Conference on Computer Vision (ECCV) (Accepted)'
authors: 'Dongliang Cao, <b>Zorah Lähner</b>, Florian Bernard'
teaser: /previews/cao2024sync.png
categories: [geometricDL,correspondence]
bibtex: true
---

{{ page.authors }}

<img class="pub_teaser" src="../images/previews/cao2024sync.png" alt="Teaser Image" title="teaser" />

## Abstract

> Most recent unsupervised non-rigid 3D shape matching methods are based on the functional map framework due to its efficiency and superior performance. Nevertheless, respective methods struggle to obtain spatially smooth pointwise correspondences due to the lack of proper regularisation. In this work, inspired by the success of message passing on graphs, we propose a synchronous diffusion process which we use as regularisation to achieve smoothness in non-rigid 3D shape matching problems. The intuition of synchronous diffusion is that diffusing the same input function on two different shapes results in consistent outputs. Using different challenging datasets, we demonstrate that our novel regularisation can substantially improve the state-of-the-art in shape matching, especially in the presence of topological noise.

## Resources

{% if page.paperurl %}<a href=" {{ page.paperurl }} ">[pdf]</a>{% endif %} {% if page.arxiv %}<a href=" {{ page.arxiv }} ">[arxiv]</a>{% endif %} {% if page.code %}<a href=" {{ page.code }} ">[github]</a>{% endif %} {% if page.video %}<a href=" {{ page.video }} ">[video]</a>{% endif %} {% if poster %}<a href=" {{ page.poster }} ">[video]</a>{% endif %}


## Bibtex

    @inproceedings{cao2024sync,
        author 	= { Dongliang Cao and Zorah Lähner and Florian Bernard},
        title 	= { Synchronous Diffusion for Unsupervised Smooth Non-Rigid 3D Shape Matching },
        booktitle = { European Conference on Computer Vision (ECCV) },
        year 	= 2024,
    }
