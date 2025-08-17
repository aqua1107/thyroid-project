# Thyroid Disease Classification for Privacy-Preserving Healthcare AI

> **"7억명의 갑상선 환자를 위한 AI 진단 시스템"**

## Project Overview
- **목적**: 갑상선 질환 조기 진단을 위한 머신러닝 모델 개발
- **핵심 가치**: 의료 데이터 프라이버시 보호와 AI 성능의 균형
- **대상**: 의료진, AI 연구자, 헬스케어 스타트업

## Dataset Information
- **Source**: UCI Machine Learning Repository
- **Size**: 215 instances, 5 features
- **Classes**: Normal (150), Hyperthyroid (35), Hypothyroid (30)
- **Features**: T3 resin uptake, Total T4, Total T3, Basal TSH, Max TSH diff

## Key Analysis Results

### 1. 의학적 인사이트
- TSH와 T3/T4의 길항작용 확인
- 갑상선 저하증: TSH 12.92 (정상의 10배 상승)
- 갑상선 항진증: T3/T4 2배 이상 증가

### 2. 데이터 과학적 접근
- 통계적 이상치를 의학적 관점에서 재해석
- 중증 환자 데이터 보존을 통한 실용적 모델 개발

## Model Performance & Insights

### 성능 요약
- **전체 정확도**: 98% (43개 중 42개 정확 예측)
- **클래스별 성능**:
  - Normal: 100% (28/28) - 완벽 분류
  - Hyperthyroid: 100% (8/8) - 완벽 분류  
  - Hypothyroid: 86% recall (6/7) - 1개 오분류

### 주요 발견사항
**의학적 타당성**: 갑상선 호르몬 수치의 명확한 구분으로 높은 정확도 달성  
**임상적 유용성**: TSH가 가장 중요한 진단 지표임을 AI 모델로 검증  
**개선 영역**: 저하증 환자 일부가 정상으로 오분류되는 문제 존재

### 결론
로지스틱 회귀 모델이 갑상선 데이터에서 전체적으로 98% 정확도를 보였으며, 특히 정상과 항진증은 완벽히 구분했습니다. 다만 저하증 환자 일부가 정상으로 분류되는 경우가 있어, recall을 더 높이는 방향의 추가 보완이 필요함.

### 데이터셋 출처
링크: https://archive.ics.uci.edu/dataset/102/thyroid+disease