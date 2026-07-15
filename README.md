# ai-feed-dashboard

**이 저장소는 생성물(generated artifact)입니다 — 손으로 편집하지 마세요.**

`index.html`, `pm.html` 전부 [`ai-feed`](https://github.com/wsungAhn/ai-feed) 저장소의
`src/ai_feed/dashboard.py` / `scripts/generate_dashboard_html.py`가 생성해서
GitHub Actions(`ai-feed`의 `.github/workflows/deploy-dashboard.yml`)가 이 저장소로
자동 push합니다.

- 실제 로직·테스트: `ai-feed` 저장소 (`tests/unit/test_dashboard.py`,
  `tests/test_dashboard_payload.py`, `tests/unit/test_generate_dashboard_html.py`)
- 여기서 직접 고친 내용은 다음 배포 때 덮어써서 사라집니다.
- 카드 레이아웃/배지/문구를 바꾸려면 `ai-feed` 저장소의 위 스크립트를 수정하세요.

**결정 근거** (2026-07-15): 2026-07-13 통합 감사에서 "독립 앱 vs 정적 생성물" 여부가
미확정 상태였음. 실사용 확인 결과 이 저장소엔 소스/빌드/테스트가 전혀 없고 자동
커밋(`update: dashboard YYYY-MM-DD`)만 반복돼 있어, 독립 앱으로 전환할 실익이
없다고 판단 — 생성물로 공식 확정.
