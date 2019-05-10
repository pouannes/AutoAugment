# Project paused because of my being accepted into Google Summer of Code 2019

### AutoAugment

This is my implementation of AutoAugment, a way to automatically search for the best transforms for Data Augmentation mainly in Computer Vision. It is intended to work with the [fastai](https://docs.fast.ai/) library, and with some adaptations with generic PyTorch models and transforms.

Here are the papers I used for this implementation and useful to read to understand what's going on:

- [AutoAugment: Learning Augmentation Strategies from Data](https://arxiv.org/pdf/1805.09501.pdf) (original AutoAugment paper, uses RL for augmentation parameters search)
- [Learning Data Augmentation Policies Using Augmented Random Search](https://arxiv.org/pdf/1811.04768.pdf) (Augmented Random Search (ARS) instead of RL)
  - [Simple random search provides a competitive approach to reinforcement learning](https://arxiv.org/abs/1803.07055) (ARS paper)

Additional useful resources:

- [platform.ai reading group session on AutoAugment](https://www.youtube.com/watch?v=qkl_7f4XO7A&list=PLFVO7pLzoo5pM8EXLJibB1RjCVbL9io2N&index=5&t=0s)

The available "child" models are:

- XResNet 18, 34, 50, 101 and 152 (vanilla ResNet with improvement from the paper [Bag of Tricks for Image Classification with Convolutionnal Neural Networks](https://arxiv.org/abs/1812.01187))
- Wide ResNet 40-2 and 28-10 from the paper [Wide Residual Networks](https://arxiv.org/abs/1605.07146) TODO
- Shake-Shake ResNet from the paper [Shake-Shake Regularization](https://arxiv.org/abs/1705.07485) TODO
- Shake-Drop TODO

TODO:

- Wide ResNet / Shake-thing with X ResNets?
- ResNeXt?
- Add table for each models: # params and relative performance on GPU
