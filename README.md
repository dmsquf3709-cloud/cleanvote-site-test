# CleanVote 사이트 (정적)

올림픽공원 자원봉사 보급 현황 사이트. 순수 정적(HTML/JS) — 데이터는 런타임에 공개 구글시트(gviz)에서 읽음.

## 구성
- `index.html` — 단일 페이지(현황판/후원폼 배너/지도)
- `*.jpg` — 게이트/화장실/배달존 지도

## 배포 (Netlify)
- 라이브: https://cleanvote0605.netlify.app
- 자동배포: 이 repo에 push → Netlify가 빌드 없이 정적 배포 (publish dir = repo root)
- **시크릿(배포 토큰 등)은 repo에 없음.** Netlify 환경/계정 측에 보관.

## 주의
- 후원자 PII·시크릿은 이 repo에 절대 넣지 말 것 (.gitignore 참조).
- 데이터 소스(구글시트)·필터 파이프라인은 별도 비공개 운영.
