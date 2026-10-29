# ApexSenseBridge Extended — 비공식 한국어 배포

**Flydigi APEX 6 Pro에서 DualSense 지원 PC 게임의 햅틱 진동을 게임별로 증폭·측정할 수 있도록 수정한 무료 오픈소스 테스트판입니다.**

> ⚠️ **비공식 베타**입니다. 원작자(ReynArts)의 공식 배포판이 아니며, 실기기에서 모든 게임·연결 방식·장시간 안정성이 검증된 것은 아닙니다. 실행 파일은 공식 코드 서명이 없는 개발 빌드입니다.

## 다운로드

**[Releases — 배포 파일 받기](https://github.com/ZaRi1l/ApexSenseBridge-Extended/releases)**

1. Releases에서 최신 **Pre-release**를 엽니다.
2. **Assets** 아래의 `ApexSenseBridge-Extension-*.zip`을 다운로드합니다. GitHub의 기본 **Source code (zip)**은 설치 파일이 아닙니다.
3. 압축을 풀고 아래 사용법대로 실행합니다.

릴리스가 아직 표시되지 않는다면 실행 파일이 **미배포 상태**입니다. 원본 프로젝트의 파일을 수정판으로 혼동하지 마세요.

## 처음 사용하는 분을 위한 사용법

**준비물:** Windows 10/11 64비트, Flydigi APEX 6 Pro (원본에서 APEX 4/5도 지원), **유선 USB 또는 2.4GHz 동글**. APEX 4는 DInput 모드를 사용합니다. Bluetooth는 이 가이드의 지원 연결 방식이 아닙니다.

1. **기존 프로그램 종료**: 원본 ApexSenseBridge/Playnite 자동화와 이 수정판을 동시에 실행하지 마세요. APEX 6 Pro를 시험할 때는 Flydigi Space Station 및 X-Haptics Engine도 종료해 비교하세요.
2. **필요한 경우에만 드라이버 설치**: 처음 쓰는 PC라면 폴더의 `Install-Drivers.cmd`를 실행해 관리자 권한 요청을 승인하고 안내에 따라 재부팅합니다. USBip·HidHide가 이미 정상 설치된 경우 **재설치하지 마세요**. 포터블 앱이어도 Windows 드라이버 설치는 필요합니다.
3. **앱 실행**: `Start-ApexSenseBridge.cmd`를 실행하고 트레이에서 연결 상태를 확인합니다.
4. **게임 실행**: PC에서 네이티브 DualSense를 지원하는 게임을 실행합니다. Steam에서 게임 **속성 → 컨트롤러 → Steam Input 사용 안 함**을 설정해야 할 수 있습니다.
5. **진동 조절**: 해당 게임의 APEX 6 PCM **Linear** 증폭을 **100%부터** 시작하여 서서히 조절합니다. 1000%는 최대 신호 배율일 뿐 실제 진동력이 10배라는 뜻이 아닙니다.
6. **진동 측정**: 원본 신호 피크·증폭 후 피크·클리핑 수치를 참고하세요. 수치는 모터의 실제 물리적인 힘이나 안전성을 측정한 값이 아닙니다.

게임에서 패드를 인식하지 못하면 게임을 종료한 뒤 트레이에서 **Force continuous activation**을 켜서 **Bridge active**를 확인하고 게임을 다시 시작하세요. [원본 기반 상세 문제 해결](https://github.com/ZaRi1l/ApexSenseBridge/blob/Extension/TROUBLESHOOTING.md)

### 추가된 기능
- APEX 6 Pro 게임별 PCM **선형 증폭 0~1000%** 및 저장
- 좌·우 원본/증폭 후 피크 실시간 측정, 포화(클리핑) 수치
- 배율 숫자 입력과 슬라이더 동기화 개선

### 주의사항
- **과열·이상 소음·거친 진동**이 발생하면 즉시 사용 중지하고 배율을 낮추세요.
- `%LOCALAPPDATA%\ApexSenseBridge\tray_settings.json` 등 설정과 USBip/HidHide 드라이버가 원본과 **공유**될 수 있습니다. 원본과 비교 전 설정을 백업하세요.
- 보안 경고가 발생할 수 있습니다. 출처를 확인하고 **Windows 보안 기능을 끄지 마세요**.
- 모든 게임에서 PCM 진동이 활성화되는 것은 아닙니다. 게임이 가상 패드를 다시 인식하지 못하면 게임 재시작이 필요할 수 있습니다.

## 소스코드 · 라이선스

**GNU GPL-3.0-or-later**. 프로그램을 무료로 사용·수정·재배포할 수 있지만, 재배포 시 GPL의 소스 제공 및 고지 조건을 지켜야 합니다.

- [LICENSE](LICENSE) · [GPL v3 전문](COPYING) · [외부 구성요소 고지](THIRD_PARTY_NOTICES.md)
- **원본 프로젝트**: [ReynArts/ApexSenseBridge](https://github.com/ReynArts/ApexSenseBridge)
- **수정판 개발 소스**: [ZaRi1l/ApexSenseBridge, Extension](https://github.com/ZaRi1l/ApexSenseBridge/tree/Extension)
- **이 초기 베타 빌드에 대응하는 고정 커밋**: [`dcdeb42222296b40fb94b67e89e06c12f65d06c8`](https://github.com/ZaRi1l/ApexSenseBridge/tree/dcdeb42222296b40fb94b67e89e06c12f65d06c8)
- **전체 대응 소스·빌드 정보**: [SOURCE-CODE.md](SOURCE-CODE.md)

**중요:** 이곳은 배포 안내 및 실행 파일을 제공하는 저장소입니다. GitHub가 이 저장소에 자동 생성하는 `Source code (zip)`에는 프로그램의 전체 대응 소스가 **포함되지 않습니다**. 위 고정 소스코드 링크를 사용하세요. 배포물의 라이선스와 제3자 고지 내용도 함께 유지해야 합니다.

## 오류 제보

[Issues](https://github.com/ZaRi1l/ApexSenseBridge-Extended/issues)에 **Windows 버전, 패드 모델·펌웨어, 유선/동글, 게임 이름, 재현 과정**을 알려주세요. 로그나 스크린샷에 개인정보가 포함되지 않도록 확인해 주세요.
