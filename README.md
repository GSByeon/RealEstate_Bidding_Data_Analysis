# RealEstate_Bidding_Data_Analysis
부동산 토지(대지) 경매 데이터 분석
---
### 분석 목적

* 경매로 올라오는 부동산 매물이 유찰이 될지 낙찰이 될지 분류한다.
* 낙찰 될 매물에 대해 낙찰가를 예측한다.

데이터 수집
---
1. 부동산 경매정보 ([http://www.auction119.co.kr/](http://www.auction119.co.kr))

2. 토지 정보 ([http://onnara.go.kr](http://onnara.go.kr))

유찰/낙찰 분류
---

해당 토지에 대한 규제 법규가 binory (0 또는 1의 값을 갖는) feature로 다수 존재하여, Naive Baysian 혹은 Decision Tree를 이용한 RandomForest를 이용한 분류가 적절하다고 판단하여 분석하였다.

낙찰가 예측
---

해당 매물에 대한 감정가는 낙찰가에 대한 의사결정에 주요한 변수임에는 틀림 없으나, 오차가 매우 크게 나타났다. 따라서 지역별로 감정가 기울기를 달리하고, 토지와 관련된 변수를 이용하여 낙찰가를 예측하였다.
