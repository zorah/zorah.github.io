---
layout: page
title: Kernel Matching
title_long: Efficient Deformable Shape Correspondence via Kernel Matching
description: 3DV 2017
img: /assets/img/vestner2017kernel.png
---

Matthias Vestner\*, *Zorah Lähner*\*, Amit Boyarski\*, Or Litany, Ron Slossberg, Tal Remez, Emanuele Rodolà, Alex Bronstein, Michael Bronstein, Ron Kimmel, Daniel Cremers

*(Authors with \* contributed equally.)*

<img class="col two teaser" src="{{ site.baseurl }}/assets/img/vestner2017kernel.png" alt="Teaser Image" title="teaser" />

**Abstract**

> We present a method to match three dimensional shapes under non-isometric deformations, topology changes and partiality. We formulate the problem as matching between a set of pair-wise and point-wise descriptors, imposing a continuity prior on the mapping, and propose a projected descent optimization procedure inspired by difference of convex functions (DC) programming. Surprisingly, in spite of the highly non-convex nature of the resulting quadratic assignment problem, our method converges to a semantically meaningful and continuous mapping in most of our experiments, and scales well. We provide preliminary theoretical analysis and several interpretations of the method.

**Resources**

[(pdf)]({{ site.baseurl }}/assets/pdfs/kernel17.pdf) [(arxiv)](https://arxiv.org/abs/1707.08991) [(github)](https://github.com/zorah/KernelMatching)

**Bibtex**

    @InProceedings{vestner17kernel,
      author = {Matthias Vestner and Zorah L\\"ahner and Amit Boyarski and Or Litany and Ron Slossberg and Tal Remez and Emanuele Rodolà and Alex M. Bronstein and Michael M. Bronstein and Ron Kimmel and Daniel Cremers},
      title = {Efficient Deformable Shape Correspondence via Kernel Matching},
      booktitle = {International Conference on 3D Vision (3DV)},
      year = {2017},
      month = {October},
      address = {Qingdao, China},
    }
