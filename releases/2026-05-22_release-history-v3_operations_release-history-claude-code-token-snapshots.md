# release-history-v3 - Operations

Date: 2026-05-22
Released at: 2026-05-22 20:12 KST
Component: Operations
Status: deployed

## Summary
Public release notes에서 Claude Code 누적 토큰 사용량도 함께 확인할 수 있도록 자동화를 보강했습니다.

## Changes
- tui-monitor가 사용하던 Claude Code 토큰 집계 결과를 public release notes README에 표시하도록 추가했습니다.
- Claude Code 누적 토큰, 주간/월간 사용량, 일평균, 세션 파일 수, assistant entry 수를 공개-safe 형식으로 보여줍니다.
- 공개 README에는 로컬 경로나 private session 파일명 대신 공개 가능한 집계 범위만 표시하도록 했습니다.

## Known Issues
- Claude Code 토큰 사용량은 실시간 값이 아니라 public release notes 업데이트 시점에 기록되는 정적 스냅샷입니다.
