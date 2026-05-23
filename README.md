# jiyoon99 Portfolio

Linux 운영, 백엔드 서비스, Windows 업무 자동화, Unity 게임 프로젝트를 직접 만들고 GitHub에 정리하고 있습니다.

핵심 방향은 “작동하는 결과물”과 “운영 가능한 구조”입니다. 단순 예제보다 실제로 실행해보고, 점검하고, 배포하거나 반복 업무를 줄이는 프로젝트를 포트폴리오로 정리했습니다.

## Portfolio Focus

| Area | What I Build | Main Projects |
| --- | --- | --- |
| Backend / Linux Ops | 실시간 서비스, Docker 운영, 모니터링, 배포 문서 | [linux-chess-portfolio](https://github.com/jiyoon99/linux-chess-portfolio), [linux-system-monitor](https://github.com/jiyoon99/linux-system-monitor) |
| Desktop / Local Tools | Linux 데스크톱 위젯, 로컬 개발 환경 상태 확인 | [linux-desktop-widget](https://github.com/jiyoon99/linux-desktop-widget) |
| Windows Automation | 노트북 검수, 드라이버 점검, USB/QC 자동화 | [inspection-automation](https://github.com/jiyoon99/inspection-automation), [driver-check-helper](https://github.com/jiyoon99/driver-check-helper), [usb-qc-automation](https://github.com/jiyoon99/usb-qc-automation) |
| Game Development | Unity 학습 결과물, 실행 가능한 Windows 빌드, 게임별 문서화 | [unity-game-portfolio](https://github.com/jiyoon99/unity-game-portfolio) |

## Featured Projects

### Linux Chess Portfolio

[Repository](https://github.com/jiyoon99/linux-chess-portfolio)

실시간 멀티플레이 체스 서비스를 기반으로 만든 백엔드 및 Linux 운영 포트폴리오입니다.

주요 구현:

- Go REST API와 WebSocket 기반 실시간 체스 대국
- 서버 측 체스 규칙 검증
- 회원가입/로그인, 게임 기록, PGN 리뷰
- PostgreSQL, Redis, Docker Compose 구성
- Nginx/Caddy reverse proxy, Prometheus, Grafana, Alertmanager
- 임시 공개 미리보기용 Cloudflare Tunnel 스크립트
- 배포, 백업/복구, 장애 대응, 운영 체크리스트 문서

설명할 수 있는 역량:

- 브라우저가 아닌 서버가 게임 상태를 책임지는 구조
- WebSocket 연결과 방 코드 기반 매칭
- Linux 서버에서 실제 서비스처럼 운영하는 구성
- 테스트, smoke test, 프로덕션 빌드, 배포 문서화

### Linux System Monitor

[Repository](https://github.com/jiyoon99/linux-system-monitor)

FastAPI, Docker, nginx, Chart.js, Ollama를 조합한 Linux 서버 실시간 모니터링 대시보드입니다.

주요 구현:

- CPU, RAM, Disk, Network 실시간 모니터링
- Docker daemon, container, image 상태 표시
- Server Bot 자동 점검과 WARN/FAIL 리포트
- Ollama 로컬 LLM 상태 확인 및 시스템 분석
- nginx reverse proxy와 Docker Compose 기반 실행
- 웹 대시보드와 CLI 동시 지원

설명할 수 있는 역량:

- Linux host metrics 수집
- Docker socket 기반 런타임 상태 확인
- 운영자가 빠르게 판단할 수 있는 대시보드 설계
- 로컬 AI API를 운영 도구에 연결하는 방식

### Linux Desktop Widget

[Repository](https://github.com/jiyoon99/linux-desktop-widget)

Linux 데스크톱 위에 떠 있는 작은 GTK 위젯으로 Docker, 로컬 서비스, Ollama AI 상태를 실시간 확인하는 도구입니다.

주요 구현:

- Docker daemon 응답 여부와 실행 중인 컨테이너 수 확인
- 로컬 포트와 호스트 상태 확인
- Ollama API와 설치 모델 상태 확인
- 3초 간격 자동 갱신
- 드래그 이동, 우클릭 종료, 로그인 자동 실행 스크립트

설명할 수 있는 역량:

- Linux desktop session에서 GTK 앱 구성
- 반복적인 터미널 확인 작업을 GUI 도구로 줄이는 방식
- 작은 개인 도구도 실행/종료/자동실행 경험까지 설계하는 관점

### Driver Check Helper

[Repository](https://github.com/jiyoon99/driver-check-helper)

Windows 장치 상태를 점검하고 필요한 드라이버 검색 경로를 정리해주는 PowerShell GUI 도구입니다.

주요 구현:

- 전체 장치 목록과 문제 장치 표시
- Hardware ID 기반 Microsoft Update Catalog 검색 링크 생성
- 제조사/모델 기반 공식 지원 페이지 안내
- JSON/HTML 리포트 저장
- GUI 버전과 콘솔 버전 제공
- Pester 테스트와 GitHub Actions Windows runner 구성

설명할 수 있는 역량:

- Windows 장치 정보를 PowerShell에서 수집하고 정규화
- 업무 반복 절차를 안전한 진단 보조 도구로 전환
- 실제 장비 정보가 노출되지 않도록 샘플 리포트와 공개 문서 분리

### Notebook Inspection Automation

[Repository](https://github.com/jiyoon99/inspection-automation)

중고/업무용 노트북 검수 과정을 GUI로 자동화한 PowerShell Windows Forms 프로젝트입니다.

주요 구현:

- 모델명, 시리얼, CPU, RAM/SSD 자동 수집
- 배터리 효율과 사이클 수 확인
- Wi-Fi, 카메라, 스피커 장치 인식 여부 점검
- 키보드/포트 테스트 창
- 정상/주의/불량 요약과 합격/재검수/불합격 자동 판정
- CSV 이력 저장과 PDF 리포트 출력

설명할 수 있는 역량:

- WMI/CIM, powercfg, device query 기반 하드웨어 진단
- 자동 진단과 수동 검수 결과를 함께 판정하는 구조
- 현장 업무 흐름을 GUI와 리포트 중심으로 정리하는 방식

### USB QC Automation

[Repository](https://github.com/jiyoon99/usb-qc-automation)

Windows 배치 파일 기반의 USB/하드웨어 출고 전 QC 자동 점검 매크로입니다.

주요 구현:

- 터미널 대시보드 형태의 QC 진행 화면
- USB 드라이브 탐지
- C 드라이브 확장, Bluetooth, 배터리, 시간 동기화 확인
- 카메라, 사운드, RAM/CPU/GPU 정보 확인
- 일반 QC와 렌탈 QC 스크립트 분리
- UEFI BIOS 재부팅 옵션 제공

설명할 수 있는 역량:

- Windows batch와 PowerShell 명령 조합
- 반복되는 출고 전 점검 절차를 스크립트화
- 실제 운영 식별 정보와 공개 포트폴리오 정보를 분리하는 방식

### Unity Game Portfolio

[Repository](https://github.com/jiyoon99/unity-game-portfolio)

Unity 학습 과정에서 만든 게임 결과물을 실행 가능한 Windows 빌드와 문서로 정리한 저장소입니다.

주요 구현:

- VamGame 2D 생존 액션 게임 빌드
- subakgame Windows 실행 빌드
- 게임별 README와 상세 문서
- VamGame Unity package 포함
- 에셋 프리뷰와 실행 방법 정리

설명할 수 있는 역량:

- Unity 게임 루프 구성
- 플레이어, 적, 무기, 아이템, HUD, 오브젝트 풀링 흐름 이해
- 학습 프로젝트를 실행 가능한 포트폴리오 결과물로 정리하는 방식

## Technical Stack

| Category | Tools |
| --- | --- |
| Backend | Go, Python, FastAPI, REST API, WebSocket |
| Frontend / UI | React, TypeScript, Vite, HTML, CSS, Chart.js, GTK, Windows Forms |
| Data / Runtime | PostgreSQL, Redis, Docker, Docker Compose |
| Linux Ops | nginx, Caddy, systemd, Prometheus, Grafana, Alertmanager |
| Windows Automation | PowerShell, Batch, WMI/CIM, powercfg, Pester |
| AI Integration | Ollama local API |
| Game | Unity, C# |
| Quality | Go test, TypeScript check, Pester, Playwright smoke test, GitHub Actions |

## Interview Story

이 포트폴리오는 한 가지 기술만 보여주는 방식이 아니라, “문제를 보고 도구를 만들어 해결하는 방식”을 보여주도록 구성했습니다.

- Linux 프로젝트는 서비스 운영, 모니터링, 배포, 장애 대응까지 설명할 수 있게 정리했습니다.
- Windows 자동화 프로젝트는 실제 반복 업무를 줄이는 도구로 만들고, 리포트와 안전한 공개 범위까지 고려했습니다.
- Unity 프로젝트는 학습 결과물을 실행 가능한 빌드와 문서로 남겨 결과 중심으로 정리했습니다.

## Links

- GitHub: [github.com/jiyoon99](https://github.com/jiyoon99)
- Main backend/Linux portfolio: [linux-chess-portfolio](https://github.com/jiyoon99/linux-chess-portfolio)
