# cs224n-lecture04-backprop

Created By: Geunho Lee
Last Edited: Apr 26, 2020 1:42 PM

## Retraining word vectors

![cs224n%20lecture04%20backprop/Untitled.png](cs224n%20lecture04%20backprop/Untitled.png)

![cs224n%20lecture04%20backprop/Untitled%201.png](cs224n%20lecture04%20backprop/Untitled%201.png)

![cs224n%20lecture04%20backprop/Untitled%202.png](cs224n%20lecture04%20backprop/Untitled%202.png)

## Backpropagation

- 체인룰을 활용해서 미분
- Upstream layer에서 계산된 derivative 재사용

### Forward propagation (expression evaluation)

![cs224n%20lecture04%20backprop/Untitled%203.png](cs224n%20lecture04%20backprop/Untitled%203.png)

### Backpropagation

![cs224n%20lecture04%20backprop/Untitled%204.png](cs224n%20lecture04%20backprop/Untitled%204.png)

![cs224n%20lecture04%20backprop/Untitled%205.png](cs224n%20lecture04%20backprop/Untitled%205.png)

- Upstream gradient * Local gradient = Downstream gradient 계속 반복

![cs224n%20lecture04%20backprop/Untitled%206.png](cs224n%20lecture04%20backprop/Untitled%206.png)

![cs224n%20lecture04%20backprop/Untitled%207.png](cs224n%20lecture04%20backprop/Untitled%207.png)

![cs224n%20lecture04%20backprop/Untitled%208.png](cs224n%20lecture04%20backprop/Untitled%208.png)

![cs224n%20lecture04%20backprop/Untitled%209.png](cs224n%20lecture04%20backprop/Untitled%209.png)

- 재사용 가능한 gradient는 재사용한다

## Training tips

### Regularization

![cs224n%20lecture04%20backprop/Untitled%2010.png](cs224n%20lecture04%20backprop/Untitled%2010.png)

### Vectoriazation

![cs224n%20lecture04%20backprop/Untitled%2011.png](cs224n%20lecture04%20backprop/Untitled%2011.png)

### Non-linearities

![cs224n%20lecture04%20backprop/Untitled%2012.png](cs224n%20lecture04%20backprop/Untitled%2012.png)

### Parameter initialization

- Xavier initialization

### Optimizers

- Start with Adam

### Learning rates

![cs224n%20lecture04%20backprop/Untitled%2013.png](cs224n%20lecture04%20backprop/Untitled%2013.png)