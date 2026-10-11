# BGA Mode 0.1.27

ADOFAI의 실제 플레이 화면에서 차트·플레이어 요소·게임 HUD를 숨기고 배경과 VFX를 감상하기 위한 Unity Mod Manager 모드입니다.

## 주요 기능

- 실제 차트 타일, 행성, 꼬리, 판정 표시와 게임 HUD 숨김
- 배경, 카메라 이동, 필터, 플래시, 파티클과 커스텀 UI VFX 유지
- 로비와 커스텀 레벨 선택 화면은 정상 표시
- 레벨 에디터에서는 편집 중 차트를 표시하고, 에디터 플레이 중에만 BGA Mode 적용
- 이펙터가 생성한 장식용 타일을 별도로 숨기는 옵션
- 이펙터가 생성한 행성과 행성 기준 장식을 별도로 숨기는 옵션
- 히트사운드 음소거 옵션
- 기타 게임 효과음과 커스텀 Play Sound 음소거 옵션
- 오른쪽 위 Build Text 숨기기 및 사용자 지정 문구
- 한국어 Build Text 글꼴 지원
- 설정 자동 저장
- 모드매니저에서 한국어·English 즉시 전환 및 선택 언어 저장

노래와 모드매니저·메뉴 조작음은 사운드 옵션의 영향을 받지 않습니다.

## 다운로드

[공개 배포 페이지](https://github.com/cgwoo0704/ADOFAI-BGA-Mode-Downloads/releases/latest)에서 `BgaMode-0.1.27.zip`을 받으세요. 공개 배포 저장소에는 설치 파일과 안내 문서만 있습니다. GitHub가 자동 생성하는 `Source code` 압축 파일에도 모드 소스코드는 없으며, 설치 파일이 아닙니다.

## 설치

1. ADOFAI에 Unity Mod Manager를 먼저 설치합니다.
2. 배포 ZIP을 게임의 `Mods` 폴더에 압축 해제합니다.
3. 다음 구조인지 확인합니다.

```text
Mods/
└─ BgaMode/
   ├─ BgaMode.dll
   ├─ Info.json
   ├─ README.md
   ├─ README_KO.md
   ├─ README_EN.md
   ├─ CHANGELOG.md
   └─ LICENSE
```

4. 게임을 완전히 종료한 뒤 다시 실행합니다.
5. 모드매니저를 열어 `BGA Mode 0.1.27`이 활성 상태인지 확인합니다.

## 사용 방법

모드매니저의 모드 목록에서 `BGA Mode`를 펼치면 상단의 `한국어`와 `English` 버튼으로 언어를 즉시 전환할 수 있습니다. 선택한 언어는 저장되며 다음 실행에서도 유지됩니다.

`BGA Mode 켜기`를 선택하면 다음 하위 옵션이 표시됩니다.

- `이펙터가 생성한 타일도 숨기기`
- `이펙터가 생성한 행성 및 행성 기준 장식도 숨기기`
- `히트사운드 음소거`
- `기타 게임 효과음 음소거`

Build Text 설정은 BGA Mode 적용 여부와 별개로 사용할 수 있습니다.

- `오른쪽 위 Build Text 숨기기`
- `사용자 지정 Build Text 사용`
- `사용자 지정 텍스트`

새 설치의 사용자 지정 문구 기본값은 비어 있습니다. `Build Text 설정 초기화`를 누르면 숨기기와 사용자 지정 사용이 해제되고 저장된 문구가 비워집니다.

설정을 바꾸면 즉시 자동 저장되며 별도의 문구 저장 버튼은 필요하지 않습니다. 설정은 모드 설치 폴더와 별도로 보관되므로 ZIP을 덮어써도 다음 실행에서 유지됩니다.

## 호환 상태

BGA Mode를 켜면 모드매니저 하위 설정에 호환 상태가 표시됩니다.

- `정상`: 편집기·차트·이펙트·사운드 후크가 모두 설치됨
- `일부 기능 확인 필요`: 일부 게임 메서드를 찾지 못했거나 패치하지 못함
- `패치 설치 실패`: 초기 후크 설치 중 예상하지 못한 오류 발생

정상이 아니라면 모드매니저의 Logs 탭에서 `BGA Mode compatibility` 줄을 확인해 주세요.

## 업데이트

게임을 종료한 상태에서 기존 `Mods/BgaMode` 폴더의 `BgaMode.dll`, `Info.json`, `README.md`, `CHANGELOG.md`를 새 파일로 교체합니다. 저장된 사용자 설정은 별도 위치에 있으므로 일반적인 파일 교체로 유지됩니다.

## 삭제

게임을 종료한 뒤 `Mods/BgaMode` 폴더를 제거합니다. 모드를 끄거나 제거해도 차트 판정과 맵 파일 자체는 변경되지 않습니다.

## 문제 보고 시 필요한 정보

GitHub의 [버그 신고 양식](https://github.com/cgwoo0704/ADOFAI-BGA-Mode-Downloads/issues/new/choose)을 사용해 주세요. GitHub 로그인이 필요하며, 공개 글이므로 개인 정보는 적지 마세요.

- BGA Mode 버전
- ADOFAI 빌드와 Unity Mod Manager 버전
- 모드매니저 Logs의 `BGA Mode compatibility` 줄
- 문제가 발생한 화면이 로비·에디터 편집·에디터 플레이·일반 플레이 중 어디인지
- 문제 직전에 수행한 동작
- 가능하다면 짧은 영상이나 스크린샷

## 테스트 환경

- Windows 11
- ADOFAI Alpha Build
- Unity Mod Manager 0.32.5.0

ADOFAI 알파 빌드가 변경되면 호환 상태가 달라질 수 있습니다.

## 제작자와 라이선스

- 제작자: 최건오사임
- 라이선스: MIT License

BGA Mode는 7th Beat Games의 공식 기능이나 공식 모드가 아닌 팬 제작 모드입니다.
