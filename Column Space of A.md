# Column Space of A

Created By: Geunho Lee
Last Edited: Mar 14, 2020 1:37 PM

### 행렬 연산을 좀 다르게 생각해보자

$$\begin{pmatrix} 2 & 1 & 3 \\ 3 & 1 & 4 \\ 5 & 7 & 12 \end{pmatrix}\begin{pmatrix} x_1 \\ x_2 \\ x_3 \end{pmatrix}=x_1\begin{pmatrix} 2 \\ 3 \\ 5 \end{pmatrix}+x_2\begin{pmatrix} 1 \\ 1 \\ 7 \end{pmatrix}+x_3\begin{pmatrix} 3 \\  4\\ 12 \end{pmatrix}$$

1. 우리가 하던대로 내적 연산 반복 (Row x Col)
2. **Column vector from A의 선형 결합**

### 열공간 (Column Space)

$$\begin{pmatrix} 2 & 1 & 3 \\ 3 & 1 & 4 \\ 5 & 7 & 12 \end{pmatrix}$$

- 위 매트릭스는 열공간 어떻게 됨?
- 전체 R3? → No, Plane임 ㅋㅋ
- Independent 개념 얘기하면서 3번째 Column vector가 1, 2번째의 합

$$\begin{pmatrix} 1 & 3 & 8 \\ 1 & 3 & 8 \\ 1 & 3 & 8 \end{pmatrix}$$

- 이건? → C(A) = line
- 바꿔 얘기하면 rank(A) = 1

![Column%20Space%20of%20A/Untitled.png](Column%20Space%20of%20A/Untitled.png)

### First Matrix Factorization

$$\begin{pmatrix} 2 & 1 & 3 \\ 3 & 1 & 4 \\ 5 & 7 & 12 \end{pmatrix}=\begin{pmatrix} 2 & 1 \\ 3 & 1 \\ 5 & 7 \end{pmatrix}\begin{pmatrix} 1 & 0 & 1 \\ 0 & 1 & 1 \end{pmatrix}$$

- Independent Column Vector
- Row (사실 Reduced echelon form 임 ㅋ)
- Column rank = Row rank = 2

### 계속 강조하는게 열벡터로 생각하라는거 강조