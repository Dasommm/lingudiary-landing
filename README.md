# Lingu Diary — Landing Page

[Lingu Diary](https://apps.apple.com/) 공식 랜딩 페이지.

## 구조

```
public/
├── index.html      메인 랜딩 페이지
└── favicon.svg     파비콘 (mint gradient L)
vercel.json         Vercel 보안 헤더 설정
```

## 로컬에서 보기

```bash
open public/index.html
# 또는 간단한 정적 서버
python3 -m http.server 8000 --directory public
# → http://localhost:8000
```

## 배포

Vercel에 연결되어 있어 main 브랜치 push 시 자동 배포됨.

- 운영 URL: `https://lingudiary.cheeselab.dev` (예정)
- 백업 URL: `https://lingudiary-landing.vercel.app`

## 콘텐츠 업데이트가 필요할 때

- **App Store 링크**: 심사 통과 후 실제 URL로 교체 (`href="#"` → 실제 링크)
- **OG 이미지**: 1200x630 PNG 만든 후 `public/og-image.png` + `<meta property="og:image">` 추가
- **스크린샷**: wireframe phone mockup을 실제 앱 스크린샷 이미지로 교체 가능

## 관련 프로젝트

- 앱 코드: [ai-english-journal](https://github.com/Dasommm/ai-english-journal)
- 법적 페이지: [lingudiary-legal](https://github.com/Dasommm/lingudiary-legal)
