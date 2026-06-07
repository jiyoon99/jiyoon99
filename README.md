<div align="center">

# 박지윤

### Linux Kernel · Backend · Linux Operations · Automation · AI-Assisted Development

반복되는 점검과 운영 작업을 자동화하고, 시스템 상태를 관찰 가능한 도구와 서비스로 만드는 개발을 하고 있습니다.

<p>
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" />
  <img src="https://img.shields.io/badge/Java%20Spring-6DB33F?style=flat-square&logo=springboot&logoColor=white" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white" />
  <img src="https://img.shields.io/badge/PowerShell-5391FE?style=flat-square&logo=powershell&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
</p>

</div>

## About Me / 소개

- Linux 커널 모듈부터 사용자 공간 CLI, TUI, 수집기, 패키징까지 연결한 드라이버 실습 환경을 구현했습니다.
- Java/Spring Boot와 Go로 인증, 데이터 저장, 실시간 통신이 포함된 백엔드 서비스를 개발했습니다.
- FastAPI, Docker, nginx, Prometheus, Grafana를 활용해 시스템 상태를 수집하고 운영 흐름을 시각화했습니다.
- PowerShell과 Windows Forms로 노트북 검수, 드라이버 확인, 출고 QC 작업을 자동화했습니다.
- AI는 요구사항 분해, 코드 검토, 문서화뿐 아니라 Ollama 기반 로컬 시스템 분석 기능에도 연결해 사용했습니다.

## Technical Areas / 기술 영역

| 영역 | 기술과 구현 경험 |
| --- | --- |
| Linux Kernel | C, kernel module, procfs, character device, ioctl ABI, poll, sysfs, debugfs, tracepoints, DKMS |
| Backend | Java, Spring Boot, Spring Security, JPA, QueryDSL, Go, FastAPI, REST API, WebSocket |
| Data | PostgreSQL, MySQL, Redis, SQLite, schema design, SQL aggregation |
| Operations | Linux, Docker Compose, nginx, Caddy, systemd, Prometheus, Grafana, Alertmanager |
| Automation | PowerShell, Windows Forms, WMI/CIM, Batch, Bash, Pester |
| AI | Ollama local API, structured diagnostics, prompt safety, human approval workflow |
| Quality | GitHub Actions, unit/integration tests, smoke tests, ShellCheck, ABI layout tests |

## Projects / 프로젝트

### Systems & Linux

| 프로젝트 | 만든 것 | 주요 구현 |
| --- | --- | --- |
| [Kernel Proc Lab](https://github.com/jiyoon99/kernel-proc-lab) | 커널 상태와 이벤트를 사용자 공간에서 관찰·제어하는 Linux kernel module lab | `/proc`, character device, ioctl ABI v4, retained ring buffer, `poll`, sysfs/debugfs/tracepoint, `labtop` TUI, JSONL collector, DKMS/Debian packaging |
| [Linux System Monitor](https://github.com/jiyoon99/linux-system-monitor) | Linux 리소스, Docker, Ollama 상태를 한 화면에서 확인하는 운영 대시보드 | FastAPI, `/proc`·`/sys` metrics, Docker socket, Server Bot, Chart.js, nginx, Ollama 분석 API |
| [Linux Desktop Widget](https://github.com/jiyoon99/linux-desktop-widget) | Docker, 로컬 포트, Ollama 상태를 3초마다 표시하는 GTK 위젯 | Python, GTK 3, GLib timer, Docker CLI, TCP health check, Ollama `/api/tags`, autostart |
| [Linux Web Log SQL Analyzer](https://github.com/jiyoon99/linux-web-log-sql-analyzer) | 웹 access log와 SQL 실행 로그를 SQLite에 적재해 분석하는 CLI·대시보드 | nginx/Apache parser, MySQL slow log parser, deduplication, SQL aggregation, CSV/JSON export, FastAPI |

### Backend & Full Stack

| 프로젝트 | 만든 것 | 주요 구현 |
| --- | --- | --- |
| [FieldOps AI](https://github.com/jiyoon99/fieldops-ai) | 설비 점검, 장애 티켓, 운영 대시보드, 진단 보조를 연결한 멀티테넌트 플랫폼 | React PWA, FastAPI, SQLAlchemy, RBAC, organization-scoped query, audit trail, structured diagnostics |
| [Linux Chess Portfolio](https://github.com/jiyoon99/linux-chess-portfolio) | 서버가 게임 상태를 관리하는 실시간 멀티플레이 체스 서비스 | Go REST/WebSocket, React, PostgreSQL, Redis, Stockfish, Docker Compose, metrics, browser smoke test |
| [EAT US](https://github.com/jiyoon99/shop) | 카페·음식점 정보를 등록하고 조회하는 Spring Boot 웹 서비스 | 회원/권한, JPA entity, QueryDSL 검색, 이미지 업로드, 장바구니, 주문, Thymeleaf |

### Windows Automation

| 프로젝트 | 만든 것 | 주요 구현 |
| --- | --- | --- |
| [Driver Check Helper](https://github.com/jiyoon99/driver-check-helper) | 문제 장치를 분류하고 공식 드라이버 검색 경로와 리포트를 생성하는 도구 | PowerShell, Windows Forms, Hardware ID 분석, 제조사 규칙, JSON/HTML report, Pester |
| [Notebook Inspection Automation](https://github.com/jiyoon99/inspection-automation) | 자동 하드웨어 진단과 수동 검수를 합쳐 최종 판정하는 GUI | WMI/CIM, `powercfg`, 포트·키보드 검사, 합격/재검수/불합격 판정, CSV/PDF output |
| [USB QC Automation](https://github.com/jiyoon99/usb-qc-automation) | 출고 전 USB·하드웨어 QC 절차를 순서대로 실행하는 터미널 대시보드 | Batch, PowerShell, USB 탐색, 시스템 정보, Bluetooth·배터리·카메라 검사, UEFI reboot option |

### Development Workflow & Game

| 프로젝트 | 만든 것 | 주요 구현 |
| --- | --- | --- |
| [AI Development Team Playbook](https://github.com/jiyoon99/ai-development-team-playbook) | 개발 요청을 역할별 작업과 품질 게이트로 연결하는 AI 협업 운영 규칙 | PM classification, risk sizing, scoped delegation, security/data/AI gates, QA verification |
| [Unity Game Portfolio](https://github.com/jiyoon99/unity-game-portfolio) | Unity 2D 게임 결과물과 Windows 실행 빌드를 정리한 포트폴리오 | C#, player/enemy loop, weapon/projectile, item/level system, object pooling, HUD |

## Development Approach / 개발 방식

1. 반복되거나 판단 기준이 흔들리는 작업을 먼저 구체적인 입력과 출력으로 정의합니다.
2. UI, API, 데이터, 운영 경계를 나누고 각 계층의 책임을 코드 구조에 반영합니다.
3. 사용자의 입력과 외부 로그는 신뢰하지 않고 검증, 권한 확인, 마스킹을 적용합니다.
4. 로컬 실행 명령, Docker 구성, 테스트, 상태 확인 경로를 함께 만들어 재현 가능한 결과물로 정리합니다.
5. 구현 결과는 README, 구조도, 샘플 데이터, 운영 문서로 남겨 코드와 사용 흐름을 함께 확인할 수 있게 합니다.

## Links

- GitHub: <https://github.com/jiyoon99>
