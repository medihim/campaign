# GitHub Pages 배포 방법

## 1. GitHub 저장소 생성

예시:
- Repository: `ippeo-task-portal`

## 2. 파일 업로드

본 폴더의 모든 파일과 `docs/` 폴더를 저장소 루트에 그대로 업로드합니다.

중요:
- `index.html`은 저장소 루트에 위치
- `docs/` 폴더 구조 유지
- `.nojekyll` 함께 업로드

## 3. GitHub Pages 활성화

저장소에서:

1. `Settings`
2. `Pages`
3. `Build and deployment`
4. Source: `Deploy from a branch`
5. Branch: `main`
6. Folder: `/ (root)`
7. `Save`

설정 후 생성되는 Pages URL에서 포털을 확인합니다.

## 4. 이후 업데이트

예: Landing LP v1.2로 변경할 경우

1. `docs/` 내 새 HTML 추가 또는 기존 파일 교체
2. `index.html`에서 최신 버전/링크 수정
3. `VERSION.md` 업데이트
4. Commit / Push

권장 커밋 예시:

```text
landing: update LP v1.1 to v1.2 release candidate
```

## 5. 보안 주의

GitHub Pages는 정적 호스팅이므로 현재 비밀번호는 클라이언트 측 접근 제한입니다.

민감한 계약정보, 환자정보, 개인정보, 의료정보는 직접 포함하지 않는 것을 권장합니다.

강한 접근제어가 필요하면:
- Cloudflare Access
- 사내 인증 서버
- 비공개 문서 시스템

등을 사용해야 합니다.