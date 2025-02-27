# Twofold Debiasing Enhances Fine-Grained Learning with Coarse Labels. (AAAI 2025 Poster)

>TheCoarse-to-Fine Few-Shot (C2FS) task is designed to train models using only coarse labels, then leverages an extremely small number of subclass examples to achieve fine-grained recognition capabilities. Intuitively, it is particularly challenging as coarse-grained supervised pre-training leads to the reduction of fine-grained features which are essential for subcategory separation, and the learned models are prone to overfitting due to the biased distributions formed by a few samples. In this paper, we propose a tailored method that calibrates biased distributions caused by a few fine labeled examples by incorporating coarse labeled features enriched with fine-grained attributes. Specifically, we first enhance the embeddings with fine-grained information using multi-layer fusion reconstruction and intermediate layer feature alignment. By fully leveraging the hierarchical relationship between coarse and fine labels, we subsequently augment the fine-grained classifier’s input with readily available coarsegrained sample embeddings, effectively calibrating the biased distributions formed within the few-shot context. Extensive experiments conducted on five benchmark datasets demonstrate the efficacy of our approach, achieving state-of-the-art results that surpass competitive methods.

### Pretrained Models

| dataset           | model     |  5-way acc.   | all-way acc. | 
|----------------|:-----------:|:--------------:|:--------------:|
| LIVING-17      | ResNet-50 | 89.23 ± 0.55 | 45.14 ± 0.12 |
| NONLIVING-26   | ResNet-50 | 86.23 ± 0.54 | 43.10 ± 0.11 |
| ENTITY-13      | ResNet-50 | 90.58 ± 0.54 | 42.29 ± 0.08 | 
| ENTITY-30      | ResNet-50 | 88.12 ± 0.54 | 41.79 ± 0.08 | 
| CIFAR-100      | ResNet-12 | 74.56 ± 0.70 | 29.84 ± 0.11 |
| tieredImageNet | ResNet-12 | 63.54 ± 0.70 | 11.97 ± 0.06 |



### License
Copyright 2019 IBM Corp. This repository is released under the Apachi-2.0 license (see the LICENSE file for details)

### References
[1] Guy Bukchin, Eli Schwartz, Kate Saenko, Ori Shahar, Rogerio Feris, Raja Giryes, Leonid Karlinsky, Fine-grained Angular Contrastive Learning with Coarse Labels
. Accepted to CVPR 2021 (Oral). https://arxiv.org/abs/2012.03515
