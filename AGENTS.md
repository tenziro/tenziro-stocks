<!-- BEGIN:nextjs-agent-rules -->

# This is NOT the Next.js you know

This version has breaking changes — APIs, conventions, and file structure may all differ from your training data. Read the relevant guide in `node_modules/next/dist/docs/` before writing any code. Heed deprecation notices.

<!-- END:nextjs-agent-rules -->

# 문구 작성 방법

사이트의 모든 텍스트 문구는 `docs/TEXT_GUIDE.md`를 참고하여 작성한다.

# 개발 이력 기록 (필수)

모든 작업 — 오류 수정, 신규 기능, 기능 개선, 리팩터링 — 을 완료하면 반드시
`docs/DEVELOPMENT_LOG.md`의 "변경 이력" 맨 위에 항목을 추가한다.
형식: `### YYYY-MM-DD — 제목` + 유형 태그(`기능`/`수정`/`개선`/`문서`/`인프라`) + 한두 문장 요약 + 관련 파일.
큰 기능이면 같은 문서의 "기능 현황" 해당 절도 함께 갱신한다.

# 업데이트 로그 작성(필수)

`docs/DEVELOPMENT_LOG.md` 내용을 참고하여 `src/lib/changelog.ts`를 업데이트 한다.
버전 규칙: 신규 기능 = minor(1.1.0), 오류 수정/개선 = patch(1.0.2).
새 배포마다 맨 위에 추가한다 (상세 개발 기록은 docs/DEVELOPMENT_LOG.md).
