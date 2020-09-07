# TF_ML_NLP

# 1. Introduction

이 단원은 자연어 처리에 대한 소개에 관한 내용입니다.



# 2. 자연어처리 개발 준비

여자연어처리 프로젝트에서 사용하게 될 중요한 라이브러리들을 익히는 장입니다.

- 텐서플로(Tensorflow)

  - [tf.keras.layers](./2.1.1.tf.keras.layers.ipynb)

  - [tf.data](./2.1.2%20tf.data.ipynb)

  - [tf.estimator](./2.1.3.estimator.ipynb)

- [사이킷-런(Sklearn)](./2.2.sklearn.ipynb)

- [넘파이(Numpy)](./2.4.1.numpy.ipynb)

- [판다스(Pandas)](./2.4.2.pandas.ipynb)

- [맷플롯립(Matplotlib)](./2.4.3.matplotlib.ipynb)

- [정규표현식 및 BeautifulSoup(Re & BeautifulSoup)](./2.4.4&5.re_and_beautiful_soup.ipynb)



# 3. 자연어 처리 개요

자연어 처리에 대한 개념들을 설명합니다.

- [텍스트 유사도](https://github.com/abooundev/TF_ML_NLP/blob/master/3.NLP_INTRO/3.3_텍스트_유사도.ipynb)
- [탐색적 데이터 분석(EDA)](https://github.com/abooundev/TF_ML_NLP/blob/master/3.NLP_INTRO/3.6 EDA.ipynb)



# 4. 텍스트 분류

머신러닝과 딥러닝 모델을 가지고 자연어처리를 하는 장입니다.

텍스트 분류(감정 분류 모델)를 실습을 해보고자 합니다.

이 장은 한글 데이터셋과 영어 데이터셋 두 가지로 나뉘어 실습을 하게 됩니다.

### 영어 데이터

영어 데이터는 캐글(Kaggle)의 "Bag of Words with bag of popcorns"를 가지고 실습하게 됩니다.

#### 실습 내용

- [데이터 EDA 및 전처리](./4.1.2.EDA&preprocessing.ipynb)

- [TF-IDF를 활용한 선형회귀모델](./4.1.4%20Linear%20Regression%20with%20TF-IDF.ipynb)

- [Word2Vec을 활용한 선형회귀모델](./4.1.4%20Linear%20Regression%20with%20Word2Vec.ipynb)

- [Random Forest 모델](./4.1.5%20Random%20Forest.ipynb)

- [RNN 모델](./4.1.6%20RNN%20Classification.ipynb)

- [CNN 모델](./4.1.7.CNN_Classification.ipynb)


### 한글 데이터

한글 데이터는 네이버 영화 리뷰 데이터를 가지고 실습하게 됩니다.

#### 실습 내용

- [데이터 EDA 및 전처리](./4.2.2.EDA&preprocessing.ipynb)

- [모델링](./4.2.3.Korea%20Sentiment%20Modeling.ipynb)



# 5. 텍스트 유사도

텍스트 유사도 모델을 만들어 각 문장 간의 거리가 어떻게 되는지 실습해보고자 합니다.

이 장은 영어 데이터셋만을 가지고 실습을 하게 됩니다.

## 데이터

데이터는 캐글(Kaggle)의 "Quora Question Pairs"를 가지고 실습하게 됩니다.

### 실습 내용

- [데이터 EDA 및 전처리](./5.2.EDA&preprocessing.ipynb)

- [XG 부스팅을 활용한 유사도 모델](./5.3.1.XGboost.ipynb)

- [CNN을 활용한 유사도 모델](./5.3.2.Quora_CNN.ipynb)

- [MaLSTM을 활용한 유사도 모델](./5.3.3_Quora_LSTM.ipynb)

## 부록

- [개선된 MaLSTM 모델](./Appendix/5.3.3_Quora_LSTM_Appendix.ipynb)



## QuoraQuestionPairs (Link 정리 해서 공유)

* [QuoraQuestionPairs](https://github.com/changwookjun/Kaggle/tree/master/QuoraQuestionPairs)   
  + [Understanding LSTM](https://github.com/changwookjun/Kaggle/blob/master/QuoraQuestionPairs/Understanding%20LSTM%20Networks.ipynb)  
  + [History Word Vectors](https://github.com/changwookjun/Kaggle/blob/master/QuoraQuestionPairs/The%20Amazing%20Power%20Of%20Word%20Vectors.ipynb)  
  + [QuoraQuestionPairsAnalysis.ipynb](https://github.com/changwookjun/Kaggle/blob/master/QuoraQuestionPairs/QuoraQuestionPairsAnalysis.ipynb)  
  + [Kaggle Quora Question Pairs MaLSTM Paper.ipynb](https://github.com/changwookjun/Kaggle/blob/master/QuoraQuestionPairs/Kaggle%20Quora%20Question%20Pairs%20MaLSTM%20Paper.ipynb)    
  + [Kaggle Quora Question Pairs MaLSTM Source.ipynb](https://github.com/changwookjun/Kaggle/blob/master/QuoraQuestionPairs/Kaggle%20Quora%20Question%20Pairs%20MaLSTM%20Source.ipynb)  



# 6. 챗봇 만들기

자연어 생성 (Natural Language Generation)을 다뤄보도록 합시다.

Seq2Seq (Sequence to Sequence) 모델을 가지고 챗봇을 만들게 됩니다.

모델은 송영숙님이 제공해주신 "챗봇 데이터셋"을 가지고 다루게 됩니다.

데이터셋에 대한 분석은 다음 페이지에서 확인할 수 있습니다.

- [챗봇 데이터 EDA](./6.2.EDA.ipynb)



## 챗봇 모델

- [RNN 기반의 Seq2Seq 모델](./6.3%20seq2seq)

- [Transformer 기반의 Seq2Seq 모델](./6.4%20transformer)


## 부록

보다 좋은 성능으로 활용할 수 있는 챗봇 모델을 제공하기 위해 발전된 모델을 구현해 뒀습니다.

- [Attention Based RNN Seq2Seq 모델](./Appendix)

- [개선된 Transformer 기반 Seq2Seq 모델](