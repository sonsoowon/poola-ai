### 1. 컵 분류 및 앞중심 높이 너비 추출 모델
2020-08 ~ 2020-12

- **[학습 데이터 전처리](https://github.com/sonsoowon/poola-ai/blob/master/Image_Preprocess.ipynb)**

  학습에 불필요한 요소(색, 무늬, 그림자 등)를 제거하기 위해 이미지의 윤곽선을 추출하고 크기를 동일하게 조정했습니다.
  ![윤곽선1](https://user-images.githubusercontent.com/55790232/195974520-1c3ef7d8-4666-413e-a200-0b6e1fd50559.png)
  ![윤곽선2](https://user-images.githubusercontent.com/55790232/195974517-94ce7220-2f59-4636-ae6c-76d0b956075f.png)
  
- 컵 분류 모델

  **[단순한 구조의 모델]**(https://github.com/sonsoowon/poola-ai/blob/master/Simple_Cup_Classification.ipynb) 부터 **[데이터 증강 및 사전학습을 진행한 모델]**(https://github.com/sonsoowon/poola-ai/blob/master/Complex_Cup_Classification.ipynb) 까지 시도하며 분류 정확도가 높은 모델을 탐색했습니다.

- **[앞중심 높이 너비 추출 모델](https://github.com/sonsoowon/poola-ai/blob/master/Keypoint_Prediction.ipynb)**

  원하는 정보를 계산하는데에 필요한 지점(Keypoint)만 라벨링하여 학습과 예측을 진행했습니다.
  
  ![keypoint1](https://user-images.githubusercontent.com/55790232/195974522-641f281f-6289-4f13-bde3-70566d4ba732.png){: width="100" height="100"}
  ![keypoint2](https://user-images.githubusercontent.com/55790232/195974524-c79d3e21-ed0c-4fd5-810b-c541939f63dc.png)


### [2. 사용자-제품 매칭률(Fit Score) 계산 알고리즘](https://github.com/sonsoowon/poola-ai/blob/master/Fit_Score_Algorithm.ipynb)
2021-01 ~ 2021-02


![아](https://img.shields.io/badge/Notion-%23000000.svg?style=for-the-badge&logo=notion&logoColor=white) [Fit Score Algorithm Manual](https://glaze-breadfruit-31f.notion.site/Fit-Score-Algorithm-Manual-8eda341793f44a71a4814a4a3e1095ec)

- 사용자의 체형과 제품의 특성을 비교 분석해 사용자가 제품을 편안하게 착용할 확률을 수치로 나타냈습니다.
- 착용감에 영향을 주는 제품의 각 요소에 가중치를 임의로 부여하고 계산했기에, 충분한 검증이 이뤄지지 않았다는 한계가 있습니다.

![fitscore](https://user-images.githubusercontent.com/55790232/195974799-6c9ffbe5-39b5-418a-896c-232d90d0df03.png){: width="100%"}

### [3. Amazon Personalize를 활용한 추천 시스템](https://glaze-breadfruit-31f.notion.site/Amazon-Personalize-Manual-84985f2ad8854491879ef25c89ae6877)
2021-06 ~ 2021-07


매칭률 계산 알고리즘의 문제점을 해결하기위해 2차 MVP 이후 추천 시스템 도입을 시도했습니다.

1. [추천 시스템 기획](https://glaze-breadfruit-31f.notion.site/W4-fbe22e9ab78244f89e69443ed2ee8d39)
2. [Amazon Personalize 입력 데이터 분석](https://glaze-breadfruit-31f.notion.site/Amazon-Personalize-Input-W5-f1cf3d99486d45e59ed27c7fd20d4443)
3. [Amazon Personalize 시범 적용](https://glaze-breadfruit-31f.notion.site/Amazon-Personalize-W6-a28cab2fc6d442b9b5072f60e35c7e30)
