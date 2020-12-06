---
layout: project
type: project
image: images/ai.png
title: Measuring Catastrophic Forgetting in Neural Networks
permalink: projects/catastrophicforgetting
# All dates must be YYYY-MM-DD format!
date: 2017-06-02
labels:
  - Deep Learning
  - Computer Vision
  - Machine Learning
  - Neural networks
  - Catastrophic forgetting
  - Lifelong learning
  - AAAI
summary: Over the past summer I researched the lifelong learning problem of catastrophic forgetting in neural networks at the Rochester Institute of Technology.
---

I received a NSF undergraduate research grant to do research in the kLab at the Rochester Institute of Technology.
The kLab is a research lab part of the Center of Imagining Science which focuses on solving the problem of lifelong learning through
machine learning and computer vision. <link>http://klab.cis.rit.edu/</link>

Catastrophic forgetting is the tendency for a neural network to immediately "forget" previously learned information after it is presented
with new, dissimilar information. This is a huge concern as we try to move towards more generalizeable and adaptable AI systems, and no efficient 
way to prevent this problem has been designed yet. 

Our task over the summer was research the common methods that had already been implemented in attempt to mitigate catastrophic forgetting,
and then design experiments to accurately compare them to each other so that we can focus future efforts on addressing the gaps in the current 
methods. 

<hr> 

Our lab group produced a paper about our research which was published to the Association for the Advancement of Artificial Intelligence
(AAAI) 2018.

Abstract: Deep neural networks are used in many state-of-the-art systems for machine perception. 
Once a network is trained to do a specific task, e.g., bird classification, it cannot easily be trained to do new tasks,
e.g., incrementally learning to recognize additional bird species or learning an entirely different task such as flower recognition. 
When new tasks are added, typical deep neural networks are prone to catastrophically forgetting previous tasks. Networks that are 
capable of assimilating new information incrementally, much like how humans form new memories over time, will be more efficient 
than re-training the model from scratch each time a new task needs to be learned. There have been multiple attempts to develop 
schemes that mitigate catastrophic forgetting, but these methods have not been directly compared, the tests used to evaluate them 
vary considerably, and these methods have only been evaluated on small-scale problems (e.g., MNIST). In this paper, we introduce new 
metrics and benchmarks for directly comparing five different mechanisms designed to mitigate catastrophic forgetting in neural networks: 
regularization, ensembling, rehearsal, dual-memory, and sparse-coding. Our experiments on real-world images and sounds show that the 
mechanism(s) that are critical for optimal performance vary based on the incremental training paradigm and type of data being used, 
but they all demonstrate that the catastrophic forgetting problem has yet to be solved.

Kemker, R., McClure, M., Abitino, A., Hayes T., and Kanan, C. (2017). (in press). Measuring Catastrophic Forgetting in Neural 
Networks. AAAI 2018. 

https://arxiv.org/abs/1708.02072
