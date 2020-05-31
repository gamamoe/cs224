# cs224n-rnnlm

Created By: Geunho Lee
Last Edited: May 31, 2020 2:13 PM

# Language Modelling & RNN

## Language Modelling

어떤 단어가 다음에 올 지 예측하는 태스크

![cs224n%20rnnlm/Untitled.png](cs224n%20rnnlm/Untitled.png)

이런 작업을 하는 것들을 **Language Model** 이라고 함

활용 Applications - Autocomplete

![cs224n%20rnnlm/Untitled%201.png](cs224n%20rnnlm/Untitled%201.png)

![cs224n%20rnnlm/Untitled%202.png](cs224n%20rnnlm/Untitled%202.png)

### n-gram Language Models

![cs224n%20rnnlm/Untitled%203.png](cs224n%20rnnlm/Untitled%203.png)

Markov assumption 활용해서 이전 n-1에만 depend 한다는 가정

결국 큰 코퍼스 셋에서 count 세서 probability 계산함

![cs224n%20rnnlm/Untitled%204.png](cs224n%20rnnlm/Untitled%204.png)

![cs224n%20rnnlm/Untitled%205.png](cs224n%20rnnlm/Untitled%205.png)

![cs224n%20rnnlm/Untitled%206.png](cs224n%20rnnlm/Untitled%206.png)

- Smoothing → 계산하려는 n-gram 형태가 없는 경우
- Backoff → 이전 context (n-1)-gram이 존재하지 않은 경우

![cs224n%20rnnlm/Untitled%207.png](cs224n%20rnnlm/Untitled%207.png)

Language Model을 이용해서 Text generation이 가능함

![cs224n%20rnnlm/Untitled%208.png](cs224n%20rnnlm/Untitled%208.png)

### Neural Language Model

![cs224n%20rnnlm/Untitled%209.png](cs224n%20rnnlm/Untitled%209.png)

## Recurrent Neural Networks (RNN)

![cs224n%20rnnlm/Untitled%2010.png](cs224n%20rnnlm/Untitled%2010.png)

![cs224n%20rnnlm/Untitled%2011.png](cs224n%20rnnlm/Untitled%2011.png)

### Training RNN

![cs224n%20rnnlm/Untitled%2012.png](cs224n%20rnnlm/Untitled%2012.png)

![cs224n%20rnnlm/Untitled%2013.png](cs224n%20rnnlm/Untitled%2013.png)

### Evaluating Language Models

![cs224n%20rnnlm/Untitled%2014.png](cs224n%20rnnlm/Untitled%2014.png)

![cs224n%20rnnlm/Untitled%2015.png](cs224n%20rnnlm/Untitled%2015.png)

### Summary

- Language Model: 다음 단어를 예측하는 시스템
- RNN: 인공신경망의 한 종류
    - 길이 제한 없는 sequential 입력
    - 각 스텝마다 동일한 웨이트 (Wh)
    - 각 스텝마다 필요하면 output 확률 계산 가능
- RNN ≠ Language Model