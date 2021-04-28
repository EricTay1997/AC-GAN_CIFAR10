# AC_GAN_CIFAR10

Contains code that implements multiple AC-GAN models, which are train on the CIFAR-10 dataset.

## Inception Network

- `resnet_training.ipynb` uses the ResNet architecture defined in `resnet20.py` and training code in `train_util.py` to train our Inception Network, which is saved as `net_before_pruning.pt`. Code for this section was provided in Homework 3 of Duke's ECE 590.07 class (Spring 2021). 

## Model 1

- `original.ipynb` is used to train Model 1 (Original Implementation), and saves the final Generator and Discriminator as `generator100_original.pt` and `discriminator100_original.pt` respectively.
- Statistics gathered during training is stored in `data_original.csv`.

## Model 2

- `finetune_small.ipynb` is used to finetune Model 2, and saves the best Generator and Discriminator as `generator160_small.pt` and `discriminator160_small.pt` respectively.

## Model 3

- `large.ipynb` is used to train Model 3, and saves the final Generator and Discriminator as `generator100_large.pt` and `discriminator100_large.pt` respectively.
- Statistics gathered during training is stored in `data_large.csv`.

## Model 4

- `finetune_large.ipynb` is used to finetune Model 3, and saves the best Generator and Discriminator as `generator120_large.pt` and `discriminator120_large.pt` respectively.

## Model Evaluation

- `model_evaluation.ipynb` uses the checkpointed models and generates the results and images in `report.pdf`.