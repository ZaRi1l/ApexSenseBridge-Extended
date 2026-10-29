# ApexSenseBridge Extended

**APEX 6 Pro 듀얼센스 햅틱 진동 개선판 — 무료 · 비공식 베타**

기존 [ApexSenseBridge](https://github.com/ReynArts/ApexSenseBridge)를 수정하여 **게임별 진동 증폭과 실시간 강도 측정** 기능을 추가한 버전입니다. 원작자의 공식 배포판이 아닙니다.

## 📥 다운로드

**[▶ 포터블 ZIP 다운로드](https://github.com/ZaRi1l/ApexSenseBridge-Extended/releases/download/extension-2026.10.29-beta.1/ApexSenseBridge-Extended-Preview-20261029.zip)**

[배포 버전 및 변경 내역 보기](https://github.com/ZaRi1l/ApexSenseBridge-Extended/releases)

> **주의:** GitHub의 `Source code (zip)`이 아니라 위 **포터블 ZIP**을 받으세요.

## 🎮 설치 및 사용법

**준비물:** Windows 10/11 (64비트), Flydigi APEX 6 Pro, **USB 케이블 또는 2.4GHz 동글**. (원본 프로그램은 APEX 4/5도 지원하지만, 이 수정판의 증폭 기능은 APEX 6 Pro용입니다.)

1. ZIP 파일을 내려받아 **압축 해제**합니다.
2. **최초 설치 시** 드라이버가 없다면 `Install-Drivers.cmd` 실행 → 안내에 따라 **재부팅**. 이미 USBip·HidHide가 정상 설치되어 있다면 이 단계는 건너뛰세요.
3. 패드를 연결하고 **`ApexSenseBridgeTray.exe`를 실행**합니다. (`Start-ApexSenseBridge.cmd`로 실행해도 동일합니다.)
4. DualSense 지원 PC 게임을 실행합니다. **Steam 게임은 해당 게임의 Steam Input을 비활성화**해야 할 수 있습니다.
5. 게임별 **APEX 6 PCM → Linear** 증폭을 **100%부터 조금씩** 조절합니다.

**주요 기능:** 게임별 선형 증폭(0~1000%), 원본/증폭 후 좌우 진동 피크 측정, 클리핑 표시, 게임별 설정 저장.

**패드 인식이 안 된다면?** 게임을 종료하고 앱의 **Force continuous activation**을 켠 뒤, **Bridge active** 상태에서 게임을 다시 실행해 보세요. [자세한 문제 해결](https://github.com/ZaRi1l/ApexSenseBridge/blob/Extension/TROUBLESHOOTING.md)

## ⚠️ 사용 전 참고

- 기존 ApexSenseBridge와 **동시에 실행하지 마세요.** 두 버전은 드라이버와 일부 설정을 공유합니다.
- **1000%는 신호 증폭 설정값**이지 실제 진동력이 10배라는 의미는 아닙니다. 과열·이상 소음·거친 진동이 느껴지면 즉시 사용을 중단하세요.
- 공식 서명이 없는 **테스트 빌드**이며, 모든 게임·환경에서의 동작과 장시간 안정성이 보장되지는 않습니다. Windows 보안 기능을 끄지 마세요.

## 📄 원작자 · 라이선스 · 소스코드

- 원작: [ReynArts/ApexSenseBridge](https://github.com/ReynArts/ApexSenseBridge)
- 라이선스: **GPL-3.0-or-later** ([전문](LICENSE) · [제3자 고지](THIRD_PARTY_NOTICES.md))
- **이번 배포본에 대응하는 실제 소스:** [개발용 포크의 고정 커밋](https://github.com/ZaRi1l/ApexSenseBridge/tree/dcdeb42222296b40fb94b67e89e06c12f65d06c8) · [소스·빌드 안내](SOURCE-CODE.md)

사용 중 문제가 있다면 [Issues에 오류 제보](https://github.com/ZaRi1l/ApexSenseBridge-Extended/issues)해 주세요.
