# An Introduction to Deep Learning with PyTorch - Lab

This repository contains materials for an undergraduate level deep learning lab class held in 2023. at a public university in Italy. It is geared towards computer science students and designed to be their first contact with coding deep learning models. After having studied the theory during lectures, the implementation aspects of the models are expounded on in detail during a four hour lecture.

The students are expected to know Python well, so no time is wasted on explaining language features. Instead, the main focus is on the libraries, relevant programming abstractions, and gaining an intuition behind how neural networks work. Any familiarity with numpy, scikit-learn and similar machine learning libraries are highly desired.

This project will not be updated with new examples nor the lastest developments in the deep learning ecosystem. Feel free to use this material however you please.

## Contents

The [deep_learning_pytorch_lab](deep_learning_pytorch_lab.ipynb) notebook contains the lecture, while the [CIFAR-10_solution](CIFAR-10_solution.ipynb) notebook contains the solution to the CIFAR-10 exercise. The lecture covers the following topics and is structured in the following way:

1. First, the students are encouraged to play with a simple vanilla model on the [TensorFlow Playground](https://playground.tensorflow.org) for 5-10 minutes to gain a visual perspective and intuition behind fundamental deep learning concepts.

2. Tensors and tensor operations are introduced, followed by an example of automatic differention and a reflection on its importance.

3. Dataset and DataLoader are presented.

4. An example of MNIST handwritten digit classification with a 1-layer CNN. This includes downloading and visualizing the data, building and training the model and evaluating performance on the test dataset.

5. An exercise for the students of CIFAR-10 classification with a CNN analogous to the MNIST example. The code is ~95% written and similar but not identical to the MNIST example. It contains small tasks the students have to complete for the example to run. The intended time for completion is around 30 minutes. While the tasks seem very simple, it's actually a great test of understanding of the material covered, being the students' first contact with programming DL models.

6. A Grad-CAM example on a single image using the ResNet-50 model. As the lecture started with gaining visually an intuition on how a simple neural network works, it ends with a visual intuition on how a modern complex CNN might "see" its inputs.

7. Q&A session.

The notebook itself contains a fair amount of text describing the topics, but its intended use is with an experienced instructor so many details are present in the code that are intended to be verbally described during the lecture.

## How to Run

First make sure that you have Python installed, any version greater or equal than 3.6 should work. You can run the model locally by first installing the dependencies either in the notebook or with pip, and then running the notebook:

```bash
pip install -r requirements.txt
jupyter notebook
```

Otherwise, and this might be a better choice for a class of students, load the notebook into Google Colab and run it there.

## References

The lecture is constructed as heavily modified versions of the following examples from the official PyTorch documentation (see [license](https://github.com/pytorch/tutorials/blob/main/LICENSE)):

+ [Tensors and Tensor Operations](https://pytorch.org/tutorials/beginner/basics/tensorqs_tutorial.html)
+ [Autograd](https://pytorch.org/tutorials/beginner/introyt/autogradyt_tutorial.html)
+ [Dataset and DataLoader](https://pytorch.org/tutorials/beginner/basics/data_tutorial.html)
+ [MNIST Example](https://pytorch.org/tutorials/beginner/nn_tutorial.html?highlight=mnist)
+ [CIFAR-10 Tutorial](https://pytorch.org/tutorials/beginner/blitz/cifar10_tutorial.html)
