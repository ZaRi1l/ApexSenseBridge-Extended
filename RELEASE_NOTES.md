# ApexSenseBridge Extended — 비공식 베타 (2026-10-29)

APEX 6 Pro에서 PC 게임의 네이티브 DualSense 햅틱 신호를 조절하기 위한 비공식 포크 테스트판입니다. 원본 [ReynArts/ApexSenseBridge](https://github.com/ReynArts/ApexSenseBridge) 제작자에게 감사를 표합니다.

### 수정판 주요 기능
- 게임별 APEX 6 Pro PCM Linear 증폭 (0~1000%) 및 저장
- 좌우 원본·증폭 후 피크 및 클리핑 측정
- 증폭 숫자 입력·슬라이더 반영 동작 개선

### 빌드 근거
- 소스: `dcdeb42222296b40fb94b67e89e06c12f65d06c8`
- [기존 CI 성공 기록](https://github.com/ZaRi1l/ApexSenseBridge/actions/runs/40717411390)
- 별도 배포용 빌드도 같은 고정 커밋을 사용하여 **컴파일·자동 테스트·파일 패키징을 다시 수행**합니다.
- CI 성공은 실물 패드 검증이나 장시간 안정성을 보장하지 않습니다.

### 설치 및 주의
Windows 10/11 x64에서 USB 또는 2.4GHz 동글을 사용합니다. 기존 Bridge와 동시에 실행하지 마세요. 드라이버가 없다면 포함된 `Install-Drivers.cmd`로 설치하고 재부팅합니다. 강한 진동, 비정상 발열 또는 소음이 발생하면 즉시 중지하세요. 실행 파일은 서명되지 않은 테스트 빌드입니다.

### 라이선스 및 소스
GPL-3.0-or-later. [전체 대응 소스 및 빌드 방법](https://github.com/ZaRi1l/ApexSenseBridge-Extended/blob/main/SOURCE-CODE.md) · [전체 GPL v3](https://github.com/ZaRi1l/ApexSenseBridge-Extended/blob/main/COPYING) · [제3자 고지](https://github.com/ZaRi1l/ApexSenseBridge-Extended/blob/main/THIRD_PARTY_NOTICES.md)

**GitHub 자동 생성 Source code ZIP은 배포 프로그램 전체 소스가 아닙니다.** 실제 소스는 고정 커밋 링크에서 확인하세요.
