# myroom-answers

myroom(기술사 공부방) 답안 스캔 이미지 저장소. 2026-11-01 부터 새 답안 이미지는 여기에 넣는다
(본 저장소가 3.6GB 가 되어 세션마다 받는 데 오래 걸려서).

- 경로: `{출처 폴더}/파일.webp` — 출처 폴더는 myroom `public/answers` 와 같은 규칙
  (`기출해설집/{정보관리|컴시응}/{회}회`, `NS19기/{주}주차/{해설집|답안지}`, `KPC모의고사/{회}회`, `ITPE모의고사/…` …)
- myroom 답안 `pages[].src` 는 `/ans2/{출처 폴더}/파일.webp` 로 적는다 —
  myroom `next.config.mjs` 의 `/ans2/:path*` rewrite 가 `raw.githubusercontent.com/yjnam-afk/myroom-answers/main/:path*` 로 넘긴다.
- 공개 저장소여야 한다(비공개면 raw 주소가 404).
- 한 폴더가 1,000장에 가까워지면 하위 폴더로 나눈다(GitHub 은 폴더당 1,000개까지만 보여 준다).
