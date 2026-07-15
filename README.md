# 캠퍼스 플래너 (Campus Planner)

대학생 시간표 & 하루 관리 웹 — 구치파치 2주차 팀 프로젝트입니다.
`index.html` 파일 하나에 HTML/CSS/JS가 모두 들어 있습니다.

## 실행 방법

별도 설치 없이 `index.html`을 브라우저로 열면 됩니다.

## 팀 구성 & 브랜치

| 담당 | 기능 | 섹션 id | 브랜치 |
|------|------|---------|--------|
| 팀원 1 | 오늘의 시간표 (+ 공통 UI 베이스, 레포·머지 담당) | `timetable` | `feature/timetable` |
| 팀원 2 | 하루 플래너 | `planner` | `feature/planner` |
| 팀원 3 | D-Day 계산기 | `dday` | `feature/dday` |
| 팀원 4 | 집중 타이머 | `timer` | `feature/timer` |

## 팀 규칙

1. 자기가 맡은 섹션(`<section id="...">`) **내부만** 수정하기
2. 브랜치 이름은 위 표와 정확히 맞추기
3. PR 올리면 팀 채팅방에 알리기

## 공통 디자인 시스템

`index.html`의 `<style>` 맨 위 주석에 팀원 가이드가 있습니다. 요약:

- 색상은 `:root`의 CSS 변수만 사용 (`var(--ink)`, `var(--sub)` 등)
- 내 섹션 포인트 색: `var(--accent)` / 연한 배경: `var(--accent-soft)` (카드에 이미 지정됨)
- 공통 컴포넌트: `.btn`, `.btn-primary`, `.input`, `.chip`, `.hl`(형광펜 하이라이트)
- 숫자 표시는 `font-family: var(--font-num)` 권장
- 개발 시작 시 내 섹션의 `.placeholder` div를 지우고 그 자리에 기능 구현
