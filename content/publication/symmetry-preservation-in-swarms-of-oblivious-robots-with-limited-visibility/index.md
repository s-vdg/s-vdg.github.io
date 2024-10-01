---
title: Symmetry Preservation in Swarms of Oblivious Robots with Limited Visibility
publication_types:
  - "3"
authors:
  - Raphael Gerlach
  - admin
  - Christopher Hahn
  - Jonas Harbig
  - Peter Kling
abstract: >-
  In the general pattern formation (GPF) problem, a swarm of simple autonomous,
  disoriented robots must form a given pattern. The robots' simplicity imply a
  strong limitation: When the initial configuration is rotationally symmetric,
  only patterns with a similar symmetry can be formed [Yamashita, Suzyuki; TCS
  2010]. The only known algorithm to form large patterns with limited visibility
  and without memory requires the robots to start in a near-gathering (a swarm
  of constant diameter) [Hahn et al.; SAND 2024]. However, not only do we not
  know any near-gathering algorithm guaranteed to preserve symmetry but most
  natural gathering strategies trivially increase symmetries [Castenow et al.;
  OPODIS 2022].

  Thus, we study near-gathering without changing the swarm's rotational symmetry for disoriented, oblivious robots with limited visibility (the OBLOT-model, see [Flocchini et al.; 2019]). We introduce a technique based on the theory of dynamical systems to analyze how a given algorithm affects symmetry and provide sufficient conditions for symmetry preservation. Until now, it was unknown whether the considered OBLOT-model allows for any non-trivial algorithm that always preserves symmetry. Our first result shows that a variant of Go-to-the-Average always preserves symmetry but may sometimes lead to multiple, unconnected near-gathering clusters. Our second result is a symmetry-preserving near-gathering algorithm that works on swarms with a convex boundary (the outer boundary of the unit disc graph) and without holes (circles of diameter 1 inside the boundary without any robots). 
draft: false
featured: false
tags:
  - dynamical systems
  - coupled systems
  - distributed computing
  - robot swarms
  - autonomous mobile robots
  - gathering
  - pattern formation
  - limited visibility
projects:
  - "Algorithms for swarms: Distributed Computing meets Dynamical Systems"
image:
  filename: featured
  focal_point: Smart
  preview_only: false
links: 
	- name: arXiv
	  url: https://arxiv.org/abs/2409.19277
date: 2024-10-01T13:40:36.430Z
---
