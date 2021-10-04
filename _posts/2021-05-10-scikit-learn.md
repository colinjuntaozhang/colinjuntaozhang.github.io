---
title: Scikit Learn in Python
layout: post
date: '2021-05-10 23:02:47'
description: Split dataset to train and test sets using SciKit Learn

tags:
- python
---
 

![scikit-learn](/assets/img/scikit_learn_intro.png)

When you’re working on a model and want to train it, you obviously have a dataset. But after training, we have to test the model on some test dataset. For this, you’ll a dataset which is different from the training set you used earlier. But it might not always be possible to have so much data during the development phase.

In such cases, the obviously solution is to split the dataset you have into two sets, one for training and the other for testing; and you do this before you start training your model.

But the question is, how do you split the data? You can’t possibly manually split the dataset into two. And you also have to make sure you split the data in a random manner. To help us with this task, the SciKit library provides a tool, called the Model Selection library. There’s a class in the library which is, aptly, named ‘train_test_split.’ Using this we can easily split the dataset into the training and the testing datasets in various proportions.
There are a few parameters that we need to understand before we use the class:
- test_size — 
  This parameter decides the size of the data that has to be split as the test dataset. This is given as a fraction. For example, if you pass 0.5 as the value, the dataset will be split 50% as the test dataset. If you’re specifying this parameter, you can ignore the next parameter.
- train_size 
  You have to specify this parameter only if you’re not specifying the test_size. This is the same as test_size, but instead you tell the class what percent of the dataset you want to split as the training set.
- random_state 
  Here you pass an integer, which will act as the seed for the random number generator during the split. Or, you can also pass an instance of the RandomState class, which will become the number generator. If you don’t pass anything, the RandomState instance used by np.random will be used instead.
