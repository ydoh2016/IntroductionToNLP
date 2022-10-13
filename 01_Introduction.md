# Introduction

## 첫 NLP 모델
ELIZA(1966)
- Pattern Matching 방법 사용

## NLP Applications
- Spam detection
- POS tagging
- NER tagging
- Sentiment analysis
- Coreference resolution
- WSD
- Parsing sentence
- Translation
- Information extraction
- QA
- Paraphrase
- Summarizatoin
- Dialog
- ...

## NLP 의 당면 과제
- Non standard English
- Ethics
- Idioms
- Neologisms
- World Knowledge
- Tricky entity names
- ...

## 코스 간 참고 링크
- [Stanford NLP Book](https://nlp.stanford.edu/fsnlp/promo/)
- [Stanford IR Book](https://nlp.stanford.edu/IR-book/)
- [Berkeley AI Course](http://ai.berkeley.edu/home.html)

# Before ML NLP

## Rule-based Approaches
- [Regular Expressions](https://en.wikipedia.org/wiki/Regular_expression)

# Metric

## Precision
- accuracy(fixing false positives)
- 틀려야 할 것을 맞추는 것(잘못 맞춤)
- reluctant하게 판단한다면 precision 올라감
- P = tp / (tp + fp)

## Recall
- coverage(fixing false negatives)
- 맞춰야 할 것을 틀리는것(잘못 틀림)
- promiscuous하게 판단한다면recall 올라감
-  R = tp / (tp + fn)

## F score
- Weighted 조화 평균(낮은 점수에 가까운 보수적인 평균)을 사용
- F = 1 / ((alpha) / P + (1 - alpha) / R) = (beta^2 + 1)PR / (beta^2(P) + R) (when beta = ((-alpha + 1) / alpha)^(1/2))

# Lexical Similarity

## String Pattern Matching Task
- Spell correction
- Compuational biology
- Machine Translation
- Information Extraction
- Speech Recognition
- ...

## [Edit Distance(Levenshtein Distance)](https://lovit.github.io/nlp/2018/08/28/levenshtein_hangle/)
- minimum number of operations in editing a word into another word
- Example : Levenshtein(INTENTION -> EXECUTION) = 8
- Confusion matrix를 이용해 weight 줄 수 있음
