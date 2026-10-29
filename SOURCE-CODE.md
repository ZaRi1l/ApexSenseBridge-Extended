# 대응 소스코드 / Corresponding Source

이 저장소는 **배포 안내 및 Releases 저장소**입니다. 실제 프로그램 전체 소스코드는 별도 공개 개발용 포크에 있습니다.

- **원본 프로젝트 / Original:** https://github.com/ReynArts/ApexSenseBridge
- **수정판 개발 저장소 / Fork:** https://github.com/ZaRi1l/ApexSenseBridge
- **초기 베타 ZIP에 정확히 대응하는 커밋 / Exact revision:** `dcdeb42222296b40fb94b67e89e06c12f65d06c8`
- **고정된 전체 소스 트리 / Source:** https://github.com/ZaRi1l/ApexSenseBridge/tree/dcdeb42222296b40fb94b67e89e06c12f65d06c8
- **빌드 워크플로 / Build workflow:** https://github.com/ZaRi1l/ApexSenseBridge/blob/dcdeb42222296b40fb94b67e89e06c12f65d06c8/.github/workflows/extension-packages.yml
- **빌드 스크립트 / Scripts:** https://github.com/ZaRi1l/ApexSenseBridge/tree/dcdeb42222296b40fb94b67e89e06c12f65d06c8/scripts
- **원본 및 수정 이력 / Commit:** https://github.com/ZaRi1l/ApexSenseBridge/commit/dcdeb42222296b40fb94b67e89e06c12f65d06c8
- **이 배포 저장소에서 다시 빌드하는 워크플로:** [.github/workflows/publish-beta.yml](.github/workflows/publish-beta.yml)
- **제3자 라이선스·패치:** https://github.com/ZaRi1l/ApexSenseBridge/blob/dcdeb42222296b40fb94b67e89e06c12f65d06c8/THIRD_PARTY_NOTICES.md

서브모듈을 포함한 소스 받기:

```bash
git clone https://github.com/ZaRi1l/ApexSenseBridge.git
cd ApexSenseBridge
git checkout dcdeb42222296b40fb94b67e89e06c12f65d06c8
git submodule update --init --recursive
```

### 배포와 소스코드 관련 참고

- 이 배포용 저장소에서 GitHub가 자동 생성하는 `Source code (zip)`은 **프로그램 전체 소스가 아닙니다.** 이 문서의 고정 커밋 링크를 사용하세요.
- 실행 파일과 대응 소스코드는 같은 커밋을 기준으로 제공해야 합니다. 배포 기간 동안 해당 소스와 필요한 스크립트 및 라이선스 고지를 이용할 수 있도록 유지해야 합니다.
- 새 버전을 배포할 때에는 반드시 **실제로 빌드한 커밋**을 가리키도록 이 문서와 릴리스 설명을 갱신하고 배포 파일의 대응 관계를 확인하세요.
- GPL 구성요소와 제3자 의존성의 소스 제공·고지·재배포 조건을 확인해야 합니다. 이 문서만으로 모든 법적 의무가 자동 충족되는 것은 아닙니다.

License for the modified ApexSenseBridge program: `GPL-3.0-or-later`. Bundled third-party software retains its respective license.
