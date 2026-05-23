<div align="center">

# jiyoon99

### Backend · Linux Ops · Automation · Unity C# Game Development

반복되는 점검, 모니터링, 운영 업무를 자동화 도구와 대시보드로 바꾸는 개발을 하고 있습니다.  
Linux 서버 모니터링, 로컬 AI 분석, Windows 장비 검수 자동화, Unity C# 게임 프로젝트를 포트폴리오로 정리했습니다.

<p>
  <img src="https://img.shields.io/badge/Backend-111827?style=flat-square" />
  <img src="https://img.shields.io/badge/Linux%20Ops-FCC624?style=flat-square&logo=linux&logoColor=black" />
  <img src="https://img.shields.io/badge/Automation-2563EB?style=flat-square" />
  <img src="https://img.shields.io/badge/Unity%20C%23-000000?style=flat-square&logo=unity&logoColor=white" />
</p>

</div>

---

## Profile

- 실무에서 반복되는 점검 절차를 자동화하고, 결과를 리포트로 남기는 도구를 직접 설계했습니다.
- Linux, Docker, Ollama, FastAPI를 활용해 서버 상태를 관찰하고 판단을 돕는 대시보드를 구성했습니다.
- Windows PowerShell과 Windows Forms로 장비 검수, 드라이버 점검, QC 자동화 도구를 만들었습니다.
- Unity와 C#으로 2D 게임 프로젝트를 구현하고, 실행 빌드와 문서 중심의 포트폴리오로 정리했습니다.

## For Interviewers

빠르게 보실 때는 아래 세 가지 흐름으로 봐주시면 됩니다.

