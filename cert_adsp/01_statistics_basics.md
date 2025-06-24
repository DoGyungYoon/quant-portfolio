# 📊 ADSP 통계 기초 정리

---

## 1. 중심 경향성 (Measures of Central Tendency)

- 평균 (Mean):  
  $ \bar{x} = \frac{1}{n} \sum x_i $

- 중앙값 (Median)

- 최빈값 (Mode)

---

## 2. 산포도 (Measures of Dispersion)

- 분산 (Variance):  
  $ \sigma^2 = \frac{1}{n} \sum (x_i - \mu)^2 $

- 표본분산 (Sample Variance, 자유도 보정):  
  $ s^2 = \frac{1}{n-1} \sum (x_i - \bar{x})^2 $

- 표준편차 (Standard Deviation):  
  $ \sigma = \sqrt{\sigma^2} $

- 범위 (Range), 사분위수 (Interquartile Range, IQR)

---

## 3. 분포의 모양

- 왜도 (Skewness): 분포의 비대칭 정도
- 첨도 (Kurtosis): 분포의 꼬리 두꺼움 정도

---

## 4. 확률분포

- 이산 확률분포: 이항분포(Binomial), 포아송분포(Poisson)
- 연속 확률분포: 정규분포(Normal), t-분포, 카이제곱분포 등

---

## 5. 신뢰구간과 가설검정

- 신뢰구간 (Confidence Interval):  
  모수를 포함할 것으로 기대되는 구간

- 가설검정 (Hypothesis Testing):
  - 귀무가설 $H_0$, 대립가설 $H_1$
  - 유의수준 $\alpha$, p-value 개념