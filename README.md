# X Operations (모바일 터치판) 업데이트

최신 빌드는 **[Releases › latest](../../releases/tag/latest)** 에 있습니다. 항상 최신 하나만 있습니다.

- `XOperations.apk` — 최신 빌드
- `version.txt` — 그 빌드의 버전 번호 (touchN의 N, 앱의 versionCode)
- `changes.txt` — 업데이트 알림에 보이는 「이번에 바뀐 것」 (한 줄에 하나)

앱은 하루 한 번(또는 설정의 「업데이트 확인」) 릴리스의 `version.txt`를 읽고, 설치된 버전보다
높으면 `XOperations.apk`를 안드로이드 다운로드 관리자로 받아 설치 화면을 엽니다.
같은 서명 키로 서명된 빌드만 덮어쓰기 설치가 됩니다.

새 빌드 올리기: `upload` 브랜치에 위 세 파일을 넣어 push하면 `publish` 작업이 릴리스의 파일을
바꾸고 `upload` 브랜치를 지웁니다 (저장소 안에는 apk가 남지 않음).
