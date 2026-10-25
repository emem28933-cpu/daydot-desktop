# Daydot 윈도우 앱

Daydot 웹앱(https://deluxe-cucurucho-d8c3ad.netlify.app)을 감싼 윈도우 프로그램입니다.
Netlify에 새 버전을 올리면 이 프로그램에도 자동으로 반영됩니다. (exe를 다시 만들 필요 없음)

## 설치 파일 받기
1. 이 저장소의 **Actions** 탭 → **Build Windows app**
2. 가장 최근 실행(초록 체크) 클릭 → 아래 **Artifacts** 의 `Daydot-Windows-Installer` 다운로드
3. 압축을 풀고 `Daydot_..._x64-setup.exe` 실행
   - "Windows의 PC 보호" 창이 뜨면 **추가 정보 → 실행** (서명하지 않은 개인 앱이라 뜨는 정상 경고)

다시 빌드하려면 Actions → Build Windows app → **Run workflow**.

## 처음 실행 후
PC 앱은 저장 공간이 따로라서 한 번 설정해야 합니다.
설정 ⚙ → 로그인 · 친구 공유 → 서버 주소/키 입력 → 로그인 → ☁ 동기화

설정의 "반투명 창", "다른 창 위에 항상 표시"는 이 PC 앱에서만 동작합니다.

## 사이트 주소가 바뀌면
`src-tauri/tauri.conf.json` 의 `url`, `src-tauri/capabilities/default.json` 의 `remote.urls`, `offline/index.html` 의 주소를 함께 바꾸세요.
