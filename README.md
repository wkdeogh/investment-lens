# Investment Lens

기업 분석 리포트를 모아 보는 정적 사이트입니다.

- 홈: https://wkdeogh.github.io/investment-lens/
- 루멘텀: `reports/lumentum-LITE-2026-10-02.html`
- 암페놀: `reports/amphenol-APH-2026-10-02.html`

## 로컬 확인

저장소에서 `python3 -m http.server 8765`를 실행하고 http://localhost:8765 를 엽니다. 별도 설치나 빌드가 필요하지 않습니다.

## 리포트 추가

1. 완성한 HTML을 `reports/`에 추가합니다.
2. 리포트의 기존 헤더와 목차 바를 제거하고 기존 리포트와 같은 `.site-header` 홈 헤더를 넣습니다. 홈 링크는 `../index.html`을 사용합니다.
3. HTML의 `<head>`에 `<link rel="stylesheet" href="../assets/site.css">`를 넣습니다.
4. `index.html`의 `.report-list`에 해당 리포트 링크를 추가합니다.

공통 헤더 스타일은 `assets/site.css`에서 관리합니다. 리포트 본문과 분석 도구는 각 HTML에 포함되며, 외부 링크의 원문 자료는 원래 출처에서 열립니다.

## 게시

GitHub Pages는 `main` 브랜치의 루트(`/`)를 게시합니다. `main`에 푸시하면 갱신됩니다.
