# GRIMOIRE : Once Upon a Crime — 포트폴리오 웹페이지

기획서(Vol.1) 기반으로 제작한 원페이지 포트폴리오 사이트입니다.
`index.html` 하나와 `assets/` 폴더만 있으면 어디서든 동작합니다.

## 폴더 구조
```
grimoire-portfolio/
├── index.html        ← 사이트 본체 (HTML+CSS+JS 단일 파일)
└── assets/            ← 기획서 PDF에서 추출한 캐릭터 원화·맵·UI 목업
    ├── char-dorothy.jpg
    ├── char-keeper.jpg
    ├── char-oz.jpg
    ├── char-rougehood.jpg
    ├── char-sinderella.jpg
    ├── level-ch01-layout.jpg
    ├── level-clocktower.jpg
    ├── ui-book.jpg
    ├── ui-hud.jpg
    ├── ui-levelup.jpg
    ├── ui-skillmenu.jpg
    ├── ui-wireframes.jpg
    └── world-map.jpg
```

## 로컬에서 바로 확인하기
`index.html`을 브라우저로 더블클릭해서 열면 됩니다. (별도 서버 불필요)

## GitHub Pages로 배포하기 (레퍼런스 사이트와 동일한 방식)
1. GitHub에 새 저장소 생성 (예: `grimoire-portfolio`)
2. 이 폴더 안의 파일들(`index.html`, `assets/`)을 저장소 루트에 그대로 업로드
3. 저장소 **Settings → Pages → Branch**를 `main` / `(root)`로 설정 후 저장
4. 잠시 후 `https://[깃허브아이디].github.io/grimoire-portfolio/` 로 접속 가능

## 이미지 교체(아트북 완성본으로 업데이트할 때)
- `assets/` 폴더의 같은 파일명으로 덮어쓰기만 하면 코드 수정 없이 반영됩니다.
- 새 이미지를 추가하고 싶다면 `index.html` 안의 `<script>` 부분,
  `CHARACTERS`(캐릭터 카드)와 `ART`(하단 갤러리) 배열에 항목을 추가하면 됩니다.
  예)
  ```js
  { img:"assets/새파일명.jpg", en:"...", name:"...", desc:"..." }
  ```

## 아직 비어있는 섹션 (원하시면 이어서 채워드릴게요)
- Ch.03 오즈 보스전 시스템 상세(현재 캐릭터 카드까지만 반영, 잠금 스포일러 항목 제외)
- 실제 게임 스크린샷/플레이 영상 (유튜브 임베드 등)
- 03~09번 미구현 구역(Crossroads Track ~ Mirror Heights) 소개 카드
- 사운드 트랙 재생 플레이어 (SoundCloud/유튜브 embed)
- press kit(로고 파일, 스크린샷 zip 등 다운로드) 섹션

## 디자인 컨셉 메모
- 색상은 기획서의 "색의 언어"를 그대로 시스템화했습니다.
  보라(진실)=`#a78bfa`, 빨강(부정)=`#e5484d`, 파랑(도피)=`#4fb0e6`, 초록(죽음)=`#2fa876`
- 히어로의 `UnTruth` 로고는 기획서에 적힌 "'Un'이 탈락 → 'Truth'가 드러남" 글리치 연출을 그대로 구현했습니다.
- 신데렐라 vs 루주후드 보스전은 "같은 뼈대, 정반대 춤"이라는 기획 의도를 대칭 테이블로 시각화했습니다.
