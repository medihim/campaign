# IPPEO Task Portal v1.2

GitHub Pages 배포용 완전 패키지입니다.

## 중요 수정
v1.1 패키지에는 `index.html`이 참조하는 `docs/` 파일이 ZIP에서 누락되어 404가 발생했습니다.
v1.2에서는 모든 상대 링크 대상 파일을 실제로 포함하고 링크 존재 여부까지 검증했습니다.

## 구조
```text
/
├─ index.html
├─ .nojekyll
├─ README.md
├─ VERSION.md
├─ DEPLOY_GITHUB_PAGES.md
└─ docs/
   ├─ operating-framework-v2.4.html
   ├─ landing-ko-v1.0.html
   ├─ landing-ja-v1.0.html
   ├─ landing-revision-v1.1.html
   └─ ads-setting-v0.1.html
```

## 비밀번호
`5153370`

> 정적 HTML의 클라이언트 측 접근 제한입니다.