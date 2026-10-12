---
name: midterm-concept
description: 중간고사 모의시험 1단계 (개념). 팀(네트워크 01 / 02)에 맞춰 30문제를 하나씩 내고, 학생이 답한 뒤에만 채점한다. 문제가 개념을 먼저 설명하고, 그 개념을 이해했는지 서술형으로 묻는다 — 이유를 대고, 새 사례에 적용하고, 비슷한 것과 가르게 한다. 중간 저장되어 여러 세션에 나눠 풀 수 있다.
---

# Codex 학습 스킬: midterm-concept

## 실행 방법

1. 저장소 루트의 `.claude/skills/midterm-concept/SKILL.md`를 읽고 그 학습 절차를 따른다. 이 파일이 공통 절차의 원본이다. Claude 전용 frontmatter(`user-invocable`, `argument-hint`)는 Codex 설정으로 해석하지 않는다.
2. 원본의 `$ARGUMENTS`는 사용자 메시지에서 `$midterm-concept` 뒤에 적은 주제·팀·모드로 해석한다. 자연어 요청이면 요청에서 같은 정보를 추출한다. 인자가 없을 때는 원본의 기본 선택 절차를 따른다.
3. 원본의 `/midterm-concept`는 Codex에서는 `$midterm-concept` 호출을 뜻한다. 다른 학습 스킬의 `/study`, `/midterm-concept`, `/midterm-prompt` 안내도 각각 `$study`, `$midterm-concept`, `$midterm-prompt`로 표시한다.
4. `문제.md`, `문제-{사례}.md`, `채점기준.md`, `채점기준-{사례}.md`는 `.claude/skills/midterm-concept/`에서 찾는다. `내학습/`, `courses/`, `study-progress/` 경로는 저장소 루트 기준이다.
5. 학생에게 한 번에 한 문제를 제시하고 답변을 기다린다. 학생이 답하기 전에는 채점기준을 읽거나 모범 답안을 공개하지 않는다. 대화를 혼자 진행하거나 학생 답을 만들어 기록하지 않는다.
6. 기록은 기존 `내학습/` 파일에 원본 형식으로 남긴다. Claude Code에서 남긴 기록도 읽고 이어서 사용하며, 기존 기록을 초기화하지 않는다.
