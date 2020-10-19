---
layout: page
title: Smooth Shells
title_long: Smooth Shells - Multi-Scale Shape Registration with Functional Maps
description: CVPR 2020
img: /assets/img/eisenberger2020smoothshells.png
---

Marvin Eisenberger, *Zorah Lähner*, Daniel Cremers

<img class="col two teaser" src="{{ site.baseurl }}/assets/img/eisenberger2020smoothshells.png" alt="Teaser Image" title="teaser" />

**Abstract**

We propose a novel 3D shape correspondence method
based on the iterative alignment of so-called smooth shells.
Smooth shells define a series of coarse-to-fine shape approximations designed to work well with multiscale algorithms. The main idea is to first align rough approximations of the geometry and then add more and more details to refine the correspondence. We fuse classical shape
registration with Functional Maps by embedding the input shapes into an intrinsic-extrinsic product space. Moreover, we disambiguate intrinsic symmetries by applying a
surrogate based Markov chain Monte Carlo initialization.
Our method naturally handles various types of noise that
commonly occur in real scans, like non-isometry or incompatible meshing. Finally, we demonstrate state-of-theart quantitative results on several datasets and show that
our pipeline produces smoother, more realistic results than
other automatic matching methods in real world applications.

**Resources**

[(pdf + supp)](../assets/pdfs/eisenberger2020smoothshells.pdf) [(arxiv)](https://arxiv.org/abs/1905.12512) [(github)](https://github.com/marvin-eisenberger/smooth-shells) [(video)](../assets/videos/eisenberger2020smoothshells.mp4)

**Bibtex**

    @InProceedings{eisenberger2020smoothshells,
      author       = "Marvin Eisenberger and Zorah L\"ahner and Daniel Cremers",
      title        = "Smooth Shells: Multi-Scale Shape Registration with Functional Maps",
      booktitle    = "IEEE Conference on Computer Vision and Pattern Recognition (CVPR)",
      month        = "June",
      year         = "2020",
    }
