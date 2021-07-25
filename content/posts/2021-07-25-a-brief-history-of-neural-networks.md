---
template: post
title: A Brief History Of Neural Networks
slug: a-brief-history-of-neural-networks
socialImage: /media/0_wewd4ggufngv_e8v.jpeg
draft: false
date: 2020-05-25T04:05:05.142Z
description: Everyone is aware of the recent Deep Learning achievements. But
  Neural Networks have a long history starting 80 years ago.
category: Machine Learning
tags:
  - Machine-Learning
---
## 1940 Prehistory: Artificial Neurons

The history of artificial neurons dates back to the 1940s, when Warren McCulloch (a neuroscientist) and Walter Pitts (a logician) modeled the biological working of an organic neuron in a first artificial neuron to show how simple units could replicate logical functions.

## 1950 Artificial Neural Networks

Inspired by Warren McCulloch’s and Walter Pitts’ publication, Frank Rosenblatt (a research psychologist working at Cornell Aeronautical Laboratory) worked in the 1950s on the Perceptron: a single layer of neurons able to classify pictures of a few hundred pixels. This can be seen as the first ancestor of modern neural networks.


![Image](media/image-1.jpeg)

The genius of Rosenblatt was to implement an algorithm to train the neurons based on a dataset. Rosenblatt inspired himself from the work of the Canadian psychologist Donald Hebb, who theorized in his 1949 book Organization of Behavior that connections between (organic) neurons are reinforced as they are used (this would only be confirmed in the 1960s). Rosenblatt’s idea was to replicate this with his Perceptron. The New York Times reported Rosenblatt prophesizing that Perceptrons would in the future be able to “recognize people and call out their name,” “instantly translate speech in one language to speech or writing in another language,” “be fired to the planets as mechanical space explorers” but also “reproduce itself” and be self-conscious.


### 1970 First Neural Network Winter (1970s—mid 1980s)

Unfortunately, due to its training algorithm, the Perceptron was limited to a single layer of neurons. Despite lots of interest in those early developments, MIT professors Marvin Minsky and Seymour Papert published in 1969 a book (Perceptrons: An introduction to computational geometry ) demonstrating that the Perceptron was limited in capabilities. This resulted in the first “neural network winter” until the mid-80s.

## 1985 Backpropagation


Paul Werbos, in his 1974 PhD thesis, was the first to propose using backpropagation to optimize neural networks. However, as we were in the first neural network winter, his work went unnoticed by the research community. It is only later, with the work of Rumelhart et al. (1986), that backpropagation was popularized as a training technique for neural networks. Armed with backpropagation, researchers could now use neural networks in many use cases. Notably, neural networks were used to recognize handwritten digits based on a technique proposed in 1989 by Yann LeCun. His model was successfully implemented, ending up reading digits written by hand in around 10 to 20% of all checks processed in the US. Nevertheless, a new issue soon appeared, causing training to become slow and unstable.

![Image](media/image-2.png)

### 1995 Second Winter (mid-1990s — mid-2000s)


As neural networks became deeper (with more stacked layers), backpropagation became slower due to the vanishing gradients problem. Simply put, the backpropagation algorithm requires using the activation functions’ derivatives (slopes). And, back then, the activation functions in use were mostly sigmoid and tanh. Unfortunately, their derivatives are close to zero, except in x ∈ [−1, 1] (as shown below). Thus, when you stack multiple layers, the gradient descent becomes slower and slower for the deeper layers, resulting in an exponentially slow optimization.

![Image](media/image-3.png)

## 2010 The Rise of Deep Learning

The 2010s saw the deep learning tsunami.


In the early 2010s, multiple studies recommended using a specific activation function (ReLu) in the neurons to transmit information (see Nair, V. and Hinton, G. E. (2010)). This, with better optimization algorithms (such as ADAM), helped to train deeper neural networks efficiently.

In 2012, the revolution started at the ImageNet Large Scale Visual Recognition Challenge, a data science competition to classify pictures. A team led by Alex Krizhevsky (from the University of Toronto) achieved an unprecedented error rate of 15.3%, whereas the second-best model got only 26.2%. Krizhevsky used a specific type of neural network: convolutional neural networks. Moreover, he trained his network using graphical processing units (GPU) instead of the traditional CPUs. In 2012, no other participants were using neural networks in this challenge. The next year, in the 2013 edition, all participants used similar neural networks.

In 2016, AlphaGo — an AI developed by DeepMind — beat the Go world champion. Computers had ruled chess-playing since 1997 after Deep Blue beat Kasparov in a famous match. But beating humans at playing Go is a much more complex challenge, with an estimated 10^170 possible combinations against 10120 for chess. Many experts were surprised by this early victory that wasn’t expected to happen until a decade later. Google acquired DeepMind in 2014 for more than $500 million.


In 2017, DeepMind released AlphaGo Zero, which beat the late 2016-AlphaGo 100 games to 0. AlphaGo Zero only required three days of training to achieve this, learning to play Go only by competing against itself. In 2017, DeepMind reported paying $243 million to its 700 employees. This amount increased twofold in 2018.


In 2020, OpenAI released the third iteration of an AI specialized in producing texts: GPT3. This AI can write poetry, tell stories, solve equations, code websites, and even write articles about itself. Earlier, in 1950, Alan Turing (1912–1946, famous English computer scientist) proposed the “Turing test” to assess if a machine could imitate human language well enough to be confused for a human. GPT-3 is now writing journal articles that are often barely recognizable from human ones. OpenAI — funded by Elon Musk — was initially a non-profit organization. However, it became a capped profit organization in 2019, capping the returns on investment at a hundred times the initial amount. Shortly after, they secured a $1 billion investment from Microsoft.

![Image](media/image-4.png)