| Focus | What to Check | Projects |
| --- | --- | --- |
| Linux / Backend Ops | Docker 기반 실행, reverse proxy, 모니터링, 로그 분석, 운영 문서 | [linux-chess-portfolio](https://github.com/jiyoon99/linux-chess-portfolio), [linux-system-monitor](https://github.com/jiyoon99/linux-system-monitor), [linux-web-log-sql-analyzer](https://github.com/jiyoon99/linux-web-log-sql-analyzer) |
| Local Productivity Tools | Linux 데스크톱에서 매번 확인하던 상태를 위젯/대시보드로 자동화 | [linux-desktop-widget](https://github.com/jiyoon99/linux-desktop-widget), [linux-system-monitor](https://github.com/jiyoon99/linux-system-monitor) |
| Work Automation | 실제 장비 점검 반복 작업을 GUI, 리포트, 테스트가 있는 도구로 정리 | [driver-check-helper](https://github.com/jiyoon99/driver-check-helper), [inspection-automation](https://github.com/jiyoon99/inspection-automation), [usb-qc-automation](https://github.com/jiyoon99/usb-qc-automation) |

## Languages

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white" />
  <img src="https://img.shields.io/badge/C%23-512BD4?style=for-the-badge&logo=dotnet&logoColor=white" />
  <img src="https://img.shields.io/badge/PowerShell-5391FE?style=for-the-badge&logo=powershell&logoColor=white" />
  <img src="https://img.shields.io/badge/Batch-111827?style=for-the-badge&logo=windows-terminal&logoColor=white" />
  <img src="https://img.shields.io/badge/Markdown-000000?style=for-the-badge&logo=markdown&logoColor=white" />
</p>

## Tech Stack

| Area | Stack |
| --- | --- |
| Backend / AI | Python, FastAPI, Go, REST API, WebSocket, Ollama |
| Linux / Infra | Linux, Docker, Docker Compose, nginx, Caddy, systemd |
| Data / Runtime | PostgreSQL, Redis, SQLite, MySQL |
| Monitoring | Prometheus, Grafana, Alertmanager, Chart.js, `/proc`, `/sys` |
| Windows Automation | PowerShell, Windows Forms, WMI/CIM, Batch, Pester |
| Game Development | Unity, C#, Windows Build |
| Documentation | Markdown, JSON/HTML reports, project runbooks |

## Linux Projects at a Glance

면접에서 설명하기 쉬운 리눅스 프로젝트를 우선순위대로 정리했습니다.

| Project | Problem | Implementation | What It Shows |
| --- | --- | --- | --- |
| [Linux Chess Portfolio](https://github.com/jiyoon99/linux-chess-portfolio) | 실시간 서비스를 Linux 환경에서 어떻게 운영할지 보여줄 프로젝트가 필요했습니다. | Go API, WebSocket, PostgreSQL, Redis, Docker Compose, reverse proxy, Prometheus/Grafana를 구성했습니다. | 백엔드 구조, 실시간 통신, DB/캐시, 배포/모니터링 문서화 |
| [Linux System Monitor](https://github.com/jiyoon99/linux-system-monitor) | CPU/RAM/Disk/Docker/Ollama 상태를 매번 여러 명령어로 확인해야 했습니다. | FastAPI 대시보드, Docker socket 조회, nginx reverse proxy, Chart.js 그래프, Ollama API 연동을 만들었습니다. | Linux metrics 수집, Docker 운영 상태 확인, 로컬 AI API 연동 |
| [Linux Desktop Widget](https://github.com/jiyoon99/linux-desktop-widget) | 개발 중 Docker와 Ollama가 켜져 있는지 터미널을 열지 않고 보고 싶었습니다. | Python GTK 위젯, 3초 자동 갱신, Docker/포트/Ollama 상태 체크, autostart 스크립트를 만들었습니다. | Linux 데스크톱 앱, 로컬 생산성 도구, 실행/종료 UX |
| [Linux Web Log SQL Analyzer](https://github.com/jiyoon99/linux-web-log-sql-analyzer) | 웹 서버 access log를 SQL로 분석하는 흐름을 보여주고 싶었습니다. | Nginx/Apache 로그 파서, SQLite 적재, 집계 SQL 리포트, 로컬 웹 대시보드를 구현했습니다. | 로그 처리, DB schema/index, SQL aggregation, CLI 자동화 |

## Representative Projects

| Project | What It Shows | Stack |
| --- | --- | --- |
| [linux-system-monitor](https://github.com/jiyoon99/linux-system-monitor) | Linux 서버, Docker, Ollama 상태를 한 화면에서 확인하고 로컬 AI 분석으로 운영 판단을 돕는 대시보드 | Python, FastAPI, Docker, nginx, Chart.js, Ollama |
| [linux-desktop-widget](https://github.com/jiyoon99/linux-desktop-widget) | Docker/Ollama/로컬 서비스 상태를 데스크톱 위젯으로 빠르게 확인하는 Linux 운영 도구 | Python, GTK, Linux, Docker, Ollama |
| [linux-chess-portfolio](https://github.com/jiyoon99/linux-chess-portfolio) | 실시간 WebSocket 서비스와 DB/캐시 구성을 포함한 백엔드 운영 포트폴리오 | Go, WebSocket, PostgreSQL, Redis, Docker |
| [linux-web-log-sql-analyzer](https://github.com/jiyoon99/linux-web-log-sql-analyzer) | Linux 웹 서버 access log를 DB에 적재하고 SQL로 트래픽과 에러 흐름을 분석하는 도구 | Python, SQLite, MySQL, SQL |
| [inspection-automation](https://github.com/jiyoon99/inspection-automation) | 노트북 검수 항목을 자동 진단, 수동 체크, 최종 판정, 리포트 저장 흐름으로 정리한 GUI 도구 | PowerShell, Windows Forms, WMI/CIM |
| [driver-check-helper](https://github.com/jiyoon99/driver-check-helper) | Windows 장치 상태와 문제 드라이버를 분류하고 공식 지원/검색 링크와 리포트를 생성하는 점검 도구 | PowerShell, Windows Forms, JSON/HTML, Pester |
| [usb-qc-automation](https://github.com/jiyoon99/usb-qc-automation) | USB/하드웨어 출고 전 QC 절차를 터미널 대시보드 흐름으로 자동화한 스크립트 | Batch, PowerShell, Windows |
| [unity-game-portfolio](https://github.com/jiyoon99/unity-game-portfolio) | Unity C# 기반 2D 게임 결과물을 실행 빌드와 구현 문서로 정리한 게임 개발 포트폴리오 | Unity, C#, Windows Build |

## Interview Notes

### Linux Chess Portfolio

- 브라우저가 아니라 서버가 게임 상태를 책임지는 이유
- WebSocket 연결과 방 코드 기반 매칭 구조
- Docker Compose로 개발/운영 구성을 나눈 방식
- Prometheus/Grafana로 어떤 지표를 보고 장애를 판단하는지

### Linux System Monitor

- `/proc`, `/sys`, Docker socket에서 운영 정보를 가져오는 방식
- 컨테이너 내부에서 호스트 리소스를 읽을 때 필요한 volume/network 설정
- 수치만 보여주는 대시보드가 아니라 경고 판단까지 넣은 이유
- 로컬 LLM을 운영 보조 도구로 연결할 때 timeout과 모델 상태를 다룬 방식

### Linux Desktop Widget

- CLI 확인 작업을 계속 반복하지 않도록 GUI 위젯으로 만든 이유
- `GLib.timeout_add()`로 UI를 멈추지 않고 상태를 갱신한 방식
- Docker socket activation 때문에 서비스 상태 판단이 단순하지 않았던 점
- 작은 도구도 실행, 종료, 자동 실행까지 고려해야 실제로 쓰기 좋다는 점

### Linux Web Log SQL Analyzer

- 로그 파일을 바로 보는 것과 DB에 적재해 분석하는 것의 차이
- status code, path, IP, 시간대별 집계가 운영에서 어떤 의미를 갖는지
- 샘플 데이터와 실제 `/var/log/nginx/access.log`를 모두 다룰 수 있게 만든 이유
- CLI 명령을 작게 나눠 재실행 가능한 분석 흐름으로 만든 방식

## Strengths

- 반복 업무를 스크립트로 끝내지 않고, GUI, 리포트, 문서, 실행 방법까지 정리합니다.
- 운영/검수 도구에서 실제 사용자가 놓치기 쉬운 예외와 개인정보 제거 흐름을 고려합니다.
- 프로젝트별 목적, 실행 방법, 구현 포인트를 README에 남겨 검토자가 빠르게 확인할 수 있게 정리합니다.
