---
layout: page
title: SHREC'16 Topology
title_long: SHREC16: Matching of Deformable Shapes with Topological Noise
description: 3DOR 2016
img: /assets/img/laehner2016shrec.png
---

Some details on this site are still under construction but the links should work correctly already.

Contest Organizers:
*Zorah Lähner*, Emanuele Rodolà, Michael M. Bronstein, Daniel Cremers

Paper Authors:
*Zorah Lähner*, Emanuele Rodolà, Michael M. Bronstein, Daniel Cremers, Oliver Burghard, Luca Cosmo, Alexander Dieckmann, Rolf Klein and Yusuf Sahillioglu

<img class="col two teaser" src="{{ site.baseurl }}/assets/img/laehner2016elastic2D3D.png" alt="Teaser Image" title="teaser" />

**Abstract**

> We propose the first algorithm for non-rigid 2D-to-3D shape matching, where the input is a 2D query shape as well as a 3D target shape and the output is a continuous matching curve represented as a closed contour on the 3D shape. We cast the problem as finding the shortest circular path on the product 3-manifold of the two shapes. We prove that the optimal matching can be computed in polynomial time with a (worst-case) complexity of O(mn^2 log(n)), where m and n denote the number of vertices on the 2D and the 3D shape respectively. Quantitative evaluation confirms that the method provides excellent results for sketch-based deformable 3D shape retrieval.

This was a track of the 2016 SHREC contest ([www.shrec.net](https://www.shrec.net)). The contest is finished and the results were published in [this paper](../assets/pdfs/shrec16-3dor.pdf).

## Introduction

Matching deformable 3D shapes is an active area of research, which has attracted the interest of many researchers during the years. A wide variety of approaches have been proposed to tackle the problem of (nearly-)isometric shape matching with different levels of robustness against topological changes and geometric noise. Standard data sets typically concentrate on the type of non-rigid deformation (i.e. change in pose and in shape class) and only include minor factors of nuisance, such as small holes and numerical noise. By contrast, the topological change of triangular meshes due to the coalescence of spatially close surface regions have been much less investigated during the years; few datasets include such instances, and these are limited to the coalescence of small areas. From a real world perspective, during a typical 3D acquisition process parts that touch each other are hidden from the sensors and will create a topologically different surface. For example, arms hanging down and along the body of a human shape may touch the torso and the legs, and there the shape is coalesced although they are not physically connected. These topological changes are very hard to match and, to the best of our knowledge, there exists no benchmark focusing on this class of changes.

IMAGES

Our data set includes shapes from the KIDS dataset [1] and new shapes produced with a free version of DAZ Studio 4.9, but merges parts that are self-intersecting so as to create a non-intersecting manifold surface using the method described in [2]. This changes the topology of each shape in several regions and to various degrees, creating a diverse but realistic data set.

IMAGES
In the original shape, arm and fingers intersect with the body and leg respectively, penetrating the shape. In the new shape the intersecting parts are removed, and the visible parts are stitched to the body.

## Dataset

The dataset contains **25 non-rigidly deformed versions of a “null” shape** (i.e. a shape in a neutral pose with no topological changes) undergoing different **topological changes**. The shapes are partly taken from the KIDS dataset but any self-intersections are removed, creating topological changes on different parts of the shape.

A **subset of 15 shapes is given as training data**. For each shape in the training set the correspondence to the null shape is given. Additionally, ground-truth correspondence mapping each point to its left-right symmetric counterpart is also provided. Note that, as a result of the merging, some points may not have a symmetric match.

Due to the changes, not all vertices in the modified shapes have a reliable ground-truth match onto the null shape. A map indicating these vertices is included in the data set (see inset figure - yellow indicates points with no reliable matches).

The whole data set exists in **two different resolutions**, ~10k vertices and ~60k-80k vertices.

### Files


* **kid[i].off** - shape data, *i between 00 and 25*
* **kid[i]_info.txt** - Some basic information about the shape including number of vertices etc.
* **kid[i]_indmap.txt** - Indices of vertices that have no match on the null shape, *only for high resolution, in the low resolution set all vertices have a match on the null shape*
* **kid[i]_ref.txt** - Ground-truth matches to the null shape, *only for the training set*
* **kid[i]_sym.txt** - Ground-truth left-right matches, *only for the training set and for the high resolution set*

### Downloads

In the contest the shapes 1-15 were given as training data and 16-25 were used for testing. The evaluation code allows you to put your method in comparison to the methods that participated in the contest.

* Low resolution dataset (~10k vertices) - [https://www.dropbox.com/s/kejp7sprttk7n46/TOPKIDS_lowres.zip?dl=0]([download, 8 MB])
* High resolution dataset (~60k-80k vertices) - [https://www.dropbox.com/s/aqrsdt5z7d7acc9/TOPKIDS_highres.zip?dl=0]([download, 43.6 MB])
* Both complete datasets - [https://www.dropbox.com/s/r0jyiglkog1442z/TOPKIDS.zip?dl=0]([download, 51.6 MB])
* Evaluation Code - [https://www.dropbox.com/s/m9tf7l4ge7pqmvx/evaluation.zip?dl=0]([download, 38 kB])

**Bibtex**

    @InProceedings{laehner2016topkids,
        author = { Z. L\"ahner and E. Rodol\`a and M. M. Bronstein and D. Cremers and O. Burghard and L. Cosmo and A. Dieckmann and R. Klein and Y. Sahillioglu },
        title = { SHREC’16: Matching of Deformable Shapes with Topological Noise },
        booktitle = { Proc. of Eurographics Workshop on 3D Object Retrieval (3DOR) },
        year = { 2016 }
}
