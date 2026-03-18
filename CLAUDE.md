# CLAUDE.md

이 파일은 Claude Code(claude.ai/code)가 이 저장소에서 작업할 때 참고하는 안내 문서입니다.

## 프로젝트 개요

유명 명언을 표시하는 단일 페이지 정적 웹 애플리케이션입니다. 빌드 도구, 의존성, 프레임워크 없이 파일 하나로 구성됩니다.

## 구조

모든 코드는 `index.html` 안에 있습니다:
- **데이터**: `quotes` 배열 (18개) — 각 항목은 `text`, `author`, `tag` 필드를 가짐
- **렌더링**: `renderQuotes(selected)` — DOM 카드를 생성하고 순서대로 애니메이션 적용
- **로직**: `getRandomQuotes(n)` — 배열을 섞어 n개 추출; `showRandom()`이 이를 연결
- **스타일**: 인라인 `<style>` 블록 — 다크 테마, 태그별 색상은 JS의 `tagColors` 맵으로 관리

## 실행

`index.html`을 브라우저에서 직접 열면 됩니다. 서버 불필요.
