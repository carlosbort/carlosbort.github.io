---
layout: post
title: Fundamentals of Machine Learning [ENG]
tags: [Machine Learning, Teaching]
date: 2020-11-30
category: Post
---

This year I debuted as a teacher in the [Data Science & Big Data Analytics - MDS+](https://thevalley.es/formacion/master-data-science-big-data-analytics) at [The Valley Business School](https://thevalley.es). A master's degree that aims to teach practical Data Capabilities and Strategy, for today's data practitioners. *Fundamentals of Machine Learning*

The objective of the session is for the students to understand how a Machine Learning algorithm works and how to approximate a real problem from their company. In addition, context will be given on the subject and the process that data modeling follows.If I have to summary the class in four things, they are:

<h3>1. Machine Learning definition and context </h3>

**Machine Learning**, is a branch of artificial intelligence where algorithms acquire their own knowledge through examples. To contextualize the concepts, Artificial Intelligence, Machine Learning and Deep Learning, let's look at the following image:

<p align="center">
<img src="/images/venn_ML.png" width="560px"/>
<br>
Source: Chapter 1: Introduction - Deep Learning Book
</p>

- **Artificial intelligence:** it is the base of knowledge, it can be coded inference rules
- **Machine Learning:** it is when the algorithms acquire knowledge through the examples without intervention in their learning
- **Deep Learning:** when these algorithms learn to represent very complex concepts by representing them in a simple way. Used on images and text 


<h3>2. Why now? </h3>

During different moments of the late twentieth century, a lot was said about artificial intelligence and the different applications it would have. Why has the expansion been in the last 10 years?

1. **Context**
	- Data: digitization of the Company and lowering the price of disk storage
	- Computation capabilities: computing capabilities have been doubling every 2 years, the well-known Moore's Law
	- Algorithms: current algorithms are outperforming people in solving specific tasks and are developed in open source

2. **Data**, it is the material on which we will build, there are two types:
	- Structured, follows a table structure
	- Unstructured, does not follow a table structure. Ex: text, image, audio

3. **Algorithm**, it is the mathematical function that links the input data and an action

	- We are in the Narrow Artificial Intelligence context, where artificial intelligence algorithms today are for **one specific task**

	- **What do they do?** It is the general objective by which our mathematical model learns
		- **Supervised**, he performs a task that he knows the result of it and can evaluate when he is doing it right or wrong.
		Ex: predict total sales for next month
		- **Unsupervised**, perform a task that we do not know exactly the result of this
		Ex: analyze the type of clients that my company has
		- **Reinforcement learning**, you learn while doing the task
		Ex: the classic example is an agent (Super Mario) who plays a video game

	- **How do they do that?** This is how a mathematical relationship is established between the input variables X and the prediction Y. This relationship can be done in different ways, where we highlight:
	Linear / Nonlinear / Tree

	<p align="center">
	<img src="/images/models.png" width="560px"/>
	<br>
	Source: self made. Example of different ways of learning. The goal is to separate the red and blue dots. The red line is the way the algorithm learns to separate.
	</p>

	- **Objective function**, it is the function that tells us objectively how our algorithm is learning. What he wants to do is that our predictions Y ̌, are as close as possible to the real value Y. So that before a new observation the value is predicted well.

4. **Prediction:** Resulting Action 

 <p align="center">
<img src="/images/prediction.png" width="560px"/>
</p>

<h3>3. Data pipeline </h3>


1. **Research Question**, the single, clear and concise question that we want to solve with our algorithm.

2. **Data Validation + Cleaning**, validation and cleaning of the data. One of the most time consuming parts of the data scientist. We must remember that we never assume that the data is correct

3. **Exploratory Data Analysis**, understand and graph our data set. This part is crucial to validate the data and begin to extract insights from it.

4. **Modeling**, the most concrete part of machine learning where our algorithm learns the underlying relationship between the input variables

5. **Performance**, evaluation of how the predictions of my mathematical model are impacting the business reality

 <p align="center">
<img src="/images/data_pipeline.png" width="560px"/>
</p>

<h3>4. Algorithm pipeline </h3>

When we say that we train an algorithm, it means that we have an objective way of measuring its learning: the **objective function / loss function**. This function, as we have commented previously, evaluates that our predictions Y^, are as close as possible to the real value Y.

1. **Input data / Dimension**
	- The typology of the input data can be of a different nature. That is why we will need to modify some variables numerically so that our algorithm establishes relationships between them. Variables such as categorical, dates, or text fields.

2. **Ways of learning**, this point already discussed in the syllabus, is the way in which the relationship of my input data X and my variable to predict Y is established.

3. **How to train - Train / Test / Validation**
	- The way we distribute our initial data in order to ensure that the training of our algorithm is well done and is generalizable.
	- Train / Test / Validation.
		- **Train:** set of data on which we fit the model
		- **Validation:** data set used to provide an unbiased sample of how the model has been fitted
		- **Test:** final set for which the model has not seen the data. The metric on this set will tell us which model works best

	<p align="center">
	<img src="/images/splits.png" width="560px"/>
	</p>
	- **Cross validation:** separation of the dataset into different data sets to validate on

4. **Evaluation metric**
- It is the business metric on which we will evaluate the performance of our algorithm. We have to evaluate prediction failures in a product recommendation algorithm in an eCommerce differently than in the medical sector.

5. **Tools**, Open Source paradigm
- **Programming languages**, is the tool that makes the code we develop operational. In the environment of data science we will talk about two main languages, Python and R
- **Libraries** are code packages which have been developed for specific functions. In this context, when the code is open, we will talk about Open Source
- Most used libraries:
		- Numpy, algebra and calculus library
		- Pandas, library to manipulate data in DataFrame format
		- Seaborn, graphic library
		- Sickit-learn, library with implemented machine learning algorithms

6. **Actions** for the algorithm to learn better
- **Feature Engineering:** creation of new variables over the existing ones in our dataset:
- **Clever Data:** add different sources that allow us to add information and improve the predictions of our model
- **Interpretability vs Predictability**, a dichotomy that we find in Machine Learning models. Those models that make better predictions tend to be more complex, being more complex they are less interpretable 


Teaching in COVID-19 times 😷

<p align="center">
<iframe src="https://www.linkedin.com/embed/feed/update/urn:li:share:6739444048874004480" height="560" width="560" frameborder="0" allowfullscreen="" title="Publicación integrada"></iframe>
</p>