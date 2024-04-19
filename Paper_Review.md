## 참고
- https://aistudy9314.tistory.com/63
- https://lcyking.tistory.com/entry/%EB%85%BC%EB%AC%B8%EB%A6%AC%EB%B7%B0-Attention-is-All-you-need%EC%9D%98-%EC%9D%B4%ED%95%B4

---

## Abstract

초기에는 순환구조(recurrent)나 Encoder-Decoder 구조를 가진 RNN이나 LSTM 등의 모델들이 번역 모델에 있어서 큰 성과를 내고 있었으나,

이들은 대량의 Memory와 많은 Computation을 요구하고 있고, 문장의 길이가 길어질수록 한계를 드러내고 있다.

이 문제점을 보완하며 기존 Encoder-Decoder구조를 벗어난 Attention Mechanism만으로 구성된 Transformer 모델이 발표되었다.

이는 성능과 메모리 두 가지 측면에서 우세하였으며 현재 Transformer는 컴퓨터 비전분야에도 쓰이고 있다.

---

## Seq2Seq 모델의 등장

- 기존 RNN 모델의 가장 큰 문제점:
  RNN 모델의 경우 이전 hidden state와 현재 입력 토큰으로 예측값을 생성해내는 구조이다.
  이러한 구조는 전체 문장의 흐름을 보는 것이 아니라 이전의 hidden state만 보는 순차인 특성이기 때문에
  문장의 길이가 아주 길어지면 batch와 메모리에 한계가 생긴다
- 


