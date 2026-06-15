# DNFWeeklyWidget Release Metadata

이 저장소는 DNFWeeklyWidget의 소스 코드나 빌드 결과물을 브랜치에 보관하는 저장소가 아닙니다.

앱의 자동 업데이트 확인에 필요한 최신 버전 정보는 `main` 브랜치의 [`update.json`](./update.json)에서 관리합니다. 실제 배포 ZIP은 Git 커밋에 포함하지 않고 [GitHub Releases](../../releases)에 Release Asset으로 업로드합니다.

## update.json

- `version`: 앱이 최신 버전 여부를 판단할 원격 버전
- `packageUrl`: GitHub Release Asset의 직접 다운로드 URL
- `sha256`: 다운로드한 ZIP의 무결성 검증 해시
- `executable`: 업데이트 후 다시 실행할 앱 파일명

자동 업데이트 클라이언트는 `update.json`을 조회하고, 로컬 버전보다 원격 버전이 높으면 지정된 Release Asset을 다운로드해 검증한 뒤 업데이트를 진행합니다.

최신 배포 파일을 직접 받으려면 [Releases](../../releases) 페이지를 이용하세요.

소스 코드와 개발 내역은 [acityboy-dev/DNFWeeklyWidget](https://github.com/acityboy-dev/DNFWeeklyWidget)에서 관리합니다.
