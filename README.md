<div align="center">

# 허민엽

### 제조 현장의 영상·설비 데이터를 읽고, 동작하는 시스템으로 연결하는 SW 엔지니어

머신비전 · 스마트팩토리 MES · 설비 진단(PHM)

<br>

[![Portfolio](https://img.shields.io/badge/Portfolio-hmy7788.github.io-2563eb?style=for-the-badge&logo=astro&logoColor=white)](https://hmy7788.github.io)
[![Mail](https://img.shields.io/badge/Mail-hmya5789@gmail.com-ea4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:hmya5789@gmail.com)

</div>

<br>

> 문제 해결에 집중하여, 상황에 맞는 도구를 선택하고 책임감 있게 끝까지 실행하는 SW 엔지니어입니다.

## About

- 동아대학교 컴퓨터공학과 2026.08 졸업
- 현대오토에버 모빌리티 SW스쿨 4기 스마트팩토리 과정 수강 중 (2026.07 ~ 2026.12): MES, CPS/PHM, 머신비전
- 스마트팩토리 MES · 머신비전 SW 개발 직무를 준비하고 있습니다

## What I Do

| 🔍 머신비전 | 🏭 MES · 관제 | 📈 설비 진단 · 생산 시뮬레이션 |
| --- | --- | --- |
| 지도학습 CNN, 비지도 이상탐지(PatchCore), 객체 검출(YOLO · RT-DETR · D-FINE)을 같은 조건에서 비교해 선택 | 검사 결과를 DB에 적재하고 실시간 관제 대시보드로 보여주는 미니 MES, 작업지시 · 판정 결과 연동 구조 | 진동 신호의 FFT · 속도 스펙트럼으로 결함 원인을 진단, 셀 생산 라인을 시뮬레이션으로 재설계 |

## Featured Work

<table>
  <tr>
    <td width="33%" align="center">
      <img src="https://raw.githubusercontent.com/hmy7788/aegis-vision/main/presentation/screenshots/demo_assembly_flow.gif" alt="AEGIS 시연: 재료 확인, 조립, 오조립 NG, 수정, PASS">
      <br><sub><b>AEGIS</b> · 오조립을 조립 중에 감지해 틀린 자리와 원인 표시</sub>
    </td>
    <td width="33%" align="center">
      <img src="https://hmy7788.github.io/images/project2-heatmap.png" alt="PatchCore 결함 위치 히트맵">
      <br><sub><b>PatchCore</b> · 정상 데이터만으로 학습해 결함 위치까지 검출</sub>
    </td>
    <td width="33%" align="center">
      <img src="https://hmy7788.github.io/images/phm-02-fft-gmf.jpg" alt="FFT 스펙트럼에서 1X GMF 607Hz와 하모닉">
      <br><sub><b>PHM</b> · FFT로 1X GMF와 하모닉을 확인해 결함 원인 진단</sub>
    </td>
  </tr>
</table>

### 머신비전

| 프로젝트 | 내용 | 결과 |
| --- | --- | --- |
| **[AEGIS](https://github.com/hmy7788/aegis-vision)** · [시연 영상](https://www.youtube.com/watch?v=MuZ7LdKFj_c)<br><sub>팀 4인 · 2026.09</sub> | 다품종 조립 공정의 오조립 검증. 룰베이스의 한계를 수치로 확인한 뒤 딥러닝 검출 3종을 같은 조건에서 비교. **담당**: 룰베이스 검증, RT-DETR 학습, 조립 과정 평가 로직 | 룰베이스 정확도 81.2%, YOLO26n-OBB mAP50-95 0.877, 오류 사건 7건 중 7건 검출 (RT-DETR 포함 2종) |
| **[K-Arch Trip](https://github.com/hmy7788/K-Arch-Trip)**<br><sub>팀 5인 · 2026.09</sub> | 형태 판별 파이프라인을 텀블러 4종 분류로 검증하고, 6갈래 방법론(룰베이스부터 ViT까지)을 비교. **담당**: 룰베이스, ResNet-18/50, 트랙 통합 · 테스트 · 문서화 | 실촬영 정확도 EfficientNet-B0 88.1%, 룰베이스 18.4% |
| **[KAMP X-ray 이물질 탐지](https://github.com/hmy7788/kamp_xray_detection)**<br><sub>팀 · 제6회 K-인공지능 제조데이터 분석 경진대회</sub> | 완제품 X-ray 영상의 5~21px 소형 이물질 검출. 6개 모델을 동일 분할 · 채점 코드로 비교 | D-FINE-N mAP50 0.989, CPU 10.3 FPS |
| **PatchCore 나사 결함 검출 & 라인 관제**<br><sub>개인 · 2026.05 – 06</sub> | 불량 데이터 희소 문제를 정상 데이터만으로 학습하는 이상탐지로 해결하고 미니 MES까지 구현 | AUPRO 0.956 · 28.0 FPS, 임계값을 F2 기준으로 재탐색해 Recall 0.992 |
| **지도학습 CNN 나사 결함 탐지**<br><sub>개인 · 졸업논문 · 2026.02 – 05</sub> | CNN 3종을 같은 조건에서 비교, 불량 미검출을 줄이는 F2-Score를 핵심 지표로 설계 | ResNet-18 F2 0.8854 · 88.8 FPS |

### 스마트팩토리

| 프로젝트 | 내용 | 결과 |
| --- | --- | --- |
| **에어컨 다품종 셀 생산라인 설계 (CPS)**<br><sub>팀 5인 · SW스쿨 교육 프로젝트</sub> | 5,000대 대량 주문 상황에서 라인 방식의 병목을 시뮬레이션으로 진단하고 다기능 작업자 기반 셀 생산으로 재설계. **담당**: TO-BE-B 레이아웃 설계 · 실험 | UPH 1.98 → 6.94 (가상 공장 시뮬레이션 기준) |
| **설비 진동 진단 (PHM)**<br><sub>팀 5인 · SW스쿨 교육 프로젝트</sub> | FAN 불평형부터 커플링, 베어링, 기어 손상까지 진동 데이터로 진단. **담당**: 신호 처리 알고리즘 설계 | 베어링 내륜 결함 계산값 120.15Hz와 측정 피크 120Hz 일치 |

각 프로젝트의 문제 정의, 트러블슈팅, 한계는 **[포트폴리오 사이트](https://hmy7788.github.io/#projects)** 에 정리해 두었습니다.

## Tech

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![Ultralytics](https://img.shields.io/badge/YOLO%20·%20RT--DETR-111F68?style=flat-square)
![anomalib](https://img.shields.io/badge/anomalib%20·%20PatchCore-0071C5?style=flat-square)

![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)

![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Notion](https://img.shields.io/badge/Notion-000000?style=flat-square&logo=notion&logoColor=white)

## Background

| 기간 | 내용 |
| --- | --- |
| 2026.07 ~ 2026.12 | 현대오토에버 모빌리티 SW스쿨 4기 스마트팩토리 과정 |
| 2026.09 | 정보처리기사 취득 |
| 2026.08 | ADsP (데이터분석 준전문가) 취득 |
| 2026.03 | TOEIC Speaking IH (ETS) |
| 2025.11 | 교내 Vision Mandarine Hack 대상 (동아대학교 소프트웨어대학, 팀장) |
| 2020.03 ~ 2026.08 | 동아대학교 컴퓨터공학과 졸업 |

## How I Work

- **명확한 역할 분담**: 팀원의 전공과 강점에 맞춰 역할을 재배치해, 특정 인원에게 업무가 쏠리지 않도록 조율합니다.
- **우선순위 먼저**: 의견이 갈릴 때는 우선순위 기준을 먼저 세워, 무엇을 먼저 하고 무엇을 나중에 할지로 정리합니다.
- **직접 구현해서 확인**: 프로젝트 목적에 맞춰 필요한 기술을 그때그때 학습하고, 이론에서 멈추지 않고 직접 구현해 완성합니다.

## Contact

- Portfolio: [hmy7788.github.io](https://hmy7788.github.io)
- Mail: [hmya5789@gmail.com](mailto:hmya5789@gmail.com)
