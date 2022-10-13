# Probabilistic Language Model의 한계

## 문장 전체의 확률을 계산하기가 어려움
- 계산하려는 문장이 corpus에 존재하지 않을 확률이 높음
- Markov Assumption: 문장 중 직전 n개와의 확률만 계산하는 것이 문장 전체의 확률을 근사한다고 가정

## 계산이 복잡함
- 로그를 취해서 계산
  - 곱셈을 덧셈으로 계산할 수 있어 유리

## Overfitting 및 Generalization 문제
- Devision by zero
  - Smoothing 기법 사용
    - Laplace Smoothing
      - 모든 count에 1을 더함
      - 1 대신 k를 더하는 방식으로 general하게 사용

# Speeling Correction

## Non word Errors
- Detection
  - Any word not in a dictionary
- Correction
  - Generate candidates and choose one with
    - Shortest weighted edit distance
    - Highest noisy channel probability
    - 
## Real word Errors
- Detection
  - For each word
- Correction
  - Generate candidates but include original word, and choose one with
    - noisy
    - Classifier

## Noisy Channel
- w = argmaxP(w|x) = P(x|w)P(w)

## Bigram Model

# Text Classification

## Supervised ML
- Naive Bayes
- Logistic regression
- SVM
- kNN

# Naive Bayes
- P(c|W) = P(c) * ㅠP(w|c)
- 이때 Laplace Smoothing 사용
