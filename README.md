# SaaS 고객 이탈 예측 & 코호트 분석 플랫폼

> 7,043명 고객 코호트 분석과 LightGBM 이탈 예측으로 리텐션 개선 타겟 세그먼트 도출, Bayesian A/B 테스트로 쿠폰 vs 이메일 전략 비교

## 📌 문제 정의
<!-- 배경, 비즈니스 질문, 성공 지표를 여기에 작성하세요 -->

## 🏗️ 아키텍처

```
[데이터 소스] → [ETL 파이프라인] → [DB/저장소] → [ML 모델] → [API] → [프론트엔드]
```

## 🔧 기술 스택

| Layer | Stack |
|-------|-------|
| Pipeline | Prefect 2.x, dbt Core |
| ML | LightGBM, SHAP, lifelines, pymc (Bayesian A/B) |
| Backend | Spring Boot 3.2 (Java 17), Spring Data JPA, Swagger |
| DB | PostgreSQL 16 (Star Schema) |
| Frontend | Next.js 14, D3.js, Tailwind CSS |
| Infra | Docker Compose, GitHub Actions |

## 📊 핵심 인사이트
<!-- 분석 결과 및 시각화를 여기에 추가하세요 -->

## 🚀 실행 방법

```bash
git clone https://github.com/sth00619/customer-churn-platform.git
cd customer-churn-platform
docker-compose up -d
```

## 📂 프로젝트 구조

```
customer-churn-platform/
├── pipeline/         # Airflow DAG / Prefect Flow
├── backend/          # FastAPI or Spring Boot
├── frontend/         # Next.js
├── ml/               # 모델 학습 및 서빙
├── db/               # 스키마 및 마이그레이션
└── docker-compose.yml
```

## 🔗 배포 URL
<!-- https://your-app.railway.app -->

## ⚠️ 한계와 다음 단계
<!-- 데이터 한계, 개선 방향 등 -->
