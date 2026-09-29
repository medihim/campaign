# GitHub Pages 배포 가이드

## 1. 저장소 생성

GitHub에서 새 저장소를 생성합니다.

예시:
- Repository name: `ippeo-campaign-playbook`
- Visibility: 조직 정책에 맞게 선택

## 2. 파일 업로드

본 폴더의 파일을 저장소 루트에 업로드합니다.

필수 파일:
- `index.html`
- `.nojekyll`

권장 파일:
- `README.md`
- `VERSION.md`
- `DEPLOY_GITHUB_PAGES.md`

## 3. GitHub Pages 활성화

GitHub 저장소에서:

1. `Settings`
2. `Pages`
3. `Build and deployment`
4. Source를 `Deploy from a branch`로 선택
5. Branch를 `main`
6. Folder를 `/ (root)`
7. Save

설정 후 GitHub가 Pages URL을 생성합니다.

## 4. 버전 업데이트 방식

이후 캠페인 결과가 추가될 때:

1. `index.html` 수정
2. 문서 내부 버전 번호 변경
3. `VERSION.md` 업데이트
4. Git commit 메시지에 변경 벡터를 명시

예시:
- `v2.5 landing-value-update`
- `v2.6 line-friction-update`
- `v2.7 offer-test-result`

## 5. 보안 주의

현재 비밀번호 보호는 JavaScript 기반의 클라이언트 측 접근 제한입니다.
GitHub Pages는 정적 호스팅이므로 서버측 비밀번호 인증을 제공하지 않습니다.

민감한 경영정보, 개인정보, 의료정보, 계약정보를 포함할 경우에는 다음 중 하나를 권장합니다.

- 사내 인증이 가능한 별도 서버에 배포
- Cloudflare Access 등 접근제어 서비스 사용
- 조직용 비공개 문서 시스템 사용

## 6. 변경 시 주의

- GA4 / GTM / Meta 관련 실제 운영 코드가 추가될 경우 개인정보가 분석 플랫폼으로 전달되지 않도록 점검
- 병원/환자 개인정보를 정적 HTML 안에 직접 기록하지 않기
- 실제 캠페인 결과값을 추가할 때도 개인 식별정보 대신 집계값만 사용