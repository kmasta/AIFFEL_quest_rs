# AIFFEL Campus Online Code Peer Review Templete
- 코더 : 강희봉
- 리뷰어 : 이현재


# PRT(Peer Review Template)
- [x]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요?**
    -  BERT 모델을 로드하고, NSMC 데이터셋으로 파인튜닝한 후, 학습 과정(loss, accuracy)을 시각화하고, 최종적으로 테스트 데이터셋에 대한 NSP, MLM 태스크 평가 결과를 제시했습니다.
        - ![image](https://github.com/user-attachments/assets/fd3bbead-bb4a-4b5c-b1c1-512d65370d83)
        - ![image](https://github.com/user-attachments/assets/46c3a738-62bf-487e-8749-687fc2344adc)


    
- [ ]  **2. 전체 코드에서 가장 핵심적이거나 가장 복잡하고 이해하기 어려운 부분에 작성된 
주석 또는 doc string을 보고 해당 코드가 잘 이해되었나요?**
    - 해당 코드 블럭을 왜 핵심적이라고 생각하는지 확인
    - 해당 코드 블럭에 doc string/annotation이 달려 있는지 확인
    - 해당 코드의 기능, 존재 이유, 작동 원리 등을 기술했는지 확인
    - 주석을 보고 코드 이해가 잘 되었는지 확인
        - 중요! 잘 작성되었다고 생각되는 부분을 캡쳐해 근거로 첨부
        
- [x]  **3. 에러가 난 부분을 디버깅하여 문제를 해결한 기록을 남겼거나
새로운 시도 또는 추가 실험을 수행해봤나요?**
    - 노트북 내에 명시적인 에러 해결 과정 기록은 보이지 않으나 회고 부분에 에러 해결 과정을 간략하게 작성했습니다.
        - ![image](https://github.com/user-attachments/assets/2d152d1e-bba7-40e3-9e7b-dcc7b1ff6be8)


        
- [x]  **4. 회고를 잘 작성했나요?**
    - 결과분석과 함께 회고 부분을 잘 작성해주셨습니다.
        - ![image](https://github.com/user-attachments/assets/35095046-7025-4911-a425-93416f46d370)

        
- [ ]  **5. 코드가 간결하고 효율적인가요?**
    - 파이썬 스타일 가이드 (PEP8) 를 준수하였는지 확인
    - 코드 중복을 최소화하고 범용적으로 사용할 수 있도록 함수화/모듈화했는지 확인
        - 중요! 잘 작성되었다고 생각되는 부분을 캡쳐해 근거로 첨부


# 회고(참고 링크 및 코드 개선)
```
저는 데이터 샘플을 128000개까지만 사용했는데, 데이터 전부 사용하셔서 학습시킨 결과가 인상적이었습니다. 비록 시간은 3배가 더 걸렸지만, 확실히 accuracy 측면에서 더 나은 퍼포먼스를 보이는 듯합니다.
비록 mlm accuracy는 0.3으로 0.2가 나온 제 결과와 큰 차이는 없었지만, nsp accuracy는 0.77로 제 결과보다 더 나은 모습이었습니다.
정량적인 지표보다 mlm 태스크에서 예측값들이 제 결과보다 더 자연스러워서 인상적이었습니다.
mlm은 태스크 특성 상 accuracy가 높게 나오기가 매우 힘든데, accuracy 0.1 차이가 이렇게 크다는 것을 느꼈습니다.
![image](https://github.com/user-attachments/assets/0809cd45-f787-45b0-9dd2-a1f54e4da6ff)

```
