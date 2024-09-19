# AIFFEL Campus Online Code Peer Review Templete
- 코더 : 이진
- 리뷰어 : 김종환


# PRT(Peer Review Template)
- [O]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요?**
    - 문제에서 요구하는 3가지 이상의 모델과 임베딩의 분석이 진행되었다. 자체 학습한 임베딩과 비교하여 가시적인 성능향상을 보여주었다.
      ![image](https://github.com/user-attachments/assets/a89b5434-2f07-492d-9b61-1c5396327ea6)
        ![image](https://github.com/user-attachments/assets/da0c10c4-e4c4-4023-b54a-a917e1cd1c9c)
        ![image](https://github.com/user-attachments/assets/cba83aa1-13ec-4b84-9960-31e577090bee)
        ![image](https://github.com/user-attachments/assets/de7310dd-419f-4aad-8877-3dce2fc49d89)

        
- [O]  **2. 전체 코드에서 가장 핵심적이거나 가장 복잡하고 이해하기 어려운 부분에 작성된 
주석 또는 doc string을 보고 해당 코드가 잘 이해되었나요?**
    - 토큰화 과정과 단어 사전 구성 및 임베딩 과정이 NLP의 가장 핵심적인 과정이라 생각한다.
    - 이러한 부분에 어떠한 과정으로 진행을하였는지 명확하게 작성되어있었다. 
    - 
        - 중요! 잘 작성되었다고 생각되는 부분을 캡쳐해 근거로 첨부
        ![image](https://github.com/user-attachments/assets/5d73c53c-4a06-4e81-925f-8a1a0492a7c0)

- [O]  **3. 에러가 난 부분을 디버깅하여 문제를 해결한 기록을 남겼거나
새로운 시도 또는 추가 실험을 수행해봤나요?**
    -  사전 임베딩된 word2veckeydevectors를 가져오는 과정에서 오류가 지속발생하여 기존 프로젝트에서 수행한 word2vector를 가져와 프로젝트를 이어나갔다.
    -  빠른 판단과 원활한 진행 방향이었다고 생각된다. 
        - 중요! 잘 작성되었다고 생각되는 부분을 캡쳐해 근거로 첨부
        ![image](https://github.com/user-attachments/assets/2bf19c48-c93f-4df6-a466-cba1cb0a74d9)

- [O]  **4. 회고를 잘 작성했나요?**
    - 회고가 잘 작성되어있었다. 설명하는 시간에서도 추가적으로 epochs 수를 늘리는 방법과 차원에 대한 질문을 하였는데 추가적으로 수행한다는 답변을 받았다.
    - 
        - 중요! 잘 작성되었다고 생각되는 부분을 캡쳐해 근거로 첨부
        ![image](https://github.com/user-attachments/assets/1afc0d78-3b0a-4e91-9675-406d802ffaf2)

- [O]  **5. 코드가 간결하고 효율적인가요?**
    - 함수화 된 코드와 이를 이용한 효율적인 코드 진행 과정을 볼 수 있었다. 그러나 자체적인 간결 및 효율적인 코드 정리 부분이 없어 아쉬웠다고 생각된다. 
        - 중요! 잘 작성되었다고 생각되는 부분을 캡쳐해 근거로 첨부
        ![image](https://github.com/user-attachments/assets/85a6a9b2-9618-455c-86a4-25e22f600284)


# 회고(참고 링크 및 코드 개선)
```
나 또한 자연어에 대한 토큰화 임베딩 과정에서 오류가 지속되어 시간이 부족하다고 느껴졌다.. 역시나 어려운 느낌이 든다... CV나 해야지 ㅜㅜ

![image](https://github.com/user-attachments/assets/b3f572ac-cdd7-4ca2-9d37-6f58e04d2ac2)

이부분에서 워드 벡터의 차원수가 기존의 자연어 노드 5에서 진행한 임베딩 모델 가져오신 듯 합니다. word2veckeyedvector 차원수는 제가 확인할 때 100개였습니다.
그리고 단어 수도 300000만개라 10000개로는 아무리 깊이 학습한다해도 한계가 있다고 느꼈습니다...ㅠ

https://radimrehurek.com/gensim/models/keyedvectors.html -> 프로젝트에 있는 링크긴 한데 이거 보고 weight 확인할 수 있었습니다. (단어 개수와 차원수)
```
