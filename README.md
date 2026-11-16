<h1 align="center">변상현 · SangHyun Byun</h1>

<p align="center">
  <b>C++·C# 응용 SW 개발자</b><br>
  AI 모델과 SDK를 실제 장비에서 멈추지 않고 돌아가는 소프트웨어로 만듭니다<br>
  <sub>C++/C# application engineer who turns AI engines into shippable software</sub>
</p>

<p align="center">
  <a href="mailto:<기존 이메일>">Email</a> ·
  <a href="https://ggoosae.tistory.com/">Blog</a>
</p>

---

## 소개

- **라온피플**에서 AI 비전 엔진을 C++·C# 제품 소프트웨어로 만들고 있습니다. (2025.10 ~ 현재)
- 이전에는 **이노시뮬레이션**에서 Unreal Engine 기반 체험 시뮬레이터를 개발했습니다. (2023.12 ~ 2025.10)
- 중앙대학교 첨단영상대학원 석사 (Computer Vision · Deep Learning)

## 잘하는 일

| 역량 | 내용 |
|---|---|
| **C++·C# 경계 설계** | 네이티브 SDK를 C++ DLL로 감싸 C# 앱에 연결합니다. C ABI, P/Invoke, 핸들 수명, 오류 코드 규약 |
| **멈추지 않는 데스크톱 SW** | SDK 전용 스레드, bounded Channel 파이프라인, 취소 처리, WPF MVVM, xUnit |
| **AI를 제품에 넣기** | TensorRT 혼합 정밀도·부분 양자화, OpenVINO CPU 추론, 온디바이스 VLM |
| **장비·통신 통합** | 시리얼·TCP·UDP 장비 연동, 여러 화면의 상태 동기화 (Unreal Engine) |

## 업무에서 만든 것

회사 코드는 공개할 수 없어 한 일과 결과만 적습니다.

| 작업 | 한 일 | 결과 |
|---|---|---|
| **CPU 비전 검사 프로그램** (단독 개발) | C++17 래퍼 DLL + C# WPF, SDK 전용 스레드와 4단 처리 파이프라인 | SDK 순수 추론 분류 약 0.2ms · 검출 약 10ms (256×256, Intel CPU), xUnit 테스트 60여 개, AW2026 전시 |
| **비전 모델 학습 SDK의 C API·CLI** (C++ 계층 단독 개발) | 순수 C 함수 경계, 학습 엔진 프로세스 실행, 출력·종료 코드 규약 | 학습 작업 4종 지원, 명령줄 자격증명 노출 제거 |
| **WPF 데스크톱 앱 안정화** | 런타임 오류 전수 점검, 원인별 재발 방지 | 설계 문제 24건 수정, 원인 5가지로 분류, xUnit 테스트 289개 |
| **엣지 AI 추론 최적화** | Jetson Orin Nano에서 TensorRT 혼합 정밀도·부분 양자화 | 모델 추론 약 20~30ms → 6~7ms (640×640 · 배치 4, FP16 대비) |
| **전차 체험 시뮬레이터** (팀) | Unreal Engine 화면·차량 동역학, 시리얼·TCP·UDP 장비 연동 | 화면 간 위치·피격 시점 불일치 해결, KADEX 2024 전시 |


## 논문 · 특허

- **Transfer Learning based Parameterized 3D Mesh Deformation with 2D Stylized Cartoon Character** — KSII Transactions on Internet and Information Systems, 2023 (제1저자) · [DOI](https://doi.org/10.3837/tiis.2023.11.012)
- **Harnessing Synthetic Data for Enhanced Detection of Pine Wilt Disease: An Image Classification Approach** — Computers and Electronics in Agriculture, 2024 (SCIE, 제2저자) · [DOI](https://doi.org/10.1016/j.compag.2024.108690)
- **Minecraft-ify: Minecraft Style Image Generation with Text-guided Image Editing for In-Game Application** — NeurIPS 2023 Workshop on ML for Creativity and Design, 구두 발표
- 특허 등록 2건 · 출원 1건 — 2D 캐릭터 기반 3D 메쉬 변형 방법(등록), 인터랙티브 가상 현미경 제공 장치(등록), 합성 데이터 기반 소나무재선충병 검출 시스템(출원)

## 기술

- **언어:** C++17 · C# · Python
- **응용 SW:** .NET 8 WPF · Qt · Win32 API · xUnit
- **AI:** PyTorch · OpenCV · TensorRT · OpenVINO · NVIDIA Jetson
- **그 외:** Unreal Engine · Unity · FastAPI · Docker · Git
