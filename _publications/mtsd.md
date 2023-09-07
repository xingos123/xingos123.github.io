---
title: "Cross-Lingual Cross-Target Stance Detection via Adversarial Heterogeneous Graph Augmented Prompt Tuning"
collection: publications
permalink: /publication/mtsd
excerpt: '<div align="middle"><img align="middle" style="max-width: 540px; width: 100%" src="https://xingos123.github.io/files/seke2023/mtsd.png" /></div> To this end, we propose a comprehensive solution to tackle the challenge of cross-language cross-target stance detection on social media platforms, which is called adversarial heterogeneous graph augmented prompt (AHGA) tuning framework. Specifically, we use a simple-effective cross-lingual prompt encoding machanism to solve the input problem for multilingual content and enhance short text representation, then we leverage context metadata to construct a batch-wise heterogeneous graph. In this graph, each labeled item is represented by a node and edges between the nodes denote the similarity between the items. AHGA establishes edges in the heterogeneous graph based on whether two news items share common attributes such as stance or sentiment, and further regulates the similarity of the representations learned by PLMs between each pair of news items to conform with the edges of the heterogeneous graph. The scalability of HGAPT is noteworthy since the heterogeneous graph is constructed based on a mini-batch of sampled data points per iteration. To further enhance the feature adaption of heterogeneous graph learning, we exploit adversarial attacks to plenish noise to the MASK representation by computing adversarial worst-case perturbations, forcing the model to learn non-trivial but effective features.'
date: 1997-01-01
venue: 'None'
---
<!-- 
[arXiv](https://arxiv.org/abs/2009.04724){: .btn .btn--info}
[code](https://github.com/bighuang624/AGAM){: .btn .btn--info}
[poster](https://kyonhuang.top/files/AGAM/aaai21-AGAM-poster.pdf){: .btn .btn--info}
[slide](https://kyonhuang.top/files/AGAM/aaai21-AGAM-presentation.pdf){: .btn .btn--info}

## Background

The purpose of few-shot recognition is to recognize novel categories with a limited number of labeled examples in each class. To encourage learning from a supplementary view, recent approaches have introduced auxiliary semantic modalities into effective metric-learning frameworks that aim to learn a feature similarity between training samples (support set) and test samples (query set). However, these approaches only augment the representations of samples with available semantics while ignoring the query set, which loses the potential for the improvement and may lead to a shift between the modalities combination and the pure-visual representation. In this paper, we devise an **attributes-guided attention module (AGAM)** to utilize human-annotated attributes and learn more discriminative features. Contributions are:

1. AGAM utilizes powerful channel-wise and spatial-wise attention to learn what information to emphasize or suppress. While considerably improving the representativeness and discriminability of representations in a fine-grained manner, features extracted by both visual contents and corresponding attributes share the same space with pure-visual features.

2. AGAM applies an attention alignment mechanism between the attributes-guided and self-guided branches. The mechanism contributes to learning the query representations by matching the focus of two branches, so that the supervision signal from the attributes-guided branch promotes the self-guided branch to concatenate on more important features even without attributes.

3. We conduct extensive experiments to demonstrate that the performance of various metric-based methods is greatly improved by plugging our light-weight module.

## Model Overview

![](https://kyonhuang.top/files/AGAM/AGAM-model-structure.png)

In AGAM, we design two parallel branches, *i.e.*, **attributes-guided branch** and **self-guided branch**. For samples with attributes annotations, the attributes-guided branch learns the attention weights by incorporating both attributes and visual contents. And the self-guided branch is designed for the inference of samples without the guidance of attributes. Furthermore, we propose an **attention alignment mechanism** in AGAM, which aims to pull the focus of the two branches closer, so that the self-guided branch can capture more informative features for query samples without the guidance of attributes. Note that AGAM is a flexible module and can be easily added into any part of convolutional neural networks. -->

<!-- This plug-and-play module enables visual contents and corresponding attributes to collectively focus on important channels and regions for support set. And the feature selection is also achieved for query set with only visual information while the attributes are not available. Therefore, representations from both sets are improved in a fine-grained manner. Moreover, an attention alignment mechanism is proposed to distill knowledge from the guidance of attributes to the pure-visual branch for samples without attributes. Extensive experiments and analysis show that our proposed module can significantly improve simple metric-based approaches to achieve state-of-the-art performance on different datasets and settings. -->

<!-- ## Experiment Results

Here we report some experimental results to empirically show the effectiveness of our AGAM. Please check the paper for the details of the experiment settings and further analysis.

### Adapting AGAM into Existing Frameworks

![](https://kyonhuang.top/files/AGAM/adapting-results.png)

### Comparison with State-of-the-Arts

Results on the CUB dataset:

![](https://kyonhuang.top/files/AGAM/sota-CUB.png)

Results on the SUN dataset:

![](https://kyonhuang.top/files/AGAM/sota-SUN.png)

### Visualization Analysis

<div align="middle"><img align="middle" style="max-width: 500px; width: 100%" src="https://kyonhuang.top/files/AGAM/AGAM-Grad-CAM.png" /></div>

Gradient-weighted class activation mapping (Grad-CAM) visualization of query samples. Each row is the result of the same query sample, and each column is: (a) Original images. (b) Results of Prototypical Network. (c) Results of AGAM but removing the attention alignment mechanism. (d) Results of the complete AGAM. It is observed that incorporating the complete AGAM helps to attend to more representative local features.

## BibTex

If our paper and codes are helpful for you research, please cite our paper:

<pre>
@inproceedings{Huang2021AGAM,
  author = {Siteng Huang and Min Zhang and Yachen Kang and Donglin Wang},
  title = {Attributes-Guided and Pure-Visual Attention Alignment for Few-Shot Recognition},
  booktitle = {Proceedings of the 35th {AAAI} Conference on Artificial Intelligence},
  month = {February},
  year = {2021}
}
</pre> -->