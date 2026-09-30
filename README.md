<div align="center">

# Seungwoo Son

### Geospatial Data Developer


공간정보 데이터를 가공하고 처리해
효율적으로 유용한 시스템을 만드는 개발자입니다

<br/>

[![Gmail](https://img.shields.io/badge/tmddn0927@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:tmddn0927@gmail.com)
[![GitHub](https://img.shields.io/badge/seungwoosoon-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/seungwoosoon)

</div>

---

## Education

**인하대학교** 공간정보공학 전공 · 컴퓨터공학 복수전공 `2021.03 ~ 2027.02 (expected)`

- 전공 4.27 / 4.5 · 복수전공 4.50 / 4.5
- 자료구조, 알고리즘, 데이터베이스, 운영체제, 공간데이터베이스, 공간분석, 위성영상처리

**영상공학연구실 학부연구생** (지도교수 김태정) `2026.03 ~ 2026.08`

---

## Skills

**Backend** Java · Spring Boot · Spring Data JPA · REST API · MQTT (Eclipse Paho)

**Database** PostgreSQL · PostGIS · SQL

**Geospatial** QGIS · ArcGIS · GDAL · Rasterio · SNAP · ISCE2 · MintPy

**Language** Java · Python · C++ · Kotlin

**Tools** Docker · Nginx · Git · Unity

---

## Projects

### LaneNavigation — 차선 단위 내비게이션 `2026.09 ~ `

기존 내비는 "우회전하세요" 수준까지만 안내해 몇 차선으로 가야 하는지 알 수 없습니다. AI로 인식한 현재 차선과 HD맵에서 조회한 목표 차선의 차이를 계산해 "오른쪽으로 2차선 이동하세요"까지 안내합니다. 3인 팀에서 **백엔드·DB**를 담당합니다.

- 정밀도로지도(HD맵) 7개 레이어를 PostgreSQL/PostGIS에 적재하고 링크·노드·인접 차로 관계로 모델링
- GPS 좌표로 주행 중인 도로를 찾아 총 차선 수와 목표 차선을 계산하는 공간 쿼리 설계
- 카메라 AI를 상시 구동할 수 없어, 분기점까지 거리와 주행 속도로 실행 시점을 판단하는 로직 구현
- Tech: `Spring Boot` `PostgreSQL` `PostGIS` `Kotlin(Android)`
- [repository](https://github.com/seungwoosoon/lane-navigation)

### Farm Link — 스마트팜 센서 데이터 수집·관리 백엔드 `2025.07 ~ 2025.08`

센서와 AI 병해 진단으로 작물 상태를 관리하고 웹·3D 화면으로 보여주는 서비스입니다. KSEB 부트캠프 6인 팀에서 **백엔드를 전담**했습니다.

- 선반–층–화분의 물리적 배치를 계층 엔티티와 위치 인덱스로 모델링하고, 위치 기반 JPQL로 칸·줄·선반 단위 조회·갱신 API 구현
- 센서 보드마다 다른 메시지 형식(JSON · key:value 문자열)을 정규화하고 값이 있는 필드만 반영해 수집 데이터 일관성 확보
- MQTT 자동 재연결·재구독(QoS 1)으로 브로커 재시작 시에도 수집이 끊기지 않도록 구성
- 계층 조회의 N+1 문제를 fetch join과 `@Fetch(SUBSELECT)`로 해결해 조회 쿼리를 3회로 고정
- 멀티 스테이지 Docker 이미지와 Docker Compose(백엔드 · Mosquitto · Nginx)로 배포
- Tech: `Java 21` `Spring Boot` `JPA` `PostgreSQL` `MQTT` `Docker` `Unity`
- [repository](https://github.com/seungwoosoon/SmartFarmProject)

### GPS 기반 버스 자동환승 시스템 — 2025 스페이스 해커톤 **우수상** `2025`

스마트폰 위치 데이터만으로 버스 탑승을 판별해 환승을 자동 처리합니다. 3인 팀에서 **백엔드·Android 앱·판별 로직**을 담당했습니다.

- 버스위치정보 API로 받은 노선 위치와 GPS(NMEA) 궤적의 일치도를 계산해 탑승 여부 판별
- 비슷한 경로를 지나는 버스가 여러 대인 경우, 실시간 이동 속도를 함께 비교해 후보를 분리
- 판별 결과로 환승 정류장을 인식해 환승을 자동 처리

### 공간데이터베이스 — 공간 인덱스 성능 분석 `2025.2학기`

- PostGIS 공간 함수(`ST_Contains`, `ST_Intersects`)와 GiST 인덱스 실습, Filter–Refine 질의 처리와 R-tree · Grid File · Space-filling curve 학습
- **인덱스 성능 논문 리뷰** — 약 1,190만 건 도로망에서 `ST_Intersects` 응답이 약 126초에서 1초 수준으로 줄지만, 넓은 범위 질의에서는 순차 스캔보다 느려짐을 정리
- **공간 DB 서베이 논문 리뷰** — 공간 데이터 모델과 질의 처리 연구 흐름, 네트워크(도로망) 데이터 모델링 과제 정리

---

## Research

**영상공학연구실 학부연구생** `2026.03 ~ 2026.08`

- **EO–SAR 이종센서 영상 정합** — RIFT 알고리즘을 C++로 구현(FFT · Log-Gabor · Phase Congruency)하고 딥러닝 매처 RoMa를 적용해 센서·해상도 조건별 정합 성능을 정량 비교. RoMa의 매칭 불안정 원인을 학습 입력 규격(768×768)에서 찾아 피라미드 타일링 구조로 개선
- **InSAR 시계열 지표 변위 분석** — Sentinel-1 영상 46장을 ISCE2로 전처리하고 MintPy(SBAS) · StaMPS(PSInSAR)로 처리. 대기 지연 · 궤도 오차 · 잔여 지형 오차를 각각 분리 검증하고 기술 문서로 정리

---

## Coursework Projects

- **SAR 편파 시계열 기반 태풍 벼 도복 탐지** `2026.S1` — Sentinel-1 RVI 시계열에 픽셀별 자연 변동성 기반 동적 임계값을 적용해 도복을 자동 판정하고, 위도 보정으로 피해 면적(ha) 산출 · [code](https://github.com/seungwoosoon/RVI)
- **다원 위성·기상 자료 기반 수확량 예측 및 토지피복 분류** `2025.S2` — 41개 변수의 다중공선성을 진단해 이상치 제거 · 표준화 · PCA를 적용하고 Ridge 회귀로 MAE 0.909 달성, 광학·레이더 변수 결합 분류 수행
- **공간분석 기반 산불 감시탑 입지 선정** `2025.S2` — 퍼지 로직 화재 위험도 격자와 DEM 기반 Viewshed를 교차분석해 후보지 순위 산정

---

## Certificates

- SQLD (SQL 개발자) `2025.09`
- TEPS 338
