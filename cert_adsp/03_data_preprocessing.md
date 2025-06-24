# 🧹 ADSP 데이터 전처리 정리

## 1. 결측치(Missing Values) 처리

### ① 제거(Drop)
- 결측치가 있는 행이나 열을 삭제
- 예: `df.dropna()`

### ② 대체(Imputation)
- 평균, 중앙값, 최빈값 등으로 채움
- 예: `df.fillna(df['col'].mean())`

### ③ 예측 기반 채움
- 회귀모델이나 KNN 등으로 결측값 예측해 채우는 방식

---

## 2. 이상치 처리 (Outlier Handling)

### ① Z-score 방법
- 평균에서 3표준편차 넘는 값 제거

### ② IQR 방법
- Q1 - 1.5×IQR 미만, Q3 + 1.5×IQR 초과 값 제거

---

## 3. 정규화 (Normalization)

- 데이터 범위를 0과 1 사이로 조정
- 예: `X_scaled = (X - X.min()) / (X.max() - X.min())`

---

## 4. 표준화 (Standardization)

- 평균 0, 표준편차 1로 변환
- 예: `X_scaled = (X - X.mean()) / X.std()`

---

## 5. 로그 변환 (Log Transform)

- 분포가 한쪽으로 치우친 경우 완화
- 예: `np.log1p(X)` (0 포함 가능)

---

## 6. 기타 전처리 기법
- 더미변수화(One-hot encoding)
- 범주형 변수 정리
- 이상치 플래깅(outlier flagging)