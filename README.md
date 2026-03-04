# 01
- Pretraining을 통한 바닥부터 파이토치로 직접 만든 간단한 LLM
- GELU() 활성함수를 사용했음.
- 영어 책(tiny_shakespeare.txt)을 데이터셋으로 활용.

- <img width="400" alt="스크린샷 2026-03-04 오후 1 22 58" src="https://github.com/user-attachments/assets/b6f7b3e2-352c-491a-ae38-ee86108d5101" />

``` Text
Tokens seen: 4096
Epoch: 1, Loss: 4.677962420294094
Tokens seen: 4100096
Epoch: 2, Loss: 2.2980352689995582
Epoch: 3, Loss: 0.7514405264048626
Tokens seen: 8196096
Epoch: 4, Loss: 0.42986429729320447
Epoch: 5, Loss: 0.3505597306149347
Tokens seen: 12292096
Epoch: 6, Loss: 0.31619176476259264
```
# 02
- 카카오 나노 2.1b base모델을 허깅페이스에서 받아, Full-Fine-Tuning 했음.
- jmcustomdata.txt로 간단한 데이터셋 제작 
  - 매우 간단한 데이터셋이라 원본 회손을 방지하기위해 lr=0.00001 로 매우 작게 하였음.
- epoch를 10으로 설정했음

<img width="400" alt="스크린샷 2026-03-04 오후 1 29 09" src="https://github.com/user-attachments/assets/5eb30bed-a5c3-4d02-b70d-d07f58c54bf9" />

