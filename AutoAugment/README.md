# AutoAugment

This is my implementation of AutoAugment, a way to automatically search for the best transforms for Data Augmentation mainly in Computer Vision. It is intended to work with the [fastai](https://docs.fast.ai/) library, and with some adaptations with generic PyTorch models and transforms.

Here are the papers I used for this implementation:

- [AutoAugment: Learning Augmentation Strategies from Data](https://arxiv.org/pdf/1805.09501.pdf) (original AutoAugment paper, uses RL);
- [Learning Data Augmentation Policies Using Augmented Random Search](https://arxiv.org/pdf/1811.04768.pdf) (random search instead of RL).