# SarangInChrist.github.io — 사랑교회 홈페이지

대전 대덕구 **사랑교회** 홈페이지 저장소입니다.

🔗 **사이트 주소: https://saranginchrist.github.io**

## 구조

- [`index.html`](index.html) — 홈페이지 전체가 담긴 단일 파일입니다.
  스타일, 스크립트, 이미지(로고·사진 포함)가 모두 이 파일 안에 들어 있어 다른 파일이 필요 없습니다.

## 홈페이지 업데이트 방법

목사님께서 새 홈페이지 HTML 파일을 보내주시면:

1. 받은 파일을 이 저장소의 `index.html`로 덮어씁니다 (파일 이름을 `index.html`로 변경).

   ```bash
   mv ~/Downloads/사랑교회-홈페이지.html index.html
   ```

2. 커밋하고 푸시합니다.

   ```bash
   git add index.html
   git commit -m "홈페이지 업데이트"
   git push
   ```

3. 1~2분 뒤 https://saranginchrist.github.io 에서 반영을 확인합니다.
   (바로 안 보이면 브라우저 새로고침을 강력 새로고침(Cmd+Shift+R)으로 해보세요.)

## 내용 수정 위치

`index.html` 상단의 관리자 주석에도 안내되어 있습니다:

| 수정할 내용 | 위치 |
|---|---|
| 예배 시간 | 맨 아래 `<script>`의 `SERVICES` 배열 |
| 설교 영상 | 맨 아래 `<script>`의 `YT_PLAYLIST_ID` |
| 전화번호 | "오시는 길" 섹션과 푸터 |
| 사진 | 부서 카드의 `<img class="ph">` |

## 참고

- `.nojekyll` — GitHub Pages의 Jekyll 빌드를 생략하고 파일을 그대로 서빙하기 위한 표시 파일입니다. 지우지 마세요.
