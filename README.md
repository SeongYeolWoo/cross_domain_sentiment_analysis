# cross_domain_sentiment_analysis
NSMC데이터로 모델 학습 후, Steam 게임리뷰 데이터 및 네이버 쇼핑데이터 감정 분석 성능 확인

기술스택: python, konlpy, tensorflow

구현환경: Google Colab

데이터셋: NSMC, Steam Review Dataset, Naver Shopping dataset(출처: https://github.com/songys/AwesomeKorean_Data)

실험과정
데이터 전처리: 한글, 공백 빼고 제거, 빈데이터 제거, 불용어 제거, 시퀀스로 변환, 최대 길이 조정, train:test(8:2) 나눔.

GRU, LSTM, RNN 모델 구현하여 학습.

Cross Domain 성능
# Steam Data


GRU: Acc: 0.70, loss: 0.62

LSTM: Acc: 0.71, loss: 0.60

RNN: ACC: 0.68, loss: 0.68

&nbsp;
# Naver Shopping Review Data

GRU: Acc: 0.77, loss: 0.48

LSTM: Acc: 0.76, loss: 0.50

RNN: ACC: 0.76, loss: 0.50



