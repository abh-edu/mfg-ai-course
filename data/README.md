# 실습 ② 데이터 — VisA 발췌본

이 폴더의 `visa_*.zip` 은 **VisA (Visual Anomaly) Dataset** 에서 수업용으로 뽑아 줄인 발췌본입니다.

- 원본: Zou et al., “SPot-the-Difference Self-Supervised Pre-training for Anomaly Detection and Segmentation”, ECCV 2022. © Amazon. https://github.com/amazon-science/spot-diff
- 사용 조건: CC BY 4.0 (출처 표시)
- 바꾼 점: 품목마다 정상 250장(외우기 150, 시험 100)과 불량 100장을 무작위로 뽑고, 긴 변을 448픽셀로 줄여 JPEG로 저장했습니다. 결함 위치 표시(마스크)는 흑백 두 값으로 바꾸었습니다.

묶음 하나의 구성: `<품목>/index.csv` (사진 경로, 용도, 정상·불량, 결함 위치 파일, 결함 종류)와 사진 폴더.

| 파일 | 품목 |
|---|---|
| `visa_pcb4.zip` | 기판 A (USB 충전 모듈) — 수업의 기본 예제 |
| `visa_pcb1.zip` | 기판 B (초음파 센서 모듈) — 해상도 실험 |
| `visa_chewinggum.zip` | 껌 |
| `visa_capsules.zip` | 캡슐 |
| `visa_pcb3.zip`, `visa_cashew.zip`, `visa_pipe_fryum.zip`, `visa_fryum.zip`, `visa_candle.zip` | 더 해 보기용 |
