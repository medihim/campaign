# GitHub Pages 배포

1. ZIP을 압축 해제합니다.
2. 내부 파일을 GitHub 저장소 루트에 모두 업로드합니다.
3. `docs/` 폴더를 반드시 함께 업로드합니다.
4. Settings → Pages → Deploy from a branch → main → / (root)
5. 저장 후 생성된 Pages URL에서 확인합니다.

주의:
`index.html`만 단독 업로드하면 개별 문서 링크는 다시 404가 발생합니다.
반드시 본 패키지의 전체 폴더 구조를 유지해야 합니다.