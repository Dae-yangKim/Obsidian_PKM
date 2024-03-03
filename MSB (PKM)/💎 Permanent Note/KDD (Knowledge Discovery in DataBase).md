
---
- author : Daeyang-Kim
- created : 2024-02-07 21:02
- last_updated : 2024-02-07 21:02
- tags : #Permanent #DataScience #BigData
---

# KDD (Knowledge Discovery in DataBase)

## *주제*

데이터 분석 방법론 중 하나인 KDD에 대해서 정리

## *나의 생각*

![[KDD.webp]]

KDD는 <mark>데이터 마이닝 기술과 데이터베이스를 중심으로 해서 , 성찰을 얻어내는 과정을 정리한 것이다.</mark>

- 1. Selection
		DB에서 분석에 필요한 데이터를 선택하는 단계.
- 2. Preprocessing
		데이터셋에 포함되어 있는 결측값이나 , 이상치 , 노이즈를 찾아내서 필요에 따라서 적절한 방법으로 처리를 하는 단계.
- 3. Transformation
		Preprocessing 단계에서 정제한 데이터를 여러 기법을 사용하여 변환한다.
		예를 들면
			- 데이터 차원의 수를 줄인다.
			- 목적에 맞게 새로운 특성을 만들어내는 Feature Engineering
			- 스케일링이나 Binning 등등
- 4. Data Mining
		Data Mining 알고리즘을 이용하여 , 데이터마이닝을 실행한다.
- 5. Evaluation
		데이터마이닝 수행 결과를 , 해석과 평가를 시행한다.

이와 같이 구성이 된다.

---

## *Link*

- [[💎 Permanent Note/데이터 분석 방법론|데이터 분석 방법론]]