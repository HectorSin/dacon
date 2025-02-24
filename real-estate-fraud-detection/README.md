# 부동산 허위매물 분류 해커톤: 가짜를 색출하라!

## 프로젝트 개요

이 프로젝트는 데이콘에서 주최하는 "부동산 허위매물 분류 해커톤: 가짜를 색출하라!" 대회에 참여하기 위한 것입니다. 이 해커톤의 주요 목표는 부동산 데이터와 AI 기술을 활용하여 허위매물을 분류하는 AI 알고리즘을 개발하는 것입니다.

## 대회 정보

* 주최: 데이콘
* 대상: 데이커라면 누구나 참여 가능
* 유형: 교육 목적의 데이스쿨 자체 해커톤 (정규 대회 아님)
* 참고사항: 프로필 이력 노출 및 랭킹 포인트 반영 없음

## 주요 일정
* 대회 시작: 2025년 1월 6일
* 대회 종료: 2025년 2월 28일
* 코드 제출 마감: 2025년 3월 5일
* 코드 검증: 2025년 3월 14일
* 최종 수상자 발표: 2025년 3월 17일

## 프로젝트 목표

부동산 매물 관련 정보가 포함된 데이터를 활용하여 허위매물을 분류하는 AI 알고리즘을 개발합니다. 이를 통해 부동산 시장의 투명성을 높이고, 소비자와 중개업자 모두에게 신뢰할 수 있는 거래 환경을 제공하는 데 기여하고자 합니다.

## 데이터셋

[train.csv]
훈련 데이터셋으로, 다음 필드를 포함합니다:
* ID: 샘플별 고유 ID
* 매물확인방식
* 보증금
* 월세
* 전용면적
* 해당층
* 총층
* 방향
* 방수
* 욕실수
* 주차가능여부
* 총주차대수
* 관리비
* 중개사무소
* 제공플랫폼
* 게재일
* 허위매물여부 (목표 변수)

[test.csv]
테스트 데이터셋으로, 훈련 데이터와 동일한 필드를 포함하지만 '허위매물여부' 필드는 제외됩니다.

[sample_submission.csv]
제출 양식 파일로, 다음 필드를 포함합니다:
ID: 샘플별 고유 ID
허위매물여부: 예측해야 할 목표 변수

## 평가 지표

* 평가 산식: Macro F1 Score
* Public Score: 전체 테스트 데이터 중 사전 샘플링된 50%
* Private Score: 전체 테스트 데이터 100%

## 프로젝트 구조

```
real-estate-fraud-detection/
│
├── data/                # 데이터셋 저장 폴더
├── notebooks/           # Jupyter 노트북 파일
├── src/                 # 소스 코드
├── models/              # 학습된 모델 저장
├── README.md            # 프로젝트 설명 (현재 파일)
└── .gitignore           # Git 무시 파일 목록
```

## 설치 및 실행 방법