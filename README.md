# Application of ResNet and Other Techniques on Image Classification Task Modified MNIST


<p float="center">
    <img src="/images/mnist.png">
</p>
The goal of this project is to recognize the largest numeric value out of three hand-written numbers for each image in the modified MINIST dataset. A linear model was implemented to provide a good baseline for the clas- sification task. Then the experiments mainly focus on convolutional neural network(CNN), and specifically investigated the performance of the state-of-the-art Residual Network (ResNet). We discussed basic intuitions behind ResNet architecture, and presented some recent works on possible improvement on ResNet in last decade. A task-specific ResNet model was implemented and experimented with several factors such as the depth of network, different choices of optimizers, and the batch size. In the end, a final convolutional neural network pipeline is presented with a 97.6% accuracy on the held-out test set.

---

[View the full report](https://github.com/dorhelium/modifiedMNISTclassification/blob/master/report.pdf)

---

## Remarks

The code for ResNet is adapted from the [torchvision library](https://pytorch.org/docs/stable/torchvision/models.html) (official PyTorch module with network architectures, image transformations and others) implementation. ResNet were originally designed for ImageNet competition, which was a color (3-channel) image classification task with 1000 classes. MNIST dataset howerver only contains 10 classes and it’s images are in the grayscale (1-channel). Therefore, the original implementation is adjusted accordingly to fit the features in MNIST dataset.


 <img src="/images/results.png" >



