cs224n-lecture01-wordvecs1
=============

WordNet
-------------
사람이 손으로 단어들의 관계(동의어, 품사, 상의어, 하의어)들을 입력하여 만듦
* Pros
    - 하나의 좋은 자료가 될 수 있다. ex) 확실한 synonym 찾기

* Cons
    - 단어의 뉘양스 고려 X (miss a lot of nuance)
    - discrete
    - human labor (up-to-date 힘듦, incomplete)
    - **word similarity 계산 불가**
    
Traditional One-Hot Words Representation
------------- 
```python
word_home = [0,0,0,0,1,0,0,...,0]
word_house = [0,1,0,0,0,0,0,...,0]
```
* Cons
    - word size 만큼의 dimension 필요
    - **word similarity 계산 불가 (orthogonal)**

Word2vec
------------- 
*  Pros
    - 단어의 백터를 **주변단어의 distribution**으로 표현 (distributional semantics)
    - 더 적은 dimension에 표현
    - **word similarity 계산 가능**
             
*  loss
    - t = center, m = window-size
<img src="/w2v.png" width="700px" title="w2v loss" alt="w2vloss"></img>

*  prediction function
    - P(Wt+j|Wt)를 simplify: 각 단어가 2가지 백터(u,v)를 가짐
    - 목적: maximize prediction(인접한 단어들이 비슷한 공간에놓기)
    
<img src="/w2v_prediction.png" width="800px" title="w2v pred" alt="w2vpred"></img>

*  Optimization
prediction function을 미분해서 u,v의 방향을 알아보자

    - slope of vc
    
    
<img src="/softmax1.jpg" width="500px" title="" alt=""></img>

<img src="/softmax2.jpg" width="500px" title="" alt=""></img>
