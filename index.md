---
title       : Embeddings
subtitle    : The future of NLP?
author      : Rob Mealey
job         : Mostly Bad Java, Nowadays
framework   : revealjs # {io2012, html5slides, shower, dzslides, ...}
revealjs    : {theme: sky, transition: concave} ## white, sky, beige, simple, serif, blood, night, moon
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
--- &vertical

# Embeddings
## the Future of NLP?
### Rob Mealey
### Mostly Bad Java, Nowadays

--- &vertical

## So what are we talking about?

***

##### EMBEDDINGS 

***

#### word embeddings...

***

### phrase embeddings...

***

## document embeddings...

***

## thought embeddings...

***

# MOAR IMBEDDINGS!

--- &vertical

## Ok but wtf?

***

## techniques for learning 
## "distributed representations"
## of words, phrases, whatever

***

## representations are
## vectors of numbers

***

!['msoft'](assets/img/msoft.jpg)

***

## GEOMETRIC relationships

***

# Meaning? Similarity? 

***

## Unsupervised 
## (no labels required)
### But lots of raw data is required

--- &vertical

## What EMBEDDINGS can do

*** 

## word/phrase/document similarity

***

<iframe width=800 height=600 src="http://irsrv2.cs.biu.ac.il:9998/?word=eisenhower"></iframe>
<a href="http://irsrv2.cs.biu.ac.il:9998/">Omer Levy Demo</a>

***

## Analogy!

***

!['similarity'](assets/img/recommender.jpg)

***

# not enough
# for you?

***

<img src="assets/img/city_zip.jpg" height=600/>

***

<img src="assets/img/company_ceo.jpg" height=600/>

***

<img src="assets/img/comparative_superlative.jpg" height=600/>

--- 

<a href="http://www.ghostweather.com/files/word2vecpride/">Another Cool Demo</a>

--- &vertical

## What "embeddings" are NOT

***

# Deep Learning

***

- Two most popular implementations:
    - word2vec, Google 2013 
    - GloVe, Stanford 2014)

***

### both implementation of word2vec 
### are SHALLOW neural networks.

***

### GloVe is a highfalutin 
### log-linear model. 

***

## Google just published successor to word2vec: "Swivel"
### Feb 6, 2016
<a href="http://arxiv.org/pdf/1602.02215v1.pdf">Swivel Paper</a>

***

> Swivel uses stochastic gradient descent to perform a weighted 
> approximate matrix factorization, ultimately arriving at embeddings 
> that reconstruct the point-wise mutual information (PMI) between
> each row and column feature. Swivel uses a piecewise loss function
> to differentiate between observed and unobserved cooccurrences.

***

# nary a "neural" to be found

***

### deep neural networks,
### especially in NLP applications,
### usually have embedding layers.

--- &vertical

## What "embeddings" ARE

***

# BIG DATA

***

>Tomas Mikolov even told me that the whole idea behind word2vec was to demonstrate that you can get better word representations if you trade the model's complexity for efficiency, i.e. the ability to learn from much bigger datasets. 
<a href=https://www.quora.com/How-does-word2vec-work>Omer Levy on Quora</a>

***

!['hype'](assets/img/hype_cycle.jpg)

--- &vertical

## A peek under the hood 

***

### implicit decomposition 
### of massive context matrix

***

<iframe width=1200 height=600 seamless src="https://en.wikipedia.org/wiki/Pointwise_mutual_information"></iframe>

***

<iframe width=1200 height=600 seamless src="https://en.wikipedia.org/wiki/Pointwise_mutual_information#Applications"></iframe>

--- &vertical

## What "embeddings" can do
# FOR US

***

## automatable 
## customer-specific
## feature engineering

***

## similarity querying 
## that gets better 
## the more data we get

***

## actors, entities, organizations 

*** 

<iframe width=800 height=600 src="http://irsrv2.cs.biu.ac.il:9998/?word=madoff"></iframe>
<a href="http://irsrv2.cs.biu.ac.il:9998/">Omer Levy Demo</a>

***

# My point: 
- our customers pump a lot of unlabeled data through our system
- more than enough to train models for each with "valid" geometries

*** 

## all sorts of interesting, unsupervised things.

***

- paragraph vectors
- document vectors, 
- "thought" vectors,
- entity vectors,
- on and on

***

### If you want to sit here all afternoon,
### I'll happily keep talking.

---

<iframe width=800 height=600 src="http://irsrv2.cs.biu.ac.il:9998/?word=stalin"></iframe>
<a href="http://irsrv2.cs.biu.ac.il:9998/">Omer Levy Demo</a>

--- &vertical

# Further reading and tools

*** 

### word2vec 
- https://code.google.com/archive/p/word2vec/

*** 

### GloVe
- http://nlp.stanford.edu/projects/glove/

*** 

### gensim (Radim Rehurek)
- http://radimrehurek.com/gensim/
- http://rare-technologies.com/word2vec-tutorial/
- http://rare-technologies.com/making-sense-of-word2vec/
- http://rare-technologies.com/doc2vec-tutorial/

*** 

### Yoav Goldberg and Omer Levy
- https://levyomer.wordpress.com/
- http://www.cs.bgu.ac.il/~yoavg/publications/

*** 

### interesting applications:
- http://bookworm.benschmidt.org/posts/2015-10-25-Word-Embeddings.html
- http://bookworm.benschmidt.org/posts/2015-10-30-rejecting-the-gender-binary.html
- http://instagram-engineering.tumblr.com/post/117889701472/emojineering-part-1-machine-learning-for-emoji

---

Questions?


