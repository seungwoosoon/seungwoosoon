# Hi, I'm Seungwoo Son 
**Satellite Image & Geospatial Data Processing**

## Contact

[![Gmail Badge](https://img.shields.io/badge/-Gmail-c14438?style=flat-square&logo=Gmail&logoColor=white&link=mailto:tmddn0927@gmail.com)](mailto:tmddn0927@gmail.com)
[![GitHub Badge](https://img.shields.io/badge/-GitHub-181717?style=flat-square&logo=github&logoColor=white&link=https://github.com/seungwoosoon)](https://github.com/seungwoosoon)

## About Me

I am a data processing engineer who works with satellite imagery (SAR/EO) and has a strong interest in SAR image processing.


### 🎓 Education

- B.S. in Geoinformatic Engineering & Computer Science (Double Major), Inha University `2021.03 ~ 2027.02 (expected)`

### Internship

- Undergraduate Researcher, Image Engineering Lab (Prof. Taejung Kim), Inha University

### Research Projects in Lab (Private)

- **InSAR 기반 지표 변위 분석** — Image Engineering Lab, `[2026.03] ~ [2026.06]`
  - [Sentinel-1] SAR 위성 영상을 활용한 InSAR 처리(SBAS, D,PS - InSAR)로 지반변위 예측의 현실성 검토 및 기하정보 적용 가능성 탐구
  - Tech: `Python-MintPy` `MATLAB-STAMPS` `ISCE2` 
- **SAR-EO 이미지 매칭 연구** — Image Engineering Lab, `[2026.07] ~ [2026.08]`
  - 이종 센서(SAR-광학) 영상 간 특징점 기반 정합을 위해 **RoMa**, **RIFT** 알고리즘 적용 및 성능 비교
  - 목표: 정밀 지오레퍼런싱
  - Tech: `Python-RoMa` `C++-RIFT (fourier transform, Gabor Filter, Phase Congereuncy)`
### Personal Projects (Public)

- **SAR 편파 데이터 기반 벼 도복 판정 (RVI 시계열 분석)** — 위성영상처리 수업 프로젝트, `[2026.S1]`
  - Sentinel-1 SAR VV VH 편파 데이터로 산출한 RVI(Radar Vegetation Index) 시계열을 이용해 태풍 전후 벼 도복 피해를 자동 판정하는 알고리즘 구현
  - 평시 변동성 대비 임계값 기반 도복 조건을 설정하고, 위도 보정을 반영한 픽셀 면적 계산으로 실제 피해 면적(ha)까지 정량화
  - Tech: `Python` `Rasterio` `NumPy`
  - [🔗code] (https://github.com/seungwoosoon/RVI)
  - [🔗report] (https://github.com/seungwoosoon/seungwoosoon/blob/main/%5B위성영상처리%5D%20최종%20보고서_최종.docx)

- **위성·기상·토양 자료 기반 옥수수 수확량 예측 및 토지피복 분류** — 공간정보 인공지능 프로젝트, `2025.S2`
  - MODIS EVI, 강수량, 기온, SMAP 토양수분, VOD 등 다변량 시계열 자료로 county 단위 옥수수 수확량을 Linear/Ridge/Lasso 회귀 및 PCA 기반 차원축소를 통해 예측 (R² 0.79)
  - 광학(ATM)·레이더(L-band) 변수를 결합해 Softmax/Random Forest 기반 토지피복 분류 수행, 변수 조합별 분류 성능 비교분석
  - Tech: `Python` `scikit-learn` `PCA`

- **공간분석 기반 산불 감시 관제탑 최적 입지 선정** — 공간분석 수업 프로젝트, `[2025.S2]`
  - 등산로 주변 인공화재 위험도를 Fuzzy 로직(MATLAB)으로 정량화하고, DEM 기반 지형분석으로 관제탑 후보지 도출
  - Viewshed 분석과 화재위험도 격자의 교차분석을 통해 감시 효율이 높은 후보지 순위 산정
  - Tech: `ArcGIS` `MATLAB`

### Awards

- **GPS 위성 기반 버스 자동환승 시스템** — 2025 스페이스 해커톤, 우수상 `[2025]`
  - GPS 위성 측위 데이터를 활용해 환승 정류장 자동 인식 및 환승 처리를 자동화하는 시스템 설계
  - 담당 역할: 백엔드 로직 설계

## Skills

### 💻 Programming Language

![Python](https://img.shields.io/badge/python-3776AB?style=flat-square&logo=python&logoColor=white)
![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=flat-square&logo=mathworks&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)

### 🛰 Geospatial / Remote Sensing Stacks

![GDAL](https://img.shields.io/badge/GDAL-4CAE4C?style=flat-square)
![QGIS](https://img.shields.io/badge/QGIS-589632?style=flat-square&logo=qgis&logoColor=white)
![ArcGIS](https://img.shields.io/badge/ArcGIS-2C7AC3?style=flat-square)
![SNAP](https://img.shields.io/badge/SNAP-0086C9?style=flat-square)
![ISCE2](https://img.shields.io/badge/ISCE2-3D3D3D?style=flat-square)
![MintPy](https://img.shields.io/badge/MintPy-006747?style=flat-square)
![StaMPS](https://img.shields.io/badge/StaMPS-8B4513?style=flat-square)
![Rasterio](https://img.shields.io/badge/Rasterio-2E7D32?style=flat-square)

### 📚 ML/DL & Data Stacks

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=PyTorch&logoColor=white)
![NumPy](https://img.shields.io/badge/Numpy-150458?style=flat-square&logo=Numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=Pandas&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)

### 🛠 Tools

![VSCode](https://img.shields.io/badge/Visual%20Studio%20Code-007ACC?style=flat&logo=Visual%20Studio%20Code&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![Visual Studio](https://img.shields.io/badge/Visual%20Studio%202022-5C2D91?style=flat&logo=visual-studio&logoColor=white)
![PyCharm](https://img.shields.io/badge/PyCharm-000000?style=flat&logo=pycharm&logoColor=white)

### 📜 Certificates

- SQLD (SQL 개발자) `[2025.09]`
- TEPS ``

---
