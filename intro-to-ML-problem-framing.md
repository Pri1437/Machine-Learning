<div id="table-of-contents">
<h2>Table of Contents</h2>
<div id="text-table-of-contents">
<ul>
<li><a href="#sec-1">1. Introduction to machine learning problem framing</a>
<ul>
<li><a href="#sec-1-1">1.1. Supervised learning</a></li>
<li><a href="#sec-1-2">1.2. Unsupervised learning</a></li>
<li><a href="#sec-1-3">1.3. Reinforcement learning</a></li>
<li><a href="#sec-1-4">1.4. Types of ML problems</a></li>
</ul>
</li>
<li><a href="#sec-2">2. The ML mindset</a></li>
</ul>
</div>
</div>

# Introduction to machine learning problem framing<a id="sec-1" name="sec-1"></a>

Notes on how to frame problems so they can be solved by ML

features &rarr; properties/attributes that you use while training a model.

The General cycle in solving problem using ML is,
-   Frame a ML problem and propose a solution
-   Gather data and construct dataset
-   preprocessing of data like cleaning, feature extraction, splitting of dataset
-   Create a model and train it
-   Test the model using test set and obtain predictions

Here we are focusing on framing a ML problem and proposing a solution:
-   Frame problem
-   Decide what features in data to use
-   decide where to get data from
-   What outputs should be predict

ML &rarr; it training a piece of software (model) and making useful predictions on dataset.
-   Can be used to predicted unseen data too.

ML problems lie on a spectrum b/w supervised and unsupervised learning.

## Supervised learning<a id="sec-1-1" name="sec-1-1"></a>

Here we train a model using labeled data, i.e. the training data has both input and correct output.
-   label is the correct output(answer) for a given training example. (single label)
-   Feature is the property or description
-   Model &rarr; relationship b/w features and label

Supervised learning finds a mathematical function between features and label.

## Unsupervised learning<a id="sec-1-2" name="sec-1-2"></a>

Main goal is to find meaniful patterns in data. The machine has to make inferences from unlabeled data.
-   Sometimes model can find unexpected patterns in the data like bias etc.
-   When a new data point comes we can categorize it into known cluster.

sometimes our machine can find patterns that can be stereotypes or bias:
-   Automation bias
-   confirmation bias
-   etc

Q) what happens if the data point doesn't resemble known clusters?

For unlabeled data supervised learning algo won't work.

Even if we are able to find clusters we can't exactly give them a particular name as we don't know the labels

Clustering is not only type of unsupervised learning

## Reinforcement learning<a id="sec-1-3" name="sec-1-3"></a>

Reinforcement learning is a type machine learing that the machine (agent) learns feedback and here don't provide labels.

RL:
-   Agent
-   Env

Agent takes decisions on basis of increasing its reward.

Compare RL and supervised learning:
-   Creating a good reward function is really difficult.
-   RL can give you unpredictable result and less stable
-   In RL, it is difficult to create the env req so agent can interact

## Types of ML problems<a id="sec-1-4" name="sec-1-4"></a>

-   Supervised
    -   Classification
    -   Regression
-   Unsupervised
    -   Clustering
-   Other learning
    -   Association rule learning &rarr; infer something based on association patterns
        1.  Ex: if you buy pizza base you might buy pizza too.
    -   Structured output (supervised), complex labeled data is needed
    -   Ranking, try to rank different stuff

# The ML mindset<a id="sec-2" name="sec-2"></a>

-   In ML, you look at a problem different compared to developing a program or software, i.e. it becomes more of finding out the right model suitable for a problem which involves experimentation and statistics
-   Working with ML is like working with a scientific hypothesis, where you need to experiment to find the best hypothesis for the problem.
-   Now in ML, models understand data differently i.e. we have to encode data in some form that may not be understandable for humans.
-   Figuring out what a model is doing can be really tough becuz an issue can be caused due to improper training, or unexpected interpretation of data.
-   In software development, we know how the code will behave for a situation but in machine learning whatever behaviour we expect may not be always whatever actually occurs.
-   Steps in the ML process are:
    -   Set a research goal (problem to solve)
    -   Create your assumption/hypothesis
    -   Collect relevant data
    -   Test your hypothesis on the collected data
    -   Analyze the results
    -   Make conclusion about your hypothesis
    -   Refine your hypothesis and experiment again.