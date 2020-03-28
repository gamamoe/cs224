# cs224n-lecture02-glove

Created By: Geunho Lee
Last Edited: Mar 28, 2020 1:24 PM

# Optimization: Gradient Descent

![cs224n%20lecture02%20glove/Untitled.png](cs224n%20lecture02%20glove/Untitled.png)

![cs224n%20lecture02%20glove/Untitled%201.png](cs224n%20lecture02%20glove/Untitled%201.png)

## Stochastic Gradient Descent

![cs224n%20lecture02%20glove/Untitled%202.png](cs224n%20lecture02%20glove/Untitled%202.png)

# Word2vec: More details

- Skip-grams vs Continuous Bag of Words
- Negative sampling

![cs224n%20lecture02%20glove/Untitled%203.png](cs224n%20lecture02%20glove/Untitled%203.png)

- 1개의 Positive sample
- k개의 Negative sample
- Negative Probability = 1- Positive Probability

# GloVe

- Word2Vec: 말뭉치 전체 통계량을 사용하지 않음 (로컬 문맥)
- LSA: 말뭉치 전체 통계량 사용하지만 유사도 측정 어려움

## Why not capture co-occurrence counts directly?

![cs224n%20lecture02%20glove/Untitled%204.png](cs224n%20lecture02%20glove/Untitled%204.png)

- Vocab 사이즈가 늘어나고
- High dimensional (requires a lot of storage)
- Subsequent classification models have sparsity issues (??)

![cs224n%20lecture02%20glove/Untitled%205.png](cs224n%20lecture02%20glove/Untitled%205.png)

![cs224n%20lecture02%20glove/Untitled%206.png](cs224n%20lecture02%20glove/Untitled%206.png)

![cs224n%20lecture02%20glove/Untitled%207.png](cs224n%20lecture02%20glove/Untitled%207.png)

![cs224n%20lecture02%20glove/Untitled%208.png](cs224n%20lecture02%20glove/Untitled%208.png)

# How to evaluate word vectors?

## Intrinsic

- specific/intermediate subtask에 대해서 evaluation
- Analogy
- Correlation

![cs224n%20lecture02%20glove/Untitled%209.png](cs224n%20lecture02%20glove/Untitled%209.png)

![cs224n%20lecture02%20glove/Untitled%2010.png](cs224n%20lecture02%20glove/Untitled%2010.png)

![cs224n%20lecture02%20glove/Untitled%2011.png](cs224n%20lecture02%20glove/Untitled%2011.png)

## Extrinsic

- real task에 대해서 evaluation

![cs224n%20lecture02%20glove/Untitled%2012.png](cs224n%20lecture02%20glove/Untitled%2012.png)

# Word sense ambiguity

![cs224n%20lecture02%20glove/Untitled%2013.png](cs224n%20lecture02%20glove/Untitled%2013.png)