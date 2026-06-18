# DNF Weekly Widget

던전앤파이터 캐릭터들의 주간 콘텐츠 진행 상태를 한 화면에서 확인하는 Windows용 어플리케이션입니다.

여러 캐릭터를 관리할 때 “이번 주에 무엇이 남았는지”를 빠르게 보는 용도로 사용하시면 됩니다.

## 다운로드

최신 배포 파일은 Release 페이지에서 받을 수 있습니다.

[DNFWeeklyWidget Releases](https://github.com/acityboy-dev/DNFWeeklyWidget.Release/releases)

ZIP 파일을 원하는 폴더에 압축 해제한 뒤 `DNFWeeklyWidget.exe`를 실행하면 됩니다.

첫 실행 시 Windows SmartScreen 경고가 표시될 수 있습니다. 배포 파일은 이 저장소의 GitHub Release에서만 받는 것을 권장합니다.

업데이트가 있으면 앱이 실행 시 자동으로 알려줍니다. 첫 설치 이후에는 새 버전 확인을 위해 Release 페이지를 주기적으로 방문할 필요가 없습니다.

## 주요 기능

- 캐릭터별 명성, 직업, 서버 표시
- 레기온/레이드 등 주간 콘텐츠 완료 여부 표시
- 주간 획득 정보 표시
- 미완료 캐릭터만 보기
- 캐릭터 카드 드래그 정렬 및 삭제
- 프리셋별 캐릭터 목록 관리
- 던담 모험단 기준 캐릭터 목록 교체, 추가 및 제외
- 카드 표시 방식, 테마, 자동 갱신 등 기본 설정 지원
- 앱 업데이트 확인 및 자동 패치 지원

## 사용 방법

1. [Neople Developers](https://developers.neople.co.kr/)에서 아무 방식으로 로그인합니다.
2. 마이페이지로 들어가 애플리케이션 등록을 누릅니다. 내용은 임의로 적어도 무방하고, 등록을 눌러 API Key를 발급받습니다.
3. 앱을 실행하고 `설정`에서 API Key를 입력합니다.
4. 서버와 캐릭터명을 선택해 캐릭터를 추가합니다.
5. 던담 모험단 불러오기는 현재 프리셋의 목록을 교체하며, 옵션을 사용하면 기존 목록에 덧붙이거나 일치하는 캐릭터를 제외할 수 있습니다.
6. `지금 갱신` 또는 `F5`로 상태를 갱신합니다.
7. 필요에 따라 미완료 필터, 카드/줄 수, 표시할 주간 콘텐츠를 조정합니다.
8. 다계정이나 모험단 캐릭터가 매우 많은 경우, 앱 윈도우 좌측의 확장 버튼을 눌러 프리셋 기능을 이용하여 나눠둘 수 있습니다.

## 설정

설정창에서 다음 항목을 조정할 수 있습니다.

- API Key
- 자동 갱신 및 갱신 주기
- 실행 시 업데이트 확인
- 윈도우 부팅 시 자동 실행
- 테마와 저성능 모드
- 캐릭터 이미지 표시 방식
- 카드/줄 수
- 표시할 주간 콘텐츠

## 저장 위치

설정과 캐릭터 목록은 사용자 PC에 저장됩니다.

```text
%AppData%\DNFWeeklyWidget\settings.json
```

캐릭터 이미지는 다음 폴더에 캐시됩니다.

```text
%AppData%\DNFWeeklyWidget\ImageCache
```

API Key는 Windows 사용자 계정에 연결된 암호화 방식으로 설정 파일에 저장됩니다. 다른 Windows 사용자 계정에서는 복호화할 수 없습니다.

## 참고

- 이 앱은 게임 클라이언트를 조작하지 않습니다.
- 캐릭터 정보 조회에는 Neople OpenAPI가 필요합니다.
- 외부 서비스 응답 변경에 따라 일부 조회 기능이 일시적으로 동작하지 않을 수 있습니다.

## 소스 코드

소스 코드는 [DNFWeeklyWidget](https://github.com/acityboy-dev/DNFWeeklyWidget) 저장소에 공개되어 있으며, 저장소를 내려받아 직접 빌드할 수 있습니다.

[PolyForm Noncommercial License 1.0.0](https://github.com/acityboy-dev/DNFWeeklyWidget/blob/main/LICENSE)이 적용됩니다. 비상업적 개인 사용과 수정은 허용되지만 상업적 이용 및 유료 재배포는 허용되지 않습니다.
