---
author: Luis Gomez
date: 2018-10-10 15:27:00
subtitle: Making the choice easy for idiots like me
tags:
  - AI
  - ML
  - Code
  - Deep Learning
title: The Only 4 Deep Learning Frameworks That Matter
url: /2018/10/10/the-only-4-deep-learning-frameworks-that-matter/
ShowReadingTime: true
---


Let me get this off my chest right off the bat: Keras is all you need for 90% of neural network tasks. Before jumping in, you should understand what is going on with neural networks(watch [3Blue1Brown's videos](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi)).

Ideally, you can understand all the math behind them and code a basic one from scratch (read [Nielsen's Neural Networks and Deep Learning](http://neuralnetworksanddeeplearning.com/index.html)).

But for most cases, even *understanding* is unnecessary with all the pretrained models frameworks ship with nowadays.

But, assuming you're not a n00b and you need to do more beyond just classifying 2D images or recognizing characters, here are the Deep Learning/ Neural Network frameworks can best fit your use case.

## The Only 4 Deep Learning Frameworks That Matter



1. [Keras](https://keras.io) 🅱️
  * **TLDR:** Are you a researcher/startup employee that wants to *test ideas 10x faster* than the competition? Just use Keras already.
  * Okay okay fellow pedants - Keras is more of a *library* than a *framework*. Regardless of what you call it, it is undeniably an incredible tool. It's favored by researchers and AI startups alike for its readability and ability to rapidly create neural networks.

    It works by using a framework in its backend (e.g. TensorFlow) to do all the neural network math, and wraps different functionalities for easy usage. Keras gives you high level functions to do things like create layers, apply max pooling, check accuracy, and other common neural network tasks in a single line of code.

    Having these possibilities at the tips of your fingers is invaluable when trying out many different model architectures.

    > pro deployment tip, you can export Keras models as TF graphs and upload them to CloudML to deploy your network in under 30 mins.


2. [Caffe2](https://caffe2.ai) ☕
  * **TLDR**: Do you need a neural network to run on *mobile*? Move Caffe2 to the top of your list.
  * This Facebook-supported framework offers extremely high performance with a focus on large scale deployments and mobile models. Users love it for its excellent performance on mobile devices, flexibility, and ease of writing. It is usually used through the Python API, though there is a C++ API as well. Also, a model can be written in Python then deployed in pure C++ for additional performance and scalability.

    Caffe2 also comes with a TON of pretrained models form the lovely [Model Zoo](https://github.com/caffe2/models).


2. [PyTorch](https://pytorch.org) 🔥
  * **TLDR:** Are you a researcher? Do you need to try a complex RNN, or a net with changing dimensions? PyTorch it is.
  * Another Facebook-supported framework, this Python library has a heavy focus on research and dynamic computation. It is loved by researchers for the ability to create exotic, experimental neural networks (without writing Lua 😈). If you have a crazy idea that you’re not sure how to implement with other frameworks, check out PyTorch. Many recent, successful research papers release their code in PyTorch. Don’t let all the research talk scare you though, PyTorch still has an accessible API, great performance, and documentation.


4. [TensorFlow](https://tensorflow.org) 🤔
  * **TLDR:** Need in-browser neural networks?
  * Sorry to put you at the bottom of the list, TensorFlow. The focus on parallelism and ease of integration with Google’s CloudML makes TensorFlow deploying highly scalable networks easy, at the expense of typically writing more complex code. It is not as intuitive to write as the other frameworks mentioned. The main reason I list it here because of the exciting new TensorFlow.js enabling high-performance, in-browser models. It is getting better and better at mobile performance but still doesn't touch Caffe2. I think TensorFlow is worth keeping an eye on as Google continue to innovate and integrate ML into different areas, but unless you have

  > if you're a beginner who needs to deploy a model, CloudML is a great option. But don't feel like you *have* to learn TensorFlow. You can write and train a model in Keras and export a TensorFlow graph and upload that.


There you go. In my humble opinion, these are the only 4 deep learning frameworks that matter in 2018.

Don't let yourself get into a black hole of paralysis by analysis, researching every framework endlessly. Pick one of the above. There are good tutorials for all of them. Pick one and learn it. If you need to switch over to another for some reason, the skills you learn in one will transfer to other. Just *start*!

> *there is no red K emoji, 🅱️ is the best I can do
