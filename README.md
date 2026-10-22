# 인터벌 타이머 (무료 웹앱)

서버 없이 동작하는 웹앱입니다. 설정, 저장한 설정, 운동 기록은 모두 각 사용자의 휴대폰 브라우저 안에만 저장되며 어디로도 전송되지 않습니다. 글꼴은 Google Fonts에서 불러옵니다.

## 파일 구성
- `index.html` : 앱 본체
- `manifest.webmanifest` : 홈 화면 설치용 정보(이름, 아이콘)
- `sw.js` : 한 번 열면 인터넷 없이도 실행되도록 파일을 보관
- `icons/` : 앱 아이콘

## 무료 배포 (GitHub Pages)
1. github.com 에 가입합니다.
2. 새 저장소(New repository)를 Public으로 만듭니다. 예: `interval-timer`
3. Add file → Upload files 에서 이 폴더의 파일과 `icons` 폴더를 모두 올리고 Commit changes를 누릅니다.
4. Settings → Pages 에서 Source를 Deploy from a branch, Branch를 main / (root)로 두고 Save를 누릅니다.
5. 1~2분 뒤 `https://아이디.github.io/interval-timer/` 주소로 열립니다.

## 휴대폰에 설치
- 아이폰: 사파리로 주소를 연 뒤 공유 버튼 → 홈 화면에 추가
- 안드로이드: 크롬으로 주소를 연 뒤 메뉴 → 홈 화면에 추가 또는 앱 설치

아이폰은 홈 화면에 추가해 쓰는 편이 기록 보관에 유리합니다. 사파리 탭으로만 쓰면, 사파리를 쓰는 동안 7일 넘게 방문하지 않은 사이트의 저장 데이터가 지워질 수 있습니다.

## 업데이트
수정한 `index.html`을 같은 방법으로 다시 올리면, 사용자가 인터넷에 연결된 상태로 앱을 열 때 새 버전이 적용됩니다. `sw.js`의 보관 파일 목록을 바꿀 때는 `CACHE` 이름의 숫자(v1 → v2)도 올려 주세요.

## 백업
앱의 기록 화면 → 백업 → 내보내기로 기록과 저장한 설정을 파일로 받을 수 있고, 가져오기로 되살릴 수 있습니다.
