# release-history-v1 - Operations

Date: 2026-05-21
Component: Operations
Status: not-deployed

## Summary
POMFS 변경 이력을 구조적으로 기록하고 검증하는 release history 체계를 추가했습니다.

## Changes
- iOS, Web, Backend, Data Pipeline, Infra, Operations 구분을 추가했습니다.
- public note 생성 전에 validation과 sanitizer 검사를 수행하도록 했습니다.
- public-safe release note를 로컬에서 preview할 수 있도록 했습니다.

## Known Issues
- Public GitHub repo는 생성되었지만 자동 publish workflow는 아직 활성화하지 않았습니다.
