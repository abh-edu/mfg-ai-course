# 제조 AI 심화과정 — 실습 자료

삼성전자 × KAMPA 「제조 AI 심화과정」에서 쓰는 실습 노트북과 데이터입니다. 만든 곳: ㈜에이비에이치

## 바로 열기

**접속 페이지: https://abh-edu.github.io/mfg-ai-course/** — 버튼 두 개만 있는 쪽입니다. 수업에서는 이 주소로 들어옵니다.

| 실습 | 내용 | Colab에서 열기 | 실행 없이 결과 보기 |
|---|---|---|---|
| **실습 ① 고장 예측** (오전) | 설비 가동 기록 10,000건으로 고장 예측 모델을 만들고, 정확도 98%를 의심해 봅니다 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/abh-edu/mfg-ai-course/blob/main/lab1_failure_prediction.ipynb) | [결과 보기](https://abh-edu.github.io/mfg-ai-course/results/lab1.html) |
| **실습 ② 외관 이상탐지** (오후) | 정상 사진만 외워서 처음 보는 불량을 찾아냅니다. 불량 사진은 쓰지 않습니다 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/abh-edu/mfg-ai-course/blob/main/lab2_vision_anomaly.ipynb) | [결과 보기](https://abh-edu.github.io/mfg-ai-course/results/lab2.html) |

두 실습 모두 GPU가 필요 없습니다. Google 계정으로 로그인한 뒤 칸 왼쪽의 ▶ 를 위에서 아래로 차례로 누르면 됩니다.

## 들어 있는 것

| 파일 | 설명 |
|---|---|
| `index.html` | 접속 페이지 |
| `lab1_failure_prediction.ipynb` | 실습 ① 노트북 |
| `lab2_vision_anomaly.ipynb` | 실습 ② 노트북 |
| `ai4i2020.csv` | 실습 ① 데이터 |
| `data/visa_*.zip` | 실습 ② 데이터 (품목별 사진 묶음 9개) |
| `results/lab1.html`, `results/lab2.html` | 실행을 마친 화면. Colab을 쓸 수 없을 때 봅니다 |
| `lab2_casting_defect_full.ipynb` | 2026년 9~10월 과정에서 쓴 이전 실습 ② (보관용) |
| `abh/` | ㈜에이비에이치 소개·제안 자료(PDF)와 자료실 쪽 — https://abh-edu.github.io/mfg-ai-course/abh/ |

## 데이터와 사용 조건

- **AI4I 2020 Predictive Maintenance Dataset** — S. Matzka, UCI Machine Learning Repository. CC BY 4.0.
- **VisA (Visual Anomaly) Dataset** — Zou et al., “SPot-the-Difference Self-Supervised Pre-training for Anomaly Detection and Segmentation”, ECCV 2022. © Amazon. CC BY 4.0. 원본: https://github.com/amazon-science/spot-diff
  - `data/visa_*.zip` 은 수업용으로 줄인 발췌본입니다. 품목마다 정상 250장(외우기 150, 시험 100)과 불량 100장을 무작위로 뽑고, 긴 변을 448픽셀로 줄여 JPEG로 저장했으며, 결함 위치 표시(마스크)는 흑백 두 값으로 바꾸었습니다.
- 실습 ②의 방법은 PatchCore(Roth et al., CVPR 2022)를 수업용으로 줄인 구현입니다.

노트북과 접속 페이지는 교육 목적으로 자유롭게 쓰셔도 됩니다. 데이터는 위의 조건(출처 표시)을 따릅니다.

`abh/` 폴더의 소개·제안 자료는 ㈜에이비에이치의 자료이며 위의 자유 이용 범위에 들지 않습니다. 같은 폴더의 정부 발표 원문(중소벤처기업부 공고 제2026-620호, 관계부처 합동 「중소제조 피지컬 AI 확산 전략」)은 해당 기관의 자료입니다.

## 문의

㈜에이비에이치 · abh@abhcst.com
