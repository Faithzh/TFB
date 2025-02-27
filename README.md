# Twofold Debiasing Enhances Fine-Grained Learning with Coarse Labels (AAAI 2025 Poster)

>The Coarse-to-Fine Few-Shot (C2FS) task is designed to train models using only coarse labels, then leverages an extremely small number of subclass examples to achieve fine-grained recognition capabilities. Intuitively, it is particularly challenging as coarse-grained supervised pre-training leads to the reduction of fine-grained features which are essential for subcategory separation, and the learned models are prone to overfitting due to the biased distributions formed by a few samples. In this paper, we propose a tailored method that calibrates biased distributions caused by a few fine labeled examples by incorporating coarse labeled features enriched with fine-grained attributes. Specifically, we first enhance the embeddings with fine-grained information using multi-layer fusion reconstruction and intermediate layer feature alignment. By fully leveraging the hierarchical relationship between coarse and fine labels, we subsequently augment the fine-grained classifier’s input with readily available coarsegrained sample embeddings, effectively calibrating the biased distributions formed within the few-shot context. Extensive experiments conducted on five benchmark datasets demonstrate the efficacy of our approach, achieving state-of-the-art results that surpass competitive methods.

![图片3](https://github.com/user-attachments/assets/b6e077f6-5895-444a-aef6-2a000aa32fe6)

### Main results

| dataset           | model     |  5-way acc.   | all-way acc. | 
|----------------|:-----------:|:--------------:|:--------------:|
| LIVING-17      | ResNet-50 | 91.89 ± 0.54 | 53.42 ± 0.12 |
| NONLIVING-26   | ResNet-50 | 90.35 ± 0.53 | 49.74 ± 0.11 |
| ENTITY-13      | ResNet-50 | 91.56 ± 0.54 | 43.23 ± 0.08 | 
| ENTITY-30      | ResNet-50 | 91.73 ± 0.54 | 45.03 ± 0.08 | 
| CIFAR-100      | ResNet-12 | 84.15 ± 0.70 | 39.03 ± 0.11 |
| tieredImageNet | ResNet-12 | 63.15 ± 0.69 | 12.98 ± 0.06 |
