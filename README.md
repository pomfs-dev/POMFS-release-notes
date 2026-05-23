# POMFS Release History

이 저장소는 POMFS의 공개 릴리즈 히스토리입니다.

각 항목은 private source repo의 release metadata에서 생성되며, 공개 가능한 요약만 포함합니다. iOS, Web, Backend, Data Pipeline, Infra, Operations 변경을 시간순으로 모아 보여줍니다.

공개 노트에는 source code, 내부 경로, 개인 이메일, private infrastructure detail, token/key, raw commit hash, sensitive security detail을 포함하지 않습니다.

상세 항목에는 Summary, Changes, Known Issues가 있으며, 시간이 확인된 항목은 `Released at`을 함께 표시합니다.

## AI Lifetime Token Usage

Codex와 Claude Code의 전체 누적 토큰량을 함께 보여줍니다. 각 값은 public release notes가 갱신될 때 기록되는 정적 스냅샷입니다.

### Codex

Codex 전체 누적 토큰량입니다. 이 값은 실시간 대시보드가 아니라 public release notes가 갱신될 때 함께 기록되는 정적 스냅샷입니다.

<table>
  <tr>
    <th align="left">Snapshot</th>
    <td>2026-05-24 02:27 KST</td>
  </tr>
  <tr>
    <th align="left">Scope</th>
    <td>Codex session logs</td>
  </tr>
  <tr>
    <th align="left">Sessions</th>
    <td>131 sessions</td>
  </tr>
  <tr>
    <th align="left">Cumulative total</th>
    <td><strong>818,008,322 tokens</strong></td>
  </tr>
  <tr>
    <th align="left">Input</th>
    <td>815,375,748 tokens</td>
  </tr>
  <tr>
    <th align="left">Cached input</th>
    <td>768,710,656 tokens</td>
  </tr>
  <tr>
    <th align="left">Output</th>
    <td>2,632,574 tokens</td>
  </tr>
  <tr>
    <th align="left">Reasoning output</th>
    <td>935,847 tokens</td>
  </tr>
</table>

<table>
  <tr>
    <th align="left">Scale</th>
    <th align="left">Usage Graph</th>
    <th align="right">Percent</th>
  </tr>
  <tr>
    <td>850,000,000 tokens</td>
    <td><code>███████████████████░</code></td>
    <td align="right">96.2%</td>
  </tr>
</table>

### Claude Code

Claude Code 전체 누적 토큰량입니다. 이 값은 tui-monitor 집계기가 Claude Code session logs를 다시 계산해 기록한 정적 스냅샷입니다.

<table>
  <tr>
    <th align="left">Snapshot</th>
    <td>2026-05-24 02:27 KST</td>
  </tr>
  <tr>
    <th align="left">Scope</th>
    <td>Claude Code session logs</td>
  </tr>
  <tr>
    <th align="left">Session files</th>
    <td>1,171 files</td>
  </tr>
  <tr>
    <th align="left">Assistant entries</th>
    <td>96,351 entries</td>
  </tr>
  <tr>
    <th align="left">Cumulative total</th>
    <td><strong>22,797,855,060 tokens</strong></td>
  </tr>
  <tr>
    <th align="left">Input</th>
    <td>1,213,842 tokens</td>
  </tr>
  <tr>
    <th align="left">Cache creation</th>
    <td>985,713,413 tokens</td>
  </tr>
  <tr>
    <th align="left">Cache read</th>
    <td>21,663,922,383 tokens</td>
  </tr>
  <tr>
    <th align="left">Output</th>
    <td>147,005,422 tokens</td>
  </tr>
  <tr>
    <th align="left">Weekly 7d</th>
    <td>5,402,912,356 tokens</td>
  </tr>
  <tr>
    <th align="left">Monthly 30d</th>
    <td>22,322,391,973 tokens</td>
  </tr>
  <tr>
    <th align="left">Daily avg</th>
    <td>670,525,148 tokens/day</td>
  </tr>
</table>

<table>
  <tr>
    <th align="left">Scale</th>
    <th align="left">Usage Graph</th>
    <th align="right">Percent</th>
  </tr>
  <tr>
    <td>22,800,000,000 tokens</td>
    <td><code>████████████████████</code></td>
    <td align="right">100.0%</td>
  </tr>
</table>

## Latest

| Date | Version | Component | Summary |
|---|---|---|---|
| 2026-05-23 | [r1.50.7](releases/2026-05-23_r1.50.7_backend_settlement-payout-reconciliation.md) | Backend | 정산 화면과 관리자 정산 흐름에서 PayPal 지급과 결제 대사 흐름을 더 정확하게 확인할 수 있도록 보강했습니다. |
| 2026-05-23 | [r1.50.7](releases/2026-05-23_r1.50.7_backend_my-settlement-aggregation.md) | Backend | 정산 화면이 최신 공연 티켓 주문 구조까지 반영해서 판매 금액을 집계하도록 보강했습니다. |
| 2026-05-22 | [r1.50.6](releases/2026-05-22_r1.50.6_backend_paypal-refund-cascade.md) | Backend | PayPal로 결제한 티켓도 환불 완료 후 안내 메일, 공연 생성자 알림, 환불 상태 표시가 Toss 결제와 같은 흐름으로 처리되도록 보강했습니다. |
| 2026-05-22 | [r1.50.5](releases/2026-05-22_r1.50.5_backend_ticket-refund-notifications-management.md) | Backend | 티켓 환불 완료 후 안내 메일과 공연 관리 화면의 환불 상태 표시가 더 정확해지도록 보강했습니다. |
| 2026-05-22 | [r1.50.5](releases/2026-05-22_r1.50.5_backend_ticket-refund-host-notifications.md) | Backend | 티켓 환불이 완료되면 공연 생성자가 알림에서 관련 티켓 관리 화면으로 이동할 수 있도록 알림 흐름을 보강했습니다. |
| 2026-05-22 | [r1.50.5](releases/2026-05-22_r1.50.5_ios_ios-ticket-deeplink-scheme.md) | iOS | iOS 앱에서 티켓 메일의 앱 열기 버튼이 티켓 화면으로 이어질 수 있도록 딥링크 처리를 보강했습니다. |
| 2026-05-22 | [release-history-v3](releases/2026-05-22_release-history-v3_operations_release-history-claude-code-token-snapshots.md) | Operations | Public release notes에서 Claude Code 누적 토큰 사용량도 함께 확인할 수 있도록 자동화를 보강했습니다. |
| 2026-05-22 | [r1.50.4](releases/2026-05-22_r1.50.4_backend_ticket-email-detail-scanner-recovery.md) | Backend | 결제 완료와 티켓 발급 메일, 나의 티켓 상세 보기, QR 확인, 티켓 스캐너 흐름을 실제 발급 티켓 기준으로 보강했습니다. |
| 2026-05-22 | [release-history-v2](releases/2026-05-22_release-history-v2_operations_release-history-codex-token-snapshots.md) | Operations | Public release notes와 iOS README가 같은 Codex 누적 토큰 스냅샷을 표시하도록 release history 자동화를 보강했습니다. |
| 2026-05-22 | [r1.50.3](releases/2026-05-22_r1.50.3_web_scoped-location-routes.md) | Web | Today와 Shows에서 필요한 위치 기능을 다시 사용할 수 있도록 하면서 결제 화면에서는 위치 사용을 막았습니다. |
| 2026-05-22 | [r1.50.3](releases/2026-05-22_r1.50.3_ios_ios-scoped-location-webview.md) | iOS | iOS 앱에서 위치 기능이 필요한 화면에서만 동작하도록 허용 범위를 조정했습니다. |
| 2026-05-22 | [r1.50.2](releases/2026-05-22_r1.50.2_backend_ticket-visibility-recovery.md) | Backend | 실제 승인된 티켓 결제가 나의 티켓에 표시되도록 결제 확정과 티켓 조회 흐름을 보강했습니다. |
| 2026-05-22 | [r1.50.4](releases/2026-05-22_r1.50.4_ios_ios-codex-token-usage-snapshot.md) | iOS | iOS 앱 README에서 Codex 누적 토큰 사용량을 확인할 수 있도록 공개 스냅샷을 추가했습니다. |
| 2026-05-22 | [r1.50.1](releases/2026-05-22_r1.50.1_backend_payment-completion.md) | Backend | 티켓 결제가 실제 승인 후 구매 완료와 티켓 발급으로 이어지도록 결제 완료 흐름을 개선했습니다. |
| 2026-05-22 | [r1.50.1](releases/2026-05-22_r1.50.1_ios_ios-payment-webview.md) | iOS | iOS 앱에서 결제 앱으로 이동하고 다시 돌아오는 흐름을 개선했습니다. |
| 2026-05-21 | [r1.49.13](releases/2026-05-21_r1.49.13_web_event-social-links-managed-cards.md) | Web | 공연 수정 후 상세 정보, 티켓 금액, 유튜브·인스타그램 링크 표시가 더 일관되게 반영되도록 개선했습니다. |
| 2026-05-21 | [r1.49.12](releases/2026-05-21_r1.49.12_web_managed-event-edit-navigation.md) | Web | 공연 수정 후 관리 목록의 가격 표시와 뒤로가기 흐름을 개선했습니다. |
| 2026-05-21 | [r1.49.11](releases/2026-05-21_r1.49.11_web_likes-auth-persistence-web.md) | Web | 앱 재실행 후에도 좋아요한 공연이 Likes 화면과 공연 상세에서 유지되도록 개선했습니다. |
| 2026-05-21 | [r1.49.11](releases/2026-05-21_r1.49.11_backend_likes-auth-persistence-api.md) | Backend | 공연 좋아요 상태를 더 정확히 조회하도록 서버 응답을 보강했습니다. |
| 2026-05-21 | [r1.49.10](releases/2026-05-21_r1.49.10_web_event-detail-flow.md) | Web | 공연 상세, 좋아요, 티켓/게스트리스트, 공유 흐름의 안정성을 개선했습니다. |
| 2026-05-21 | [r1.49.10](releases/2026-05-21_r1.49.10_web_apple-login-routing-fallback-fix.md) | Web | 운영 커뮤니티 웹에서 Apple 로그인 버튼이 잘못된 로그인 경로로 이동하던 문제를 수정했습니다. |
| 2026-05-21 | [r1.49.10](releases/2026-05-21_r1.49.10_backend_event-owner-api-guard.md) | Backend | 공연을 만든 계정이 자신의 공연에 티켓 구매나 게스트리스트 신청을 하지 않도록 서버 검증을 추가했습니다. |
| 2026-05-21 | [release-history-v1](releases/2026-05-21_release-history-v1_operations_release-history-scaffold.md) | Operations | POMFS 변경 이력을 구조적으로 기록하고 검증하는 release history 체계를 추가했습니다. |
| 2026-05-19 | [R1.49.2](releases/2026-05-19_R1.49.2_ios_devlog-002-b25a861e.md) | iOS | iOS 앱 변경 이력: R1.49.2 simpler approach fail PROVEN + session handoff base — R1.49.2 ASWebAuthenticationSession 측 다음 세션 base sustained 진행 base |
| 2026-05-17 | [R1.41](releases/2026-05-17_R1.41_web_devlog-008-bafb15e5.md) | Web | 웹/프론트엔드 변경 이력: R1.41 cluster Phase B 완료 base + Phase C-E close LIVE — community.prideofmisfits.com cutover Path X (nginx reverse proxy) + 풀스택 8 워커 병렬 + Wave 1 6/6 + Wave 2 2/2 + cascade 4건 + Codex audit 2건 ALL [FINAL] LIVE + 사용자 visible 사고 0건 sustained LIVE 첫 record + R1.42+ scope cumulative 8건 보존 |
| 2026-05-17 | [r1.43](releases/2026-05-17_r1.43_operations_session-handoff-automation.md) | Operations | 내부 릴리스 및 세션 handoff 자동화를 개선했습니다. |
| 2026-05-17 | [R1.40](releases/2026-05-17_R1.40_web_devlog-009-40a817c3.md) | Web | 웹/프론트엔드 변경 이력: R1.40 cluster final close GRAND TOTAL 37/37 = 100% COMPLETED LIVE 첫 record + 영구 룰 #140 정식 승격 + production endpoint design.prideofmisfits.com HTTP 200 LIVE |
| 2026-05-16 | [R1.38.x](releases/2026-05-16_R1.38.x_backend_devlog-018-e96d4b4c.md) | Backend | 백엔드/API 변경 이력: R1.38.x cluster cascade LIVE 영구 종료 final (R1.37.0.1.X 5개월 cascade 진짜 root cause 100% 해소 ) |
| 2026-05-16 | [R1.38.0](releases/2026-05-16_R1.38.0_backend_devlog-019-883ea31e.md) | Backend | 백엔드/API 변경 이력: R1.38.0 cluster LIVE (spec-kit 정상 도입 + dispatch_observer daemon + voice cascade screencapture + LRN-NEW-114 진짜 root cause + LRN-NEW-115 chicken-and-egg #133 후보) |
| 2026-05-16 | [R1.33](releases/2026-05-16_R1.33_web_devlog-020-9b07dcf7.md) | Web | 웹/프론트엔드 변경 이력: R1.33 + R1.34 cluster LIVE + AWS Key 영구 마스킹 (외부 모니터 자동 감지 + voice-close /exit 강화 + Codex P1 + 자율 발견 1건 cascade) |
| 2026-05-16 | [R1.38.x](releases/2026-05-16_R1.38.x_backend_devlog-010-d8e232c2.md) | Backend | 백엔드/API 변경 이력: R1.38.x Phase 9 cascade chain hard termination 첫 적용 LIVE 첫 record (iter 7 MAJOR META-META IRONY + #134 Rule F 15회차 +200% surplus triple sustained record + 세션 종료 base) |
| 2026-05-16 | [R1.38.x](releases/2026-05-16_R1.38.x_data-pipeline_devlog-011-fb51290a.md) | Data Pipeline | 데이터 파이프라인 변경 이력: R1.38.x Phase 8 #136 Option A rollback (MAJOR IRONY = #136 SOP 자체 측 cascade chain 재개 LIVE 첫 입증, meta-level cascade recursion) |
| 2026-05-16 | [R1.38.x](releases/2026-05-16_R1.38.x_backend_devlog-012-1c384d19.md) | Backend | 백엔드/API 변경 이력: R1.38.x cluster cascade close + #136 정식 승격 (audit cascade chained finding pattern + cascade chain termination LIVE 첫 입증 record) |
| 2026-05-16 | [R1.38.3.4](releases/2026-05-16_R1.38.3.4_backend_devlog-013-2a18424f.md) | Backend | 백엔드/API 변경 이력: R1.38.3.4 hotfix #135 L100 명시적 pane target + LRN-NEW-121 6 step matrix (cascade chain termination 첫 적용 LIVE 첫 record + #134 Rule F dogfooding 8회차 +60% surplus) |
| 2026-05-16 | [R1.38.3.3](releases/2026-05-16_R1.38.3.3_backend_devlog-014-201379a8.md) | Backend | 백엔드/API 변경 이력: R1.38.3.3 hotfix #135 L100 Option C + LRN-NEW-121 정식 등재 (audit cascade chained finding pattern + trade-off recursive cascade 영구 회피 SOP base + #134 Rule F dogfooding 6회차 sustained record 갱신 LIVE + #136 후보 base) |
| 2026-05-16 | [R1.38.3.2](releases/2026-05-16_R1.38.3.2_backend_devlog-015-684917f8.md) | Backend | 백엔드/API 변경 이력: R1.38.3.2 hotfix #135 L100 Option A + L123 SUMMARY 정정 (Codex P2 finding 2건 + #134 Rule F dogfooding 5회차 첫 도달 LIVE) |
| 2026-05-16 | [R1.38.3.1](releases/2026-05-16_R1.38.3.1_backend_devlog-016-95090466.md) | Backend | 백엔드/API 변경 이력: R1.38.3.1 hotfix #135 effective scope 11 한정 정정 (Codex P2 finding) |
| 2026-05-16 | [R1.38.3](releases/2026-05-16_R1.38.3_web_devlog-017-14362873.md) | Web | 웹/프론트엔드 변경 이력: R1.38.3 cluster Phase 4 LIVE 종료 + #134/#135 영구 룰 2건 정식 승격 + LRN-NEW-118/119/120 cluster cascade |
| 2026-05-15 | [history-20260515-021](releases/2026-05-15_history-20260515-021_web_devlog-021-bda49d36.md) | Web | 웹/프론트엔드 변경 이력: AWS Postiz 인프라 셋업 (운영 환경 NAS 호스팅용 S3 + Route53) |
| 2026-05-15 | [R1.32.x.VOICE-1.9](releases/2026-05-15_R1.32.x.VOICE-1.9_web_devlog-022-426d7c30.md) | Web | 웹/프론트엔드 변경 이력: R1.32.x.VOICE-1.9 LIVE 영구 종료 (AF-VS-3 fix + voice-feedback.sh helper 2 함수 +4 LOC + Phase C mock TS-1 +43% over matrix) |
| 2026-05-15 | [R1.32.x.VOICE-1](releases/2026-05-15_R1.32.x.VOICE-1_web_devlog-023-b522c95e.md) | Web | 웹/프론트엔드 변경 이력: R1.32.x.VOICE-1 LIVE 영구 종료 (voice-shutdown.sh hierarchical event-driven cascade SOP refactor + Phase B' 3 fix + LRN-NEW-101~104) |
| 2026-05-14 | [R1.28.x.HOTFIx](releases/2026-05-14_R1.28.x.HOTFIx_web_devlog-024-8d5935c7.md) | Web | 웹/프론트엔드 변경 이력: R1.28.x.HOTFIX LIVE 영구 종료 final + ECS deploy 진정 완료 + Bug #2 fix LIVE 적용 확정 |
| 2026-05-14 | [R1.28.x](releases/2026-05-14_R1.28.x_web_devlog-025-8229bf9d.md) | Web | 웹/프론트엔드 변경 이력: R1.28.x sub-sprint LIVE 영구 종료 final + 웹 앱 /api/logout Google IdP revocation LIVE 적용 (R1.28.4 사용자 명시 GO 정합) |
| 2026-05-14 | [R1.28](releases/2026-05-14_R1.28_web_devlog-026-72c31f18.md) | Web | 웹/프론트엔드 변경 이력: R1.28 sub-sprint LIVE 영구 종료 final + 디자인 사이트 로그아웃 버그 fix LIVE deployed |
| 2026-05-12 | [R1.19.13](releases/2026-05-12_R1.19.13_web_devlog-027-8ff53d0f.md) | Web | 웹/프론트엔드 변경 이력: R1.19.13 iTerm Status Bar broadcaster Phase 1~5 LIVE 종료 + 3건 사고 영구 제거 + LRN-NEW-55 등재 |
| 2026-05-12 | [R1.19.5](releases/2026-05-12_R1.19.5_operations_devlog-032-f0b121f9.md) | Operations | 운영 자동화 변경 이력: R1.19.5 fast-follow: handoff-respawn-commander.sh set -u P2 fix + 신규 추적 + audit 100% PASS + #91 LIVE 8번째 누적 |
| 2026-05-12 | [R1.19.10](releases/2026-05-12_R1.19.10_backend_devlog-028-f546e466.md) | Backend | 백엔드/API 변경 이력: R1.19.10 Security Hotfix LIVE PASS (#NEW-α IPv6 keyGenerator + #NEW-β Toss log masking) + LRN-NEW-51 SOP 2회차 정합 입증 |
| 2026-05-12 | [R1.19.6](releases/2026-05-12_R1.19.6_web_devlog-029-52b1b6d8.md) | Web | 웹/프론트엔드 변경 이력: R1.19.6 진정 ECS LIVE PASS (5/12 03:13 false claim 정정) + task def digest pin 영구 회피 + LRN-NEW-51 등재 |
| 2026-05-12 | [R1.19.6](releases/2026-05-12_R1.19.6_web_devlog-030-4cdc8643.md) | Web | 웹/프론트엔드 변경 이력: R1.19.6 ECS LIVE PASS + R1.19.8 hotfix #3 loading state per-card 분리 PASS + LRN-NEW-50 등재 |
| 2026-05-12 | [R1.19.6](releases/2026-05-12_R1.19.6_web_devlog-031-4a9cfa65.md) | Web | 웹/프론트엔드 변경 이력: R1.19.6 FF-A: 백엔드 서버 adminTickets jsonb fallback precedence commit+push + LRN-NEW-48/49 등재 (A+B-2 일괄) |
| 2026-05-11 | [R1.19.5](releases/2026-05-11_R1.19.5_backend_devlog-034-4e2a6e64.md) | Backend | 백엔드/API 변경 이력: R1.19.5 Phase 2 sprint 영구 종료 + #90 9 Rule LIVE 입증 + 권커맨더 자율 commit + HOF-023 발행 |
| 2026-05-11 | [R1.19.5](releases/2026-05-11_R1.19.5_web_devlog-035-9712b550.md) | Web | 웹/프론트엔드 변경 이력: R1.19.5 Phase 1 박수 폐기 결정 + 권커맨더 단독 핸드오프 + Phase 2 prep (HOF-022 발행) |
| 2026-05-11 | [R1.19.5](releases/2026-05-11_R1.19.5_web_devlog-036-11e6ab5e.md) | Web | 웹/프론트엔드 변경 이력: R1.19.5 Phase 1 박수 detect LIVE + 컴퓨터 재시작 핸드오프 (HOF-021 발행) |
| 2026-05-11 | [R1.19.4](releases/2026-05-11_R1.19.4_web_devlog-037-70a681f4.md) | Web | 웹/프론트엔드 변경 이력: R1.19.4 sprint 풀스택 100% LIVE + R1.19.5 자동화 음성 trigger 100% PASS + 사용자 명시 fresh spawn 의뢰 (HOF-020 발행) |
| 2026-05-11 | [R1.19.x](releases/2026-05-11_R1.19.x_backend_devlog-038-f9cfc6fd.md) | Backend | 백엔드/API 변경 이력: R1.19.x sprint 통합 종료 + 자율 자동화 100% 영구 입증 + R1.18 fast-follow #NEW-1 진정 종료 (HOF-018 발행) |
| 2026-05-11 | [R1.19.5](releases/2026-05-11_R1.19.5_web_devlog-033-0f42f8c5.md) | Web | 웹/프론트엔드 변경 이력: R1.19.5 Phase 3 v3 sprint 영구 종료 + 페어 명령 2단계 분리 사용자 verbatim 시연 LIVE 100% 입증 + #91 LRN-NEW-35 LIVE 7번째 + LRN-NEW-36/37 등재 |
| 2026-05-10 | [R1.18](releases/2026-05-10_R1.18_web_devlog-039-7db09b85.md) | Web | 웹/프론트엔드 변경 이력: R1.18 sprint 영구 종료 + HOF-017 발행 + 영구 메모리 4건 등재 (#78~#81, 자율 자동화 75% LIVE 입증) |
| 2026-05-10 | [R1.15](releases/2026-05-10_R1.15_web_devlog-040-c2c413d1.md) | Web | 웹/프론트엔드 변경 이력: R1.15 sprint 영구 종료 + HOF-016 발행 + R1.18 이메일 발송 (#77 절차 첫 입증, A+B 동시 진행) |
| 2026-05-10 | [R1.14](releases/2026-05-10_R1.14_web_devlog-041-9af86315.md) | Web | 웹/프론트엔드 변경 이력: HOF-014 발행 (R1.14 Phase 1 + R1.12.14 사이클, 사용자 명시 의뢰) |
| 2026-05-10 | [R1.12.14](releases/2026-05-10_R1.12.14_web_devlog-042-86703d8c.md) | Web | 웹/프론트엔드 변경 이력: R1.12.14 sprint 종료 (confirm flow db.transaction wrap + 자동 환불 mutation, 권커맨더 단독) |
| 2026-05-10 | [R1.14](releases/2026-05-10_R1.14_ios_devlog-043-e939dfa2.md) | iOS | iOS 앱 변경 이력: R1.14 sprint Phase 1 종료 (SECURITY ECS task def env Parameter Store 이전 + 자동 회전 5건 + RDS password 회전, 권커맨더 단독) |
| 2026-05-10 | [R1.13.2](releases/2026-05-10_R1.13.2_web_devlog-044-f5ee36a8.md) | Web | 웹/프론트엔드 변경 이력: HOF-013 발행 (R1.13.2 + R1.13.3 + R1.13.4 사이클, 사용자 명시 의뢰) |
| 2026-05-10 | [R1.13.4](releases/2026-05-10_R1.13.4_ios_devlog-045-53b576bc.md) | iOS | iOS 앱 변경 이력: R1.13.4 sprint 종료 (AuthCallbackPage navigate() → window.location.replace, 모바일 OAuth cookie 동기화, 권커맨더 단독) |
| 2026-05-10 | [R1.13.3](releases/2026-05-10_R1.13.3_ios_devlog-046-e27d6565.md) | iOS | iOS 앱 변경 이력: R1.13.3 sprint 종료 (cookie SameSite=Lax → None, 모바일 OAuth flow 안정화, 권커맨더 단독) |
| 2026-05-09 | [R1.13.2](releases/2026-05-09_R1.13.2_web_devlog-047-eaa1ee8d.md) | Web | 웹/프론트엔드 변경 이력: R1.13.2 sprint 종료 (ShowsPage 전 세계 마커 회귀 영구 제거, pg-pool + statement_timeout 강화, 권커맨더 단독) |
| 2026-05-09 | [R1.12.12.1](releases/2026-05-09_R1.12.12.1_web_devlog-048-6a3d72cb.md) | Web | 웹/프론트엔드 변경 이력: HOF-012 발행 (R1.12.12.1 cleanup 사이클 + 이메일/SMS 샘플 검증, 사용자 명시 의뢰) |
| 2026-05-09 | [R1.12.13](releases/2026-05-09_R1.12.13_backend_devlog-049-6b48f25f.md) | Backend | 백엔드/API 변경 이력: R1.12.13 sprint 종료 (cleanup endpoint 완전 제거, security 우선) |
| 2026-05-09 | [R1.12.x](releases/2026-05-09_R1.12.x_ios_devlog-050-7eda34ea.md) | iOS | iOS 앱 변경 이력: cleanup endpoint 호출 SUCCESS (R1.12.x incident 데이터 정리 완료) |
| 2026-05-09 | [R1.12.12.1](releases/2026-05-09_R1.12.12.1_ios_devlog-051-52593157.md) | iOS | iOS 앱 변경 이력: R1.12.12.1 임시 hotfix backend (cleanup endpoint auth bypass + X-Cleanup-Secret) |
| 2026-05-09 | [R1.12.11](releases/2026-05-09_R1.12.11_operations_devlog-052-ba3969a2.md) | Operations | 운영 자동화 변경 이력: R1.12.11 + R1.12.12 + R1.13.1 사이클 핸드오프 발행 (HOF-011, 사용자 명시 의뢰) |
| 2026-05-09 | [R1.13.1](releases/2026-05-09_R1.13.1_web_devlog-053-89c1480d.md) | Web | 웹/프론트엔드 변경 이력: R1.13.1 sprint 종료 (ShowsPage list view 카드 onClick 누락 영구 제거, 권커맨더 단독) |
| 2026-05-08 | [R1.12.11](releases/2026-05-08_R1.12.11_web_devlog-054-ca404afc.md) | Web | 웹/프론트엔드 변경 이력: R1.12.11 sprint 종료 (confirm flow entry_token NOT NULL 위반 영구 제거, 권커맨더 단독) |
| 2026-05-08 | [R1.12.9](releases/2026-05-08_R1.12.9_operations_devlog-055-e14049ed.md) | Operations | 운영 자동화 변경 이력: R1.12.9 + R1.12.10 사이클 핸드오프 발행 (HOF-010, 사용자 명시 의뢰) |
| 2026-05-08 | [R1.12.10](releases/2026-05-08_R1.12.10_web_devlog-056-ea176952.md) | Web | 웹/프론트엔드 변경 이력: R1.12.10 sprint 종료 (jsonb 분기 sold_count UPDATE + frontend remaining 차감, 권커맨더 단독) |
| 2026-05-08 | [R1.12.9](releases/2026-05-08_R1.12.9_web_devlog-057-ada1c59e.md) | Web | 웹/프론트엔드 변경 이력: R1.12.9 sprint 종료 (Toss confirm jsonb 분기 통합, 권커맨더 단독) |
| 2026-05-08 | [R1.13](releases/2026-05-08_R1.13_web_devlog-058-85a0d313.md) | Web | 웹/프론트엔드 변경 이력: R1.13 sprint 결제+티켓 영역 mock 100% 제거 (7 페이지 backend wire, 권커맨더 단독) |
| 2026-05-08 | [R1.12](releases/2026-05-08_R1.12_web_devlog-059-6874e3b7.md) | Web | 웹/프론트엔드 변경 이력: R1.12 sprint #C event source-of-truth (R1.10/R1.11 잔존 회귀 hotfix, 권커맨더 단독) |
| 2026-05-08 | [R1.6](releases/2026-05-08_R1.6_backend_devlog-060-356cf36b.md) | Backend | 백엔드/API 변경 이력: R1.6~R1.11 8 sprint 누적 핸드오프 발행 (HOF-008, 사용자 명시 의뢰) |
| 2026-05-08 | [R1.11](releases/2026-05-08_R1.11_web_devlog-061-dd52865e.md) | Web | 웹/프론트엔드 변경 이력: R1.11 sprint 종료 (#B' 영구 fix backend 모든 분기 검증 통일) |
| 2026-05-08 | [R1.10](releases/2026-05-08_R1.10_web_devlog-062-d550606b.md) | Web | 웹/프론트엔드 변경 이력: R1.10 sprint 종료 (snap=[1] revert + #B' eventType 분기 영구 fix) |
| 2026-05-08 | [R1.9](releases/2026-05-08_R1.9_web_devlog-063-be480d8a.md) | Web | 웹/프론트엔드 변경 이력: R1.9 sprint 종료 (R1.8 PWA 회귀 P0 hotfix #3 + 사용자 명시 의지 정합) |
| 2026-05-08 | [R1.8](releases/2026-05-08_R1.8_web_devlog-064-752456aa.md) | Web | 웹/프론트엔드 변경 이력: R1.8 sprint 종료 (R1.7 PWA 회귀 P0 hotfix #2) |
| 2026-05-08 | [R1.7](releases/2026-05-08_R1.7_web_devlog-065-1cd252c8.md) | Web | 웹/프론트엔드 변경 이력: R1.7 sprint 종료 (R1.6 PWA 회귀 P0 hotfix) |
| 2026-05-08 | [R1.6](releases/2026-05-08_R1.6_web_devlog-066-e7c20ef5.md) | Web | 웹/프론트엔드 변경 이력: R1.6 sprint TicketPurchase architecture refactor 종료 |
| 2026-05-08 | [R1.5.x](releases/2026-05-08_R1.5.x_web_devlog-067-37599964.md) | Web | 웹/프론트엔드 변경 이력: R1.5.x 4 sprint 누적 후 권커맨더 + 5워커 fresh spawn 인계 (R1.5.3 진행 중 + HOF-2026-05-08-001 발행) |
| 2026-05-07 | [R1.5.1](releases/2026-05-07_R1.5.1_web_devlog-068-d82f1793.md) | Web | 웹/프론트엔드 변경 이력: R1.5.1 + R1.5.2 hotfix 통합 종료 (사용자 PWA 시연 발견 사고 2 라운드, footer prop 분리 + BottomSheet minHeight + 숫자 입력 0 prefix) |
| 2026-05-07 | [R1.5](releases/2026-05-07_R1.5_web_devlog-069-52a18603.md) | Web | 웹/프론트엔드 변경 이력: R1.5 sprint 종료 27 BottomSheet 시스템적 근본 fix 옵션 E 완료 (5워커 풀 정합 ~68min, ai-engineer §11 ETA 150-180min 대비 -55~-62% 단축) |
| 2026-05-07 | [R1.4.11](releases/2026-05-07_R1.4.11_ios_devlog-070-0e42e348.md) | iOS | iOS 앱 변경 이력: R1.4.11 #V refine4 권커맨더 단독 hotfix 종료 (TicketPurchase Drawer Content bottom 자체 들어올림, R1.4.x 12 사이클 누적) |
| 2026-05-07 | [R1.3](releases/2026-05-07_R1.3_web_devlog-072-7cee802b.md) | Web | 웹/프론트엔드 변경 이력: R1.3 More + Settlement + 결제 풀구현 + R0a frontend 4건 + Fast-follow #6 통합 종료 (출시 차단 5건 → 0건 100% 달성, mock 100% 제거, 누적 R0a~R1.3 출시 차단 28건 → 0건) |
| 2026-05-07 | [R2.7](releases/2026-05-07_R2.7_web_devlog-073-6b96a426.md) | Web | 웹/프론트엔드 변경 이력: R2.7 admin 데이터 안 보임 회귀 4건 + 신규 사고 #5 visibility mismatch 통합 hotfix 종료 (출시 차단 5건 → 0건 100% 달성, 누적 R0a~R2.7 출시 차단 23건 → 0건) |
| 2026-05-07 | [R2.5](releases/2026-05-07_R2.5_web_devlog-074-1eb80900.md) | Web | 웹/프론트엔드 변경 이력: R2.5 + R2.6 사이클 권커맨더 단독 인계 종료 (5 워커 stuck/missed 사고 학습 + admin 5 사고 fix + bundle -26% minify) |
| 2026-05-07 | [R1.3](releases/2026-05-07_R1.3_web_devlog-071-b7fb7cdb.md) | Web | 웹/프론트엔드 변경 이력: R1.3 PWA 시연 + 실 결제 테스트 시나리오 상세 가이드 발행 (HOF-005, 권커맨더 재진입 후 인수인계 자료) |
| 2026-05-06 | [R2](releases/2026-05-06_R2_web_devlog-075-479e916b.md) | Web | 웹/프론트엔드 변경 이력: R2 회귀 sweep + Fast-follow 통합 hotfix 종료 + R0a~R2 누적 통합 (출시 차단 14건 → 0건 100% 달성, 거버넌스 §F 19/19 정합, 사고 1건 즉시 회피) |
| 2026-05-06 | [R1.2.d](releases/2026-05-06_R1.2.d_web_devlog-076-fc4536b6.md) | Web | 웹/프론트엔드 변경 이력: R1.2.d admin sub-라운드 4 풀스택 종료 + R1.2 4 sub 통합 종료 (22 항목 admin 풀스택 wire 완전 종료, 출시 차단 신규 0, 마스터 플랜 in-target, 사고 0건 첫 라운드) |
| 2026-05-06 | [R1.2.c](releases/2026-05-06_R1.2.c_web_devlog-077-97514a29.md) | Web | 웹/프론트엔드 변경 이력: R1.2.c admin sub-라운드 3 풀스택 종료 (출시 차단 신규 0, 마스터 플랜 in-target, team-lead fresh spawn 의무) |
| 2026-05-06 | [R1.2.b](releases/2026-05-06_R1.2.b_web_devlog-078-79fa072b.md) | Web | 웹/프론트엔드 변경 이력: R1.2.b admin sub-라운드 2 풀스택 종료 (출시 차단 신규 0, 마스터 플랜 -50%) |
| 2026-05-06 | [R1.2.a](releases/2026-05-06_R1.2.a_web_devlog-284-0c6c6bce.md) | Web | 웹/프론트엔드 변경 이력: R1.2.a admin sub-라운드 1 풀스택 종료 + 권커맨더+team-lead 동시 fresh spawn 시점 |
| 2026-05-06 | [R1.2.a](releases/2026-05-06_R1.2.a_web_devlog-079-d8d89321.md) | Web | 웹/프론트엔드 변경 이력: R1.2.a admin sub-라운드 1 풀스택 종료 (Services hotfix 포함, 거버넌스 §F 7/7 정합) |
| 2026-05-06 | [R1.1](releases/2026-05-06_R1.1_web_devlog-080-86947c8f.md) | Web | 웹/프론트엔드 변경 이력: R1.1 DB 정합성 풀스택 종료 (Phase A→B→E ALL PASS, G1 게이트 진입) |
| 2026-05-06 | [history-20260506-081](releases/2026-05-06_history-20260506-081_web_devlog-081-a3685a09.md) | Web | 웹/프론트엔드 변경 이력: R0a 인프라 전수 audit 종료 (출시 차단 14건 발견) |
| 2026-05-06 | [history-20260506-082](releases/2026-05-06_history-20260506-082_ios_devlog-082-4e0e6943.md) | iOS | iOS 앱 변경 이력: EXIF orientation 근본 수정 + 송사장 프로필 이미지 회전 복구 |
| 2026-05-06 | [history-20260506-084](releases/2026-05-06_history-20260506-084_web_devlog-084-3f3e3877.md) | Web | 웹/프론트엔드 변경 이력: VenuePage 크래시 체계적 수정 (4종, 전 공연장 정상화) |
| 2026-05-06 | [R1](releases/2026-05-06_R1_web_devlog-083-0cf42716.md) | Web | 웹/프론트엔드 변경 이력: SHOWS-INFO-1 ShowsPage 공간 정보 풀스택 리뉴얼 R1+R1.A (5인 팀모드) |
| 2026-05-06 | [history-20260506-085](releases/2026-05-06_history-20260506-085_web_devlog-085-3a821a23.md) | Web | 웹/프론트엔드 변경 이력: SHOWS-INFO-1 Phase 3 + hotfix: VenuePage 실 API 연결 + m.map 크래시 수정 |
| 2026-05-05 | [history-20260505-086](releases/2026-05-05_history-20260505-086_web_devlog-086-693b7f20.md) | Web | 웹/프론트엔드 변경 이력: GNB-1 공지 관리 admin 탭 + NotificationsPage 모두 삭제 제거 (단일 라운드 26분 ALL PASS) |
| 2026-05-05 | [R3](releases/2026-05-05_R3_ios_devlog-087-6ec20457.md) | iOS | iOS 앱 변경 이력: R3 P2.5 R3+R4+R5 통합 사이클 (R2 검증 후 13 도메인 회귀 fix + hotfix + EPK 라벨, 단일 team-lead 세션 4 워커 사이클 3회 + qa-devops 3회) |
| 2026-05-05 | [R3](releases/2026-05-05_R3_ios_devlog-088-f0b7f7f2.md) | iOS | iOS 앱 변경 이력: R3 Phase 2 + 2.5 ArtistDrop 풀스택 종합 라이브 (7 라운드 + 5 워커, ArtistDropPage RUNTIME BROKEN 근본 해결 + 갤러리/QR 스캐너 출시 도입) |
| 2026-05-05 | [R3](releases/2026-05-05_R3_web_devlog-089-1c825e7d.md) | Web | 웹/프론트엔드 변경 이력: R3 Round 2-A 회귀 진단 + hotfix #3 풀스택 라이브 + 세션 종료 (auto-handoff 누락) |
| 2026-05-05 | [R3](releases/2026-05-05_R3_web_devlog-090-6272c657.md) | Web | 웹/프론트엔드 변경 이력: R3 Round 2-A frontend quick wins 5건 NAS 배포 완료 |
| 2026-05-05 | [R3](releases/2026-05-05_R3_web_devlog-091-1baf5146.md) | Web | 웹/프론트엔드 변경 이력: P0-2 sweep R3 Phase 1 라이브 + 세션 종료 핸드오프 (Phase 2~5 다음 세션) |
| 2026-05-04 | [R3](releases/2026-05-04_R3_web_devlog-092-51f111ff.md) | Web | 웹/프론트엔드 변경 이력: R3 Phase 1: Tier B 6페이지 mock 의존 제거 + 실 backend 연결 |
| 2026-05-04 | [R2](releases/2026-05-04_R2_ios_devlog-093-7c6cbe03.md) | iOS | iOS 앱 변경 이력: P0-2 sweep R2: Backend↔Frontend Drift 풀스윕 (7 항목 + ECS 재배포 hotfix) 사용자 PWA PASS |
| 2026-05-04 | [R1](releases/2026-05-04_R1_web_devlog-094-6a17eff7.md) | Web | 웹/프론트엔드 변경 이력: P0-2 sweep R1: Cache Drift 도메인 (frontend invalidate + backend stored column hotfix) 사용자 PWA PASS |
| 2026-05-04 | [history-20260504-095](releases/2026-05-04_history-20260504-095_ios_devlog-095-46a49d89.md) | iOS | iOS 앱 변경 이력: GuestList 미션 종료: 종합 핸드오프 메일 + 워커 전체 stop + 강프로 exit |
| 2026-05-04 | [history-20260504-096](releases/2026-05-04_history-20260504-096_web_devlog-096-84ea14c2.md) | Web | 웹/프론트엔드 변경 이력: 휴가 복귀: iTerm+tmux 팀모드 인프라 신규 + GuestList 5라운드 사이클 (D-3 출시 가능 상태) |
| 2026-05-04 | [history-20260504-097](releases/2026-05-04_history-20260504-097_backend_devlog-097-c691a096.md) | Backend | 백엔드/API 변경 이력: GuestList 라운드 5: 호스트 invalidate 누락 + status 메시지 단순화 |
| 2026-05-04 | [history-20260504-098](releases/2026-05-04_history-20260504-098_backend_devlog-098-c01a63fc.md) | Backend | 백엔드/API 변경 이력: Warroom UI 헬스체크 false-down 해소 (URL → Tailscale) |
| 2026-04-30 | [history-20260430-099](releases/2026-04-30_history-20260430-099_backend_devlog-099-02da76ee.md) | Backend | 백엔드/API 변경 이력: health-check 이메일 발송 빈도 완화 (cooldown 1h→6h, 정기 4h→8h) |
| 2026-04-29 | [history-20260429-101](releases/2026-04-29_history-20260429-101_web_devlog-101-a8354265.md) | Web | 웹/프론트엔드 변경 이력: ShowsPage 마커 팝업 + Bottom Sheet snap 통일 + Guest List 풀스택 백엔드 연결 |
| 2026-04-29 | [history-20260429-100](releases/2026-04-29_history-20260429-100_web_devlog-100-05f93661.md) | Web | 웹/프론트엔드 변경 이력: 루트 인프라 정비 사이클 (cron 화이트리스트화 + 죽은 데몬 부활 + NAS DR 백업 복구) |
| 2026-04-29 | [history-20260429-102](releases/2026-04-29_history-20260429-102_operations_devlog-102-a1128a50.md) | Operations | 운영 자동화 변경 이력: Shows 지도 내 위치 마커 녹색→보라(#8B29D8) |
| 2026-04-29 | [history-20260429-103](releases/2026-04-29_history-20260429-103_web_devlog-103-1f6e6f5d.md) | Web | 웹/프론트엔드 변경 이력: 프로필 BottomSheet 카드 5 Phase 정리 (Listener 라벨 + RDS 실데이터 + mock 전부 삭제) |
| 2026-04-28 | [history-20260428-104](releases/2026-04-28_history-20260428-104_web_devlog-104-0bfd159a.md) | Web | 웹/프론트엔드 변경 이력: 세션 마무리 (3 repo push + 웹 앱 main merge + 백엔드 서버 cleanup + 메일) |
| 2026-04-28 | [history-20260428-105](releases/2026-04-28_history-20260428-105_web_devlog-105-c670299e.md) | Web | 웹/프론트엔드 변경 이력: Instagram 임베드 cropping 한계 확인 + Meta oEmbed 도입 후속 보류 |
| 2026-04-28 | [history-20260428-106](releases/2026-04-28_history-20260428-106_web_devlog-106-4a7e6e05.md) | Web | 웹/프론트엔드 변경 이력: Instagram iframe height 540 → 480 (댓글 입력란 cropping) |
| 2026-04-28 | [history-20260428-107](releases/2026-04-28_history-20260428-107_web_devlog-107-892fef1a.md) | Web | 웹/프론트엔드 변경 이력: createPost hook 강화 (externalLink 패턴 감지) + ECS 재배포 |
| 2026-04-28 | [history-20260428-108](releases/2026-04-28_history-20260428-108_web_devlog-108-38bd2a5d.md) | Web | 웹/프론트엔드 변경 이력: TikTok short URL backend resolve hook 추가 + ECS 재배포 |
| 2026-04-28 | [history-20260428-109](releases/2026-04-28_history-20260428-109_web_devlog-109-20e95fb1.md) | Web | 웹/프론트엔드 변경 이력: SoundCloud short URL backend resolve hook 추가 + ECS 재배포 |
| 2026-04-28 | [history-20260428-110](releases/2026-04-28_history-20260428-110_ios_devlog-110-47238f6a.md) | iOS | iOS 앱 변경 이력: SoundCloud backend select fix + ECS 재배포 + 디자인 사이트 isEmbedded fallback 배포 |
| 2026-04-28 | [history-20260428-111](releases/2026-04-28_history-20260428-111_backend_devlog-111-bbbe3b14.md) | Backend | 백엔드/API 변경 이력: Threads 자동포스팅용 내부 항목 셋업 + NAS 노출 하드닝 |
| 2026-04-28 | [history-20260428-113](releases/2026-04-28_history-20260428-113_web_devlog-113-7b650a28.md) | Web | 웹/프론트엔드 변경 이력: 웹 앱 백엔드 ECS 재배포 (mentionedUsers join enrichment 활성) |
| 2026-04-28 | [history-20260428-114](releases/2026-04-28_history-20260428-114_ios_devlog-114-8ac220bb.md) | iOS | iOS 앱 변경 이력: PostCreate toolbar swap revert + Capacitor 출시 시점 처리 메모 (commit 32) |
| 2026-04-28 | [history-20260428-115](releases/2026-04-28_history-20260428-115_ios_devlog-115-96782dfb.md) | iOS | iOS 앱 변경 이력: PostCreate toolbar 가 iOS accessory bar 자리로 내려옴 (commit 31) |
| 2026-04-28 | [history-20260428-116](releases/2026-04-28_history-20260428-116_data-pipeline_devlog-116-25885a4a.md) | Data Pipeline | 데이터 파이프라인 변경 이력: PostCreate toolbar 위치 / paddingBottom dynamic / KeyboardSheet bottomOffset (commit 30) |
| 2026-04-28 | [history-20260428-117](releases/2026-04-28_history-20260428-117_infra_devlog-117-7adc47e0.md) | Infra | 인프라/배포 변경 이력: PostCreate toolbar 키보드 위 fixed + mention sheet 빈 결과 (commit 29) |
| 2026-04-28 | [history-20260428-118](releases/2026-04-28_history-20260428-118_ios_devlog-118-f0f0610d.md) | iOS | iOS 앱 변경 이력: PostCreate textarea auto-grow → caret 빈 영역 이탈 fix (commit 28) |
| 2026-04-28 | [history-20260428-122](releases/2026-04-28_history-20260428-122_ios_devlog-122-64810e56.md) | iOS | iOS 앱 변경 이력: PostCreate 풀스크린 architectural fix 24 commits + 검증 절반 이하 (handoff) |
| 2026-04-28 | [history-20260428-119](releases/2026-04-28_history-20260428-119_backend_devlog-119-b28c3d03.md) | Backend | 백엔드/API 변경 이력: PostCreate mention chip 카드 X 본문 동기화 + caret 정렬 (commit 27) |
| 2026-04-28 | [history-20260428-120](releases/2026-04-28_history-20260428-120_web_devlog-120-901de221.md) | Web | 웹/프론트엔드 변경 이력: PostCreate mention chip 본문 시각화 + 가로 긴 프로필 카드 (commit 26) |
| 2026-04-28 | [history-20260428-121](releases/2026-04-28_history-20260428-121_ios_devlog-121-47470f87.md) | iOS | iOS 앱 변경 이력: PostCreate 8가지 사용자 수정 요청 통합 (commit 25) |
| 2026-04-28 | [history-20260428-112](releases/2026-04-28_history-20260428-112_web_devlog-112-8eec761d.md) | Web | 웹/프론트엔드 변경 이력: 디자인 사이트 main↔feature 배포 swap (햄버거 등급 매칭 검증 후 KeyboardSheet 회귀 → 즉시 복구) |
| 2026-04-27 | [history-20260427-124](releases/2026-04-27_history-20260427-124_ios_devlog-124-b56c5560.md) | iOS | iOS 앱 변경 이력: 세션 종료 (PostCreate dropdown scroll 14+ 라운드 미해결, 다음 세션 인수인계) |
| 2026-04-27 | [history-20260427-125](releases/2026-04-27_history-20260427-125_operations_devlog-125-2678f387.md) | Operations | 운영 자동화 변경 이력: PostCreate floating-ui strategy:'fixed' |
| 2026-04-27 | [history-20260427-126](releases/2026-04-27_history-20260427-126_ios_devlog-126-fb2ece1c.md) | iOS | iOS 앱 변경 이력: PostCreate vaul noBodyStyles=true (진짜 진짜 근본 — body position:fixed) |
| 2026-04-27 | [history-20260427-127](releases/2026-04-27_history-20260427-127_ios_devlog-127-56cc1df3.md) | iOS | iOS 앱 변경 이력: PostCreate @floating-ui/react 도입 (근본 production-grade) |
| 2026-04-27 | [history-20260427-128](releases/2026-04-27_history-20260427-128_ios_devlog-128-de6f4b09.md) | iOS | iOS 앱 변경 이력: PostCreate JS scroll handler 제거 + native scroll + 항목 5개 |
| 2026-04-27 | [history-20260427-129](releases/2026-04-27_history-20260427-129_infra_devlog-129-828e3b01.md) | Infra | 인프라/배포 변경 이력: PostCreate TDZ 'ze' fix (useDropdownScroll active 인자) |
| 2026-04-27 | [history-20260427-130](releases/2026-04-27_history-20260427-130_infra_devlog-130-45ff19d7.md) | Infra | 인프라/배포 변경 이력: PostCreate scroll rAF + useEffect 분리 + max-h + cursor gap (round 10) |
| 2026-04-27 | [history-20260427-131](releases/2026-04-27_history-20260427-131_ios_devlog-131-943d4a86.md) | iOS | iOS 앱 변경 이력: PostCreate Notion 스타일 floating dropdown (JS touchmove scroll) |
| 2026-04-27 | [history-20260427-132](releases/2026-04-27_history-20260427-132_ios_devlog-132-4320b0e1.md) | iOS | iOS 앱 변경 이력: PostCreate dropdown 을 ScrollPanel inline 으로 (Portal 폐기) |
| 2026-04-27 | [history-20260427-133](releases/2026-04-27_history-20260427-133_infra_devlog-133-76dc523b.md) | Infra | 인프라/배포 변경 이력: PostCreate dropdown anchor textareaRef + 외부 click 감지 |
| 2026-04-27 | [history-20260427-134](releases/2026-04-27_history-20260427-134_infra_devlog-134-282873b9.md) | Infra | 인프라/배포 변경 이력: PostCreate portal dropdown 위치 rAF loop 추적 |
| 2026-04-27 | [history-20260427-135](releases/2026-04-27_history-20260427-135_ios_devlog-135-7aebf98d.md) | iOS | iOS 앱 변경 이력: PostCreate dropdown Portal 분리 (진짜 근본 — iOS nested scroll 버그) |
| 2026-04-27 | [history-20260427-136](releases/2026-04-27_history-20260427-136_web_devlog-136-a923a866.md) | Web | 웹/프론트엔드 변경 이력: PostCreate TDZ 에러 fix (dropdownActive useEffect 위치) |
| 2026-04-27 | [history-20260427-137](releases/2026-04-27_history-20260427-137_infra_devlog-137-5bfe7b17.md) | Infra | 인프라/배포 변경 이력: PostCreate dropdown scroll 진짜 근본 해결 (textarea blur 자동 닫기 제거 + 외부 클릭 감지) |
| 2026-04-27 | [history-20260427-138](releases/2026-04-27_history-20260427-138_infra_devlog-138-6559320e.md) | Infra | 인프라/배포 변경 이력: PostCreate dropdown 에 data-vaul-no-drag (native scroll 회복) |
| 2026-04-27 | [history-20260427-139](releases/2026-04-27_history-20260427-139_ios_devlog-139-8af99e61.md) | iOS | iOS 앱 변경 이력: PostCreate select jitter + dropdown max-h + cursor 겹침 완화 |
| 2026-04-27 | [history-20260427-140](releases/2026-04-27_history-20260427-140_ios_devlog-140-10a5aa3e.md) | iOS | iOS 앱 변경 이력: PostCreate mention=artist only + event tag title special char normalize |
| 2026-04-27 | [history-20260427-141](releases/2026-04-27_history-20260427-141_ios_devlog-141-d4a9de8d.md) | iOS | iOS 앱 변경 이력: PostCreate venue 멘션 색 entity genre 컬러 + cursor 위치 명시 |
| 2026-04-27 | [history-20260427-142](releases/2026-04-27_history-20260427-142_ios_devlog-142-7d964a5d.md) | iOS | iOS 앱 변경 이력: PostCreate dropdown 스크롤 vs 탭 분리 + venue handle '@' 강제 |
| 2026-04-27 | [history-20260427-143](releases/2026-04-27_history-20260427-143_ios_devlog-143-fe78560f.md) | iOS | iOS 앱 변경 이력: PostCreate vaul keyboard handling 직접 제어 + 멘션 색 등급 컬러 |
| 2026-04-27 | [history-20260427-144](releases/2026-04-27_history-20260427-144_ios_devlog-144-85f6a6d7.md) | iOS | iOS 앱 변경 이력: PostCreate drawer 구조 재설계 (Composer fixed + ScrollPanel 분리 + inline @/# 초록 강조 재도입) |
| 2026-04-27 | [history-20260427-145](releases/2026-04-27_history-20260427-145_ios_devlog-145-0995b836.md) | iOS | iOS 앱 변경 이력: PostCreate 폴리싱 풀스택 (Lexical mention/tag chip + Spotify/SoundCloud 임베드 + LinkPreviewCard) |
| 2026-04-27 | [history-20260427-123](releases/2026-04-27_history-20260427-123_ios_devlog-123-3e2e94bc.md) | iOS | iOS 앱 변경 이력: PostCreatePage 장소 입력 필수 변경 |
| 2026-04-26 | [history-20260426-147](releases/2026-04-26_history-20260426-147_web_devlog-147-97d4f79e.md) | Web | 웹/프론트엔드 변경 이력: Today "새 멤버" ghost user 근본 수정 (백엔드 onboarding 가드) |
| 2026-04-26 | [history-20260426-148](releases/2026-04-26_history-20260426-148_web_devlog-148-add914b7.md) | Web | 웹/프론트엔드 변경 이력: 웹 앱 아티스트/리스너 카드 흰색 3버튼 + 공유 OG |
| 2026-04-26 | [history-20260426-149](releases/2026-04-26_history-20260426-149_ios_devlog-149-0037bb88.md) | iOS | iOS 앱 변경 이력: 웹 앱 PWA iOS safe-area 일괄 정리 (5회 iterate) |
| 2026-04-26 | [history-20260426-150](releases/2026-04-26_history-20260426-150_web_devlog-150-e005e5ef.md) | Web | 웹/프론트엔드 변경 이력: drift 7컬럼 fix + 출시 게이트 정지/비번찾기 정상화 + 메일 deliverability 개선 (SendGrid→SES 이전 진행) |
| 2026-04-26 | [history-20260426-151](releases/2026-04-26_history-20260426-151_web_devlog-151-026ff81a.md) | Web | 웹/프론트엔드 변경 이력: 헬스체크 후속 3건 일괄 정리 (NAS DB 노출 / launchd retry / 메일 제목 임계값) |
| 2026-04-26 | [history-20260426-152](releases/2026-04-26_history-20260426-152_backend_devlog-152-bf2c93a6.md) | Backend | 백엔드/API 변경 이력: 헬스체크 GitHub CLI ❌ 근본 수정 (revoke된 옛 인증값 동기화) |
| 2026-04-26 | [history-20260426-153](releases/2026-04-26_history-20260426-153_web_devlog-153-9ed1ea0f.md) | Web | 웹/프론트엔드 변경 이력: audit v2 cleanup 보류 결정 + grep 절차 메모 캡처 |
| 2026-04-26 | [history-20260426-154](releases/2026-04-26_history-20260426-154_backend_devlog-154-46b369f5.md) | Backend | 백엔드/API 변경 이력: sync 카운트 정확화 (synced_events vs skipped_events 분리) |
| 2026-04-26 | [history-20260426-155](releases/2026-04-26_history-20260426-155_ios_devlog-155-68bb5dc7.md) | iOS | iOS 앱 변경 이력: PWA visible 시 iOS 알림 센터 누적 자동 정리 |
| 2026-04-26 | [history-20260426-156](releases/2026-04-26_history-20260426-156_ios_devlog-156-b849ae65.md) | iOS | iOS 앱 변경 이력: PWA foreground 사용 중 OS 시스템 배너 suppress |
| 2026-04-26 | [history-20260426-157](releases/2026-04-26_history-20260426-157_ios_devlog-157-0a6453c7.md) | iOS | iOS 앱 변경 이력: DM 이미지 탭 시 cloudfront URL 노출 차단 (자체 lightbox) |
| 2026-04-26 | [history-20260426-158](releases/2026-04-26_history-20260426-158_web_devlog-158-6edfb85a.md) | Web | 웹/프론트엔드 변경 이력: Drift critical 2건 근본 해결 (artist_venue_events + domestic_settlements) + 자동화 cron |
| 2026-04-26 | [history-20260426-159](releases/2026-04-26_history-20260426-159_ios_devlog-159-ce15b903.md) | iOS | iOS 앱 변경 이력: DM/푸시 풀스택 다듬기 (입력바 + in-app banner + read 처리 + 권한 prompt) |
| 2026-04-26 | [history-20260426-160](releases/2026-04-26_history-20260426-160_web_devlog-160-2f552d6c.md) | Web | 웹/프론트엔드 변경 이력: 헬스체크 Warroom 12.5h false-down 근본 수정 |
| 2026-04-26 | [history-20260426-161](releases/2026-04-26_history-20260426-161_ios_devlog-161-3719f1b9.md) | iOS | iOS 앱 변경 이력: PWA SW update 자동 감지 강화 (acc78d0a) |
| 2026-04-26 | [history-20260426-162](releases/2026-04-26_history-20260426-162_ios_devlog-162-6be8cc66.md) | iOS | iOS 앱 변경 이력: PWA 라벨 'P.O.MFS' 원복 (manifest short_name + apple-mobile-web-app-title) |
| 2026-04-26 | [history-20260426-163](releases/2026-04-26_history-20260426-163_ios_devlog-163-78b66f17.md) | iOS | iOS 앱 변경 이력: ECS 누적 stale 해소 (웹 앱-app:17, digest 3301ebd7bf6d) + 디자인 사이트 NAS 배포 |
| 2026-04-26 | [history-20260426-164](releases/2026-04-26_history-20260426-164_ios_devlog-164-0bba5ac5.md) | iOS | iOS 앱 변경 이력: push 알림 진단 + DM 배너 본문 노출 + DMListPage 좌스와이프 삭제 |
| 2026-04-26 | [history-20260426-165](releases/2026-04-26_history-20260426-165_backend_devlog-165-e385dcc3.md) | Backend | 백엔드/API 변경 이력: chat 디버그 로그 cleanup + push subscription stale 검증 |
| 2026-04-26 | [history-20260426-166](releases/2026-04-26_history-20260426-166_web_devlog-166-072e1f0f.md) | Web | 웹/프론트엔드 변경 이력: RDS↔drizzle 컬럼 drift 전수 진단 (어제 사고 패턴 추가 위험 0 확인) |
| 2026-04-26 | [history-20260426-167](releases/2026-04-26_history-20260426-167_ios_devlog-167-315bbe54.md) | iOS | iOS 앱 변경 이력: 웹 앱/AWSDevPlan 미커밋 working tree 정리 (양 repo mirror 미완 finalize) |
| 2026-04-25 | [history-20260425-168](releases/2026-04-25_history-20260425-168_web_devlog-168-a50df303.md) | Web | 웹/프론트엔드 변경 이력: 디자인 사이트 검색 간헐 503 근본 수정 (NAS 13차) |
| 2026-04-25 | [history-20260425-169](releases/2026-04-25_history-20260425-169_ios_devlog-169-29ee6c10.md) | iOS | iOS 앱 변경 이력: DM/알림/푸시 운영 안정화 사이클 (ECS 10차 / NAS 12차) |
| 2026-04-25 | [history-20260425-170](releases/2026-04-25_history-20260425-170_web_devlog-170-0b242ee0.md) | Web | 웹/프론트엔드 변경 이력: 디자인 사이트 GNB 메시지 기능 실 API 연동 (mock 340줄+ 제거) |
| 2026-04-25 | [history-20260425-171](releases/2026-04-25_history-20260425-171_web_devlog-171-7a691717.md) | Web | 웹/프론트엔드 변경 이력: Microsite 감사 v2 완료 (근본 해결 권고 8건) |
| 2026-04-24 | [history-20260424-172](releases/2026-04-24_history-20260424-172_web_devlog-172-a97b19df.md) | Web | 웹/프론트엔드 변경 이력: community.prideofmisfits.com (AWS ECS) maintenance 모드 활성화 배포 |
| 2026-04-24 | [history-20260424-173](releases/2026-04-24_history-20260424-173_web_devlog-173-25b53f4d.md) | Web | 웹/프론트엔드 변경 이력: Replit community 사이트 maintenance 모드 강제 활성화 (kkwon 1회 예외 승인) |
| 2026-04-24 | [history-20260424-174](releases/2026-04-24_history-20260424-174_web_devlog-174-35e61da6.md) | Web | 웹/프론트엔드 변경 이력: Today 히어로 카운터 RDS 실시간화 (하드코딩 23/1247/384 → 104/1097/2103) |
| 2026-04-24 | [v1.3.0](releases/2026-04-24_v1.3.0_ios_devlog-175-348857c8.md) | iOS | iOS 앱 변경 이력: design.prideofmisfits.com 접속 장애 근본 규명 + POMFS 서버 문서 v1.3.0 정비 |
| 2026-04-23 | [history-20260423-176](releases/2026-04-23_history-20260423-176_infra_devlog-176-ddc2b7a4.md) | Infra | 인프라/배포 변경 이력: POMFS 공식 홈페이지 v2 Phase 3 QA (2차) — 폼 UI + 메일 디자인 5건 추가 수정 |
| 2026-04-23 | [history-20260423-177](releases/2026-04-23_history-20260423-177_ios_devlog-177-13abf76d.md) | iOS | iOS 앱 변경 이력: POMFS 공식 홈페이지 v2 Phase 3 staging QA (1차) — 이슈 7건 수정 + 캐시 정책 개선 |
| 2026-04-23 | [history-20260423-178](releases/2026-04-23_history-20260423-178_web_devlog-178-6f90d3d5.md) | Web | 웹/프론트엔드 변경 이력: POMFS 공식 홈페이지 v2 Phase 2-b 완료 (문의 폼 Lambda + SSM SecureString) |
| 2026-04-23 | [history-20260423-179](releases/2026-04-23_history-20260423-179_ios_devlog-179-f3cf284e.md) | iOS | iOS 앱 변경 이력: 세션 마무리: iOS 탭 보강 + MEMORY.md 55.9→13.8 KB 대규모 압축 |
| 2026-04-22 | [history-20260422-181](releases/2026-04-22_history-20260422-181_web_devlog-181-9777c9b6.md) | Web | 웹/프론트엔드 변경 이력: FeedPage TDZ 에러 핫픽스 (useEffect 순서 재배치) |
| 2026-04-22 | [history-20260422-182](releases/2026-04-22_history-20260422-182_ios_devlog-182-71a724b8.md) | iOS | iOS 앱 변경 이력: 새 포스트 카드 UX 피벗: 바텀시트 폐기 → Explore 피드 이동 + 하이라이트 |
| 2026-04-22 | [history-20260422-180](releases/2026-04-22_history-20260422-180_web_devlog-180-2d47ada3.md) | Web | 웹/프론트엔드 변경 이력: POMFS 공식 홈페이지 v2 Phase 1 + 2-a 완료 (AWS CloudFront+S3 staging 가동) |
| 2026-04-22 | [history-20260422-183](releases/2026-04-22_history-20260422-183_ios_devlog-183-83b05894.md) | iOS | iOS 앱 변경 이력: 공식 홈페이지 v2 Phase 0: 신규 리포 POMFS-official-web 생성 + SEO/스토어/폼 반영 |
| 2026-04-22 | [history-20260422-184](releases/2026-04-22_history-20260422-184_ios_devlog-184-fca45beb.md) | iOS | iOS 앱 변경 이력: PWA 업데이트 배너 iOS 잘림 해소 + 빌드 ID 주입 fast-follow |
| 2026-04-22 | [history-20260422-185](releases/2026-04-22_history-20260422-185_ios_devlog-185-dfffe2dc.md) | iOS | iOS 앱 변경 이력: Today 새 포스트 카드 클릭 상세 시트 + 본인/스태프 삭제 기능 (웹 앱) |
| 2026-04-22 | [history-20260422-186](releases/2026-04-22_history-20260422-186_ios_devlog-186-8c7fcd19.md) | iOS | iOS 앱 변경 이력: 알림 시스템 감사 + Priority A/B 풀스택 배포 (follower/staff 벨 누락 + NotificationsPage type 매핑 확장) |
| 2026-04-22 | [history-20260422-187](releases/2026-04-22_history-20260422-187_ios_devlog-187-4c291521.md) | iOS | iOS 앱 변경 이력: 디자인사이트 PWA 지원 추가 (iOS Web Push 수신 경로 개통) |
| 2026-04-22 | [history-20260422-188](releases/2026-04-22_history-20260422-188_ios_devlog-188-7c020b89.md) | iOS | iOS 앱 변경 이력: Admin Push 탭 가시성 fix + Push E2E 진단 + Members 검색/Rank API 버그 패치 |
| 2026-04-22 | [history-20260422-189](releases/2026-04-22_history-20260422-189_ios_devlog-189-eaeb438a.md) | iOS | iOS 앱 변경 이력: NotificationsPage 좌스와이프 삭제 제스처 (iOS Mail 스타일) — 디자인 사이트 배포 |
| 2026-04-22 | [history-20260422-190](releases/2026-04-22_history-20260422-190_web_devlog-190-956462d0.md) | Web | 웹/프론트엔드 변경 이력: 슈퍼관리자 allowlist 확장 (kk*******@*****.com 추가) — Members 탭 destructive action 게이트 |
| 2026-04-22 | [v0.3](releases/2026-04-22_v0.3_ios_devlog-191-128e6d66.md) | iOS | iOS 앱 변경 이력: 비밀번호 찾기 v0.3/v0.4 이터레이션 (UI 개선 + 3분 TTL + 스팸함 대응) |
| 2026-04-22 | [v0.2](releases/2026-04-22_v0.2_ios_devlog-192-8b098e93.md) | iOS | iOS 앱 변경 이력: 비밀번호 찾기 풀스택 v0.2 구현 및 배포 완료 |
| 2026-04-22 | [v0.1](releases/2026-04-22_v0.1_ios_devlog-193-f0dd7b75.md) | iOS | iOS 앱 변경 이력: 비밀번호 찾기 풀스택 v0.1→v0.2 로컬 Multi-Agent Ultraplan 재설계 (구현 미시작) |
| 2026-04-22 | [history-20260422-194](releases/2026-04-22_history-20260422-194_web_devlog-194-7d47f699.md) | Web | 웹/프론트엔드 변경 이력: 관리자 Members 탭 "일괄 삭제" 풀스택 배포 (헤더 휴지통 → 선택 모드 → Bulk Delete) |
| 2026-04-21 | [history-20260421-195](releases/2026-04-21_history-20260421-195_web_devlog-195-6a9dc739.md) | Web | 웹/프론트엔드 변경 이력: 디자인 사이트 관리자 Rank Apps 신청서 Instagram/외부 링크 버튼 작동 수정 + NAS 배포 |
| 2026-04-21 | [history-20260421-196](releases/2026-04-21_history-20260421-196_web_devlog-196-98d3cecf.md) | Web | 웹/프론트엔드 변경 이력: 디자인 사이트 관리자 Blocklist 탭 풀스택 복구 (POST 완화 + DELETE 신규) |
| 2026-04-21 | [history-20260421-197](releases/2026-04-21_history-20260421-197_web_devlog-197-249b2a41.md) | Web | 웹/프론트엔드 변경 이력: 디자인 사이트 관리자 Members 탭 3종 개선 풀스택 배포 (프로필 BottomSheet · 정지 기능 작동 · 강제 삭제 버튼) |
| 2026-04-21 | [history-20260421-198](releases/2026-04-21_history-20260421-198_ios_devlog-198-113d185b.md) | iOS | iOS 앱 변경 이력: 이메일 가입/로그인 풀스택 7 Track 통합 (SendGrid + Domain Auth + 6자리 코드 + DESIGN.md 메일) |
| 2026-04-21 | [history-20260421-199](releases/2026-04-21_history-20260421-199_web_devlog-199-1654a8d5.md) | Web | 웹/프론트엔드 변경 이력: Onboarding 완료 신호 근본 해결 (users.onboarding_completed_at 도입) |
| 2026-04-21 | [history-20260421-200](releases/2026-04-21_history-20260421-200_web_devlog-200-4c4f6a50.md) | Web | 웹/프론트엔드 변경 이력: 관리자 Blocklist 탭 복구 플랜 재검증 (구현 0건, 플랜만 확정) |
| 2026-04-21 | [history-20260421-201](releases/2026-04-21_history-20260421-201_backend_devlog-201-a63b6acc.md) | Backend | 백엔드/API 변경 이력: 관리자 패널 Email 탭 Phase 1 (+T1/T2/T4/E1 선행 보강) |
| 2026-04-21 | [history-20260421-202](releases/2026-04-21_history-20260421-202_ios_devlog-202-b4413ad3.md) | iOS | iOS 앱 변경 이력: Web FCM 제거, 디자인 사이트 VAPID Web Push 단독 체제로 정리 |
| 2026-04-21 | [history-20260421-203](releases/2026-04-21_history-20260421-203_ios_devlog-203-491f90bc.md) | iOS | iOS 앱 변경 이력: Push 후속 scope 완성 (FCM 프론트 + storage.updateUser + setupUserSettingsRoutes 배선) |
| 2026-04-21 | [history-20260421-204](releases/2026-04-21_history-20260421-204_ios_devlog-204-60b40c05.md) | iOS | iOS 앱 변경 이력: Push 구독 파이프라인 DOA 복구 (setupPushNotificationsRoutes 배선 + 프론트 VAPID 구독 흐름) |
| 2026-04-21 | [history-20260421-205](releases/2026-04-21_history-20260421-205_web_devlog-205-fdca596f.md) | Web | 웹/프론트엔드 변경 이력: GNB 벨/메세지 배지 실 DB 연결 + Push Campaign → notifications 미러링 (B 플랜 실행) |
| 2026-04-21 | [history-20260421-206](releases/2026-04-21_history-20260421-206_ios_devlog-206-0931e16e.md) | iOS | iOS 앱 변경 이력: 관리자 Push 캠페인 풀스택 신규 구현 + routes.ts 배선 누락 pre-existing 버그 수정 |
| 2026-04-21 | [history-20260421-207](releases/2026-04-21_history-20260421-207_web_devlog-207-08cbcfba.md) | Web | 웹/프론트엔드 변경 이력: KPI 회원 국가 분포 풀스택 복원 (country 입력 경로 도입 + ECS/NAS 배포) |
| 2026-04-20 | [history-20260420-208](releases/2026-04-20_history-20260420-208_ios_devlog-208-610178cf.md) | iOS | iOS 앱 변경 이력: 관리자 Push 캠페인 복원 계획 v2 (Pre-Mortem 반영 수정본) |
| 2026-04-20 | [history-20260420-209](releases/2026-04-20_history-20260420-209_ios_devlog-209-945a4f74.md) | iOS | iOS 앱 변경 이력: 관리자 Push 캠페인 풀스택 복원 계획 수립 (세션 인계) |
| 2026-04-20 | [history-20260420-210](releases/2026-04-20_history-20260420-210_ios_devlog-210-1908be47.md) | iOS | iOS 앱 변경 이력: 디자인사이트 GNB 검색 전면 구축 + 5종 고도화 + P1~P4 품질 라운드 |
| 2026-04-20 | [history-20260420-211](releases/2026-04-20_history-20260420-211_web_devlog-211-2f84a1cb.md) | Web | 웹/프론트엔드 변경 이력: Rank Apps schema drift 근본 해소 (ALTER TABLE IF NOT EXISTS 자동) |
| 2026-04-19 | [history-20260419-212](releases/2026-04-19_history-20260419-212_web_devlog-212-48042a83.md) | Web | 웹/프론트엔드 변경 이력: 관리자 패널 Rank Apps 탭 풀스택 연동 (Figma Make 디자인 활성화) |
| 2026-04-19 | [history-20260419-214](releases/2026-04-19_history-20260419-214_ios_devlog-214-f2c703b4.md) | iOS | iOS 앱 변경 이력: req.user canonical shape 정규화 미들웨어 (isLiked 근본 해결 + 크로스 디바이스 정확성) |
| 2026-04-19 | [history-20260419-215](releases/2026-04-19_history-20260419-215_web_devlog-215-910b1c44.md) | Web | 웹/프론트엔드 변경 이력: 디자인사이트 관리자 패널 31개 탭 실 API 연동 (Phase 0~5) |
| 2026-04-19 | [history-20260419-217](releases/2026-04-19_history-20260419-217_web_devlog-217-43703f5d.md) | Web | 웹/프론트엔드 변경 이력: Likes 공연 카드 우상단 "-" 제거 (가격 fallback 가드) |
| 2026-04-19 | [history-20260419-234](releases/2026-04-19_history-20260419-234_ios_devlog-234-fccc3d6d.md) | iOS | iOS 앱 변경 이력: 댓글 좋아요 500 근본 수정 + Send 버튼 분리 + 웹 앱/ECR 재배포 |
| 2026-04-19 | [history-20260419-218](releases/2026-04-19_history-20260419-218_ios_devlog-218-f1e3ec8a.md) | iOS | iOS 앱 변경 이력: 히어로 YouTube carousel 스와이프 끊김 해소 |
| 2026-04-19 | [history-20260419-219](releases/2026-04-19_history-20260419-219_web_devlog-219-29a46fa6.md) | Web | 웹/프론트엔드 변경 이력: Today "더 보기" 타겟 탭 지정 라우팅 |
| 2026-04-19 | [history-20260419-216](releases/2026-04-19_history-20260419-216_ios_devlog-216-9d716726.md) | iOS | iOS 앱 변경 이력: 공연장 상세 → 공연 탭 → 공연 상세 시트 전환 + 하트 실 API + CSP 지도 임베드 |
| 2026-04-19 | [history-20260419-220](releases/2026-04-19_history-20260419-220_web_devlog-220-2bd7b498.md) | Web | 웹/프론트엔드 변경 이력: 디자인사이트 Staff 관리자 패널 ReferenceError 수정 |
| 2026-04-19 | [history-20260419-235](releases/2026-04-19_history-20260419-235_ios_devlog-235-590b5991.md) | iOS | iOS 앱 변경 이력: 대댓글 UI + 배너 overflow + 전체 DB sequence 전수 resync |
| 2026-04-19 | [history-20260419-236](releases/2026-04-19_history-20260419-236_ios_devlog-236-f646eaf1.md) | iOS | iOS 앱 변경 이력: Feed 무한스크롤 쿼리 invalidate 누락 일괄 수정 |
| 2026-04-19 | [history-20260419-221](releases/2026-04-19_history-20260419-221_web_devlog-221-8f4102f6.md) | Web | 웹/프론트엔드 변경 이력: Today 소셜/미디어 UX 다듬기 + isLiked 서버 근본 수정 |
| 2026-04-19 | [history-20260419-237](releases/2026-04-19_history-20260419-237_ios_devlog-237-f75ca1aa.md) | iOS | iOS 앱 변경 이력: CommentBottomSheet UX 3건 (이니셜 아바타 + 대댓글 scroll + 포커스 맨아래) |
| 2026-04-19 | [history-20260419-222](releases/2026-04-19_history-20260419-222_web_devlog-222-55b1918d.md) | Web | 웹/프론트엔드 변경 이력: Feed Project 탭 실 DB 연동 + 포스터 fallback 컴포넌트 |
| 2026-04-19 | [history-20260419-238](releases/2026-04-19_history-20260419-238_ios_devlog-238-32a48bc4.md) | iOS | iOS 앱 변경 이력: 이미지 업로드 3중 버그 해소 (필드명/응답키/nginx body size) |
| 2026-04-19 | [history-20260419-241](releases/2026-04-19_history-20260419-241_ios_devlog-241-d65e8c1d.md) | iOS | iOS 앱 변경 이력: 웹 앱 RDS serial sequence 5개 일괄 resync (댓글 500 근본 원인) |
| 2026-04-19 | [history-20260419-242](releases/2026-04-19_history-20260419-242_web_devlog-242-57efafe9.md) | Web | 웹/프론트엔드 변경 이력: ProfileSettingsPage 이미지 업로드 실 연동 + 가입일 검증 |
| 2026-04-19 | [history-20260419-223](releases/2026-04-19_history-20260419-223_ios_devlog-223-f3d98833.md) | iOS | iOS 앱 변경 이력: Explore 포스트 하트 isLiked localStorage 우회 (세션 마감) |
| 2026-04-19 | [history-20260419-243](releases/2026-04-19_history-20260419-243_ios_devlog-243-bdded8d7.md) | iOS | iOS 앱 변경 이력: 댓글 iOS 자동확대 해소 + 500 진단 강화 |
| 2026-04-19 | [history-20260419-227](releases/2026-04-19_history-20260419-227_web_devlog-227-d20010bf.md) | Web | 웹/프론트엔드 변경 이력: 디자인 사이트 Likes 페이지 실 데이터 연동 (포스트/공연 탭 버그 수정) |
| 2026-04-19 | [history-20260419-224](releases/2026-04-19_history-20260419-224_ios_devlog-224-2a49f9d2.md) | iOS | iOS 앱 변경 이력: 3차 ECR 배포: 댓글 삭제 FK cascade + iframe embedUrl + SW v2 bump |
| 2026-04-19 | [history-20260419-226](releases/2026-04-19_history-20260419-226_ios_devlog-226-273a5677.md) | iOS | iOS 앱 변경 이력: 프로필 편집 세션 마무리 후속 수정 (iOS 줌 + HTML 에러 토스트) |
| 2026-04-19 | [history-20260419-225](releases/2026-04-19_history-20260419-225_web_devlog-225-085ba525.md) | Web | 웹/프론트엔드 변경 이력: Today 소셜 반응 3종 실 DB 연동 (팔로우 + 포스트 하트 + 공연 하트 신규 엔드포인트) |
| 2026-04-19 | [history-20260419-244](releases/2026-04-19_history-20260419-244_web_devlog-244-de019b6f.md) | Web | 웹/프론트엔드 변경 이력: Feed 포스트/모집/토론 작성 실 DB 연동 (Mock 해소) |
| 2026-04-19 | [history-20260419-229](releases/2026-04-19_history-20260419-229_ios_devlog-229-8a9656b0.md) | iOS | iOS 앱 변경 이력: 프로필 설정 공통 기본정보 5필드 풀스택 완성 |
| 2026-04-19 | [history-20260419-228](releases/2026-04-19_history-20260419-228_ios_devlog-228-16e878fb.md) | iOS | iOS 앱 변경 이력: 2차 ECR 배포: comment_likes.user_id NOT NULL schema drift fix |
| 2026-04-19 | [history-20260419-230](releases/2026-04-19_history-20260419-230_ios_devlog-230-8c97db3b.md) | iOS | iOS 앱 변경 이력: Feed 포스트 하트 Mock 해제 + 레거시 placeholder 숨김 |
| 2026-04-19 | [history-20260419-245](releases/2026-04-19_history-20260419-245_web_devlog-245-c0a94833.md) | Web | 웹/프론트엔드 변경 이력: ProfileSettingsPage 실유저 데이터 연동 재복원 |
| 2026-04-19 | [history-20260419-231](releases/2026-04-19_history-20260419-231_web_devlog-231-808c2956.md) | Web | 웹/프론트엔드 변경 이력: 댓글 첨부 이미지/링크 렌더 복구 + iframe 임베드 (1차 배포분) |
| 2026-04-19 | [history-20260419-213](releases/2026-04-19_history-20260419-213_web_devlog-213-c4fdc6a1.md) | Web | 웹/프론트엔드 변경 이력: scraped_artists 분리 + Discovery UI 감사 v1 + 정책 확정 (세션 인수인계) |
| 2026-04-18 | [history-20260418-232](releases/2026-04-18_history-20260418-232_infra_devlog-232-34c04572.md) | Infra | 인프라/배포 변경 이력: 구독 중 버튼 색 일관성 이터레이션 (3 커밋) |
| 2026-04-18 | [history-20260418-233](releases/2026-04-18_history-20260418-233_ios_devlog-233-682b5af9.md) | iOS | iOS 앱 변경 이력: 구독 이중 POST 제거 + 버튼 UI 안정화 + 랭킹 무한 스크롤 |
| 2026-04-18 | [history-20260418-247](releases/2026-04-18_history-20260418-247_web_devlog-247-ebdcbaa5.md) | Web | 웹/프론트엔드 변경 이력: Task #9 해결: CSP 헤더 누락 원인 재진단 (Synology 무고) |
| 2026-04-18 | [v3.6.0](releases/2026-04-18_v3.6.0_web_devlog-248-ed577ba9.md) | Web | 웹/프론트엔드 변경 이력: v3.6.0 문서 현행화 + Synology CSP SDD (#8 / #9) |
| 2026-04-18 | [history-20260418-239](releases/2026-04-18_history-20260418-239_ios_devlog-239-f7e1573d.md) | iOS | iOS 앱 변경 이력: 구독 버튼 즉시 취소 버그 해결: follows/event_venue sequence resync + 프론트 방어 |
| 2026-04-18 | [history-20260418-249](releases/2026-04-18_history-20260418-249_web_devlog-249-7dedbceb.md) | Web | 웹/프론트엔드 변경 이력: 댓글 실 DB 연동 풀 피처 + 재배포 |
| 2026-04-18 | [history-20260418-240](releases/2026-04-18_history-20260418-240_web_devlog-240-1f0d145a.md) | Web | 웹/프론트엔드 변경 이력: Artists 페이지 Figma Make mock 제거 + 랭킹/구독 실 DB 전면 연동 |
| 2026-04-18 | [history-20260418-250](releases/2026-04-18_history-20260418-250_ios_devlog-250-7dd710b7.md) | iOS | iOS 앱 변경 이력: Feed UX 자잘한 버그 3건 + 재배포 (3차) |
| 2026-04-18 | [history-20260418-251](releases/2026-04-18_history-20260418-251_web_devlog-251-18eb4a5f.md) | Web | 웹/프론트엔드 변경 이력: Feed UX 라이브 피드백 6건 수정 + 재배포 (2차) |
| 2026-04-18 | [history-20260418-252](releases/2026-04-18_history-20260418-252_web_devlog-252-29c0e51e.md) | Web | 웹/프론트엔드 변경 이력: Feed UX 라이브 피드백 4건 수정 + 재배포 |
| 2026-04-18 | [history-20260418-253](releases/2026-04-18_history-20260418-253_web_devlog-253-a5c86c34.md) | Web | 웹/프론트엔드 변경 이력: Feed 플랫폼 임베드 Phase 2~5 완료 + 재배포 |
| 2026-04-18 | [history-20260418-254](releases/2026-04-18_history-20260418-254_ios_devlog-254-c0e7fe8c.md) | iOS | iOS 앱 변경 이력: 디자인 사이트 NAS Docker 재배포 |
| 2026-04-18 | [history-20260418-255](releases/2026-04-18_history-20260418-255_web_devlog-255-8b0c07a5.md) | Web | 웹/프론트엔드 변경 이력: Feed rank bug 해제 (Phase 1) |
| 2026-04-18 | [history-20260418-256](releases/2026-04-18_history-20260418-256_backend_devlog-256-135faed8.md) | Backend | 백엔드/API 변경 이력: 단일 Dev Log 도입 (CLAUDE_DEV_LOG.md) |
| 2026-04-18 | [history-20260418-257](releases/2026-04-18_history-20260418-257_web_devlog-257-25b559fb.md) | Web | 웹/프론트엔드 변경 이력: NEON→웹 앱 리네이밍 완료 + auto-sync 이슈 해결 |
| 2026-04-18 | [history-20260418-258](releases/2026-04-18_history-20260418-258_web_devlog-258-452785d0.md) | Web | 웹/프론트엔드 변경 이력: 이미지 S3 마이그레이션 + Today 페이지 개선 (낮) |
| 2026-04-18 | [history-20260418-259](releases/2026-04-18_history-20260418-259_ios_devlog-259-da72291b.md) | iOS | iOS 앱 변경 이력: /venues/:id 화이트스크린 수정 |
| 2026-04-18 | [history-20260418-246](releases/2026-04-18_history-20260418-246_web_devlog-246-102a3ee7.md) | Web | 웹/프론트엔드 변경 이력: Discovery S3/CloudFront 이식 재적용 (핸드오프 복구) |
| 2026-04-17 | [history-20260417-260](releases/2026-04-17_history-20260417-260_ios_devlog-260-8fb41e4a.md) | iOS | iOS 앱 변경 이력: /map 전체 QA (오전~심야) |
| 2026-04-15 | [history-20260415-262](releases/2026-04-15_history-20260415-262_web_devlog-262-fce7d852.md) | Web | 웹/프론트엔드 변경 이력: 웹 앱 리디자인 백엔드 연결 |
| 2026-04-15 | [history-20260415-261](releases/2026-04-15_history-20260415-261_backend_devlog-261-57785ae5.md) | Backend | 백엔드/API 변경 이력: 웹 앱 AWS 마이그레이션 최종 완료 |
| 2026-04-14 | [history-20260414-263](releases/2026-04-14_history-20260414-263_operations_devlog-263-8393be50.md) | Operations | 운영 자동화 변경 이력: 워치독 스팸 + 대시보드 복구 + 권커맨더 라우팅 |
| 2026-04-13 | [history-20260413-264](releases/2026-04-13_history-20260413-264_data-pipeline_devlog-264-351991f6.md) | Data Pipeline | 데이터 파이프라인 변경 이력: Warroom 안정화 |
| 2026-04-11 | [history-20260411-265](releases/2026-04-11_history-20260411-265_data-pipeline_devlog-265-135b1e8d.md) | Data Pipeline | 데이터 파이프라인 변경 이력: NAS 알림 + 헬스체크 + 대시보드 수정 |
| 2026-04-10 | [history-20260410-266](releases/2026-04-10_history-20260410-266_backend_devlog-266-a181c518.md) | Backend | 백엔드/API 변경 이력: 인프라 일일 보고서 + Tailscale IP 변경 |
| 2026-04-09 | [history-20260409-267](releases/2026-04-09_history-20260409-267_backend_devlog-267-93e08ff1.md) | Backend | 백엔드/API 변경 이력: Warroom 캘린더 복구 |
| 2026-04-08 | [history-20260408-268](releases/2026-04-08_history-20260408-268_infra_devlog-268-aa5578d0.md) | Infra | 인프라/배포 변경 이력: Discord 취소 기능 구현 |
| 2026-04-07 | [history-20260407-269](releases/2026-04-07_history-20260407-269_operations_devlog-269-d6748d57.md) | Operations | 운영 자동화 변경 이력: Discord 미션컨트롤 v2 구현 |
| 2026-04-06 | [history-20260406-270](releases/2026-04-06_history-20260406-270_operations_devlog-270-eab088ba.md) | Operations | 운영 자동화 변경 이력: Mac Mini B Figma + Phase 4 전체 구현 |
| 2026-04-04 | [history-20260404-271](releases/2026-04-04_history-20260404-271_backend_devlog-271-c4cfa7c8.md) | Backend | 백엔드/API 변경 이력: 헬스체크 + PostgreSQL 복구 + 커맨더 설정 |
| 2026-04-01 | [history-20260401-272](releases/2026-04-01_history-20260401-272_infra_devlog-272-8d2cc200.md) | Infra | 인프라/배포 변경 이력: Phase 3 구현 + 대시보드 시각화 |
| 2026-03-31 | [history-20260331-273](releases/2026-03-31_history-20260331-273_operations_devlog-273-457238d6.md) | Operations | 운영 자동화 변경 이력: Meta Orchestrator Phase 2 구현 완료 |
| 2026-03-29 | [history-20260329-274](releases/2026-03-29_history-20260329-274_backend_devlog-274-659654de.md) | Backend | 백엔드/API 변경 이력: Harness 대시보드 구축 |
| 2026-03-28 | [history-20260328-275](releases/2026-03-28_history-20260328-275_backend_devlog-275-6b471951.md) | Backend | 백엔드/API 변경 이력: 미완료 작업 완료 + gitsafe-backup 복구 |
| 2026-03-26 | [history-20260326-276](releases/2026-03-26_history-20260326-276_backend_devlog-276-c0889bd9.md) | Backend | 백엔드/API 변경 이력: 서버 재구성 Phase 1-5 완료 |
| 2026-03-25 | [history-20260325-277](releases/2026-03-25_history-20260325-277_infra_devlog-277-7598d21a.md) | Infra | 인프라/배포 변경 이력: Tailscale IP 마이그레이션 |
| 2026-03-22 | [history-20260322-278](releases/2026-03-22_history-20260322-278_web_devlog-278-7f49c8ba.md) | Web | 웹/프론트엔드 변경 이력: Figma 워크플로우 D-1~D-13 완료 |
| 2026-03-21 | [history-20260321-279](releases/2026-03-21_history-20260321-279_web_devlog-279-fb1c1fcc.md) | Web | 웹/프론트엔드 변경 이력: 웹 앱 Stitch 워크플로우 완료 + Penpot→Stitch 전환 |
| 2026-03-20 | [v4.2](releases/2026-03-20_v4.2_ios_devlog-280-39d9c28b.md) | iOS | iOS 앱 변경 이력: 웹 앱 리디자인 와이어프레임 + Discord v4.2 + DICE/LiveNation 분석 |
| 2026-03-19 | [v1.0.0](releases/2026-03-19_v1.0.0_web_devlog-281-d5a04d1c.md) | Web | 웹/프론트엔드 변경 이력: CSS 토큰화 + 다크모드 + Knowledge Map v1.0.0 + Serena 제거 |
| 2026-03-18 | [history-20260318-282](releases/2026-03-18_history-20260318-282_backend_devlog-282-ce683bfd.md) | Backend | 백엔드/API 변경 이력: 에이전트 이름 변경 + Claude Code 로그아웃 해결 |
| 2026-03-15 | [v2.0](releases/2026-03-15_v2.0_web_devlog-283-df3b666c.md) | Web | 웹/프론트엔드 변경 이력: 다중팀 v2.0 재편 + Knowledge Map 설계 |

## By Component

### iOS

| Date | Version | Summary |
|---|---|---|
| 2026-05-22 | [r1.50.5](releases/2026-05-22_r1.50.5_ios_ios-ticket-deeplink-scheme.md) | iOS 앱에서 티켓 메일의 앱 열기 버튼이 티켓 화면으로 이어질 수 있도록 딥링크 처리를 보강했습니다. |
| 2026-05-22 | [r1.50.3](releases/2026-05-22_r1.50.3_ios_ios-scoped-location-webview.md) | iOS 앱에서 위치 기능이 필요한 화면에서만 동작하도록 허용 범위를 조정했습니다. |
| 2026-05-22 | [r1.50.4](releases/2026-05-22_r1.50.4_ios_ios-codex-token-usage-snapshot.md) | iOS 앱 README에서 Codex 누적 토큰 사용량을 확인할 수 있도록 공개 스냅샷을 추가했습니다. |
| 2026-05-22 | [r1.50.1](releases/2026-05-22_r1.50.1_ios_ios-payment-webview.md) | iOS 앱에서 결제 앱으로 이동하고 다시 돌아오는 흐름을 개선했습니다. |
| 2026-05-19 | [R1.49.2](releases/2026-05-19_R1.49.2_ios_devlog-002-b25a861e.md) | iOS 앱 변경 이력: R1.49.2 simpler approach fail PROVEN + session handoff base — R1.49.2 ASWebAuthenticationSession 측 다음 세션 base sustained 진행 base |
| 2026-05-10 | [R1.14](releases/2026-05-10_R1.14_ios_devlog-043-e939dfa2.md) | iOS 앱 변경 이력: R1.14 sprint Phase 1 종료 (SECURITY ECS task def env Parameter Store 이전 + 자동 회전 5건 + RDS password 회전, 권커맨더 단독) |
| 2026-05-10 | [R1.13.4](releases/2026-05-10_R1.13.4_ios_devlog-045-53b576bc.md) | iOS 앱 변경 이력: R1.13.4 sprint 종료 (AuthCallbackPage navigate() → window.location.replace, 모바일 OAuth cookie 동기화, 권커맨더 단독) |
| 2026-05-10 | [R1.13.3](releases/2026-05-10_R1.13.3_ios_devlog-046-e27d6565.md) | iOS 앱 변경 이력: R1.13.3 sprint 종료 (cookie SameSite=Lax → None, 모바일 OAuth flow 안정화, 권커맨더 단독) |
| 2026-05-09 | [R1.12.x](releases/2026-05-09_R1.12.x_ios_devlog-050-7eda34ea.md) | iOS 앱 변경 이력: cleanup endpoint 호출 SUCCESS (R1.12.x incident 데이터 정리 완료) |
| 2026-05-09 | [R1.12.12.1](releases/2026-05-09_R1.12.12.1_ios_devlog-051-52593157.md) | iOS 앱 변경 이력: R1.12.12.1 임시 hotfix backend (cleanup endpoint auth bypass + X-Cleanup-Secret) |
| 2026-05-07 | [R1.4.11](releases/2026-05-07_R1.4.11_ios_devlog-070-0e42e348.md) | iOS 앱 변경 이력: R1.4.11 #V refine4 권커맨더 단독 hotfix 종료 (TicketPurchase Drawer Content bottom 자체 들어올림, R1.4.x 12 사이클 누적) |
| 2026-05-06 | [history-20260506-082](releases/2026-05-06_history-20260506-082_ios_devlog-082-4e0e6943.md) | iOS 앱 변경 이력: EXIF orientation 근본 수정 + 송사장 프로필 이미지 회전 복구 |
| 2026-05-05 | [R3](releases/2026-05-05_R3_ios_devlog-087-6ec20457.md) | iOS 앱 변경 이력: R3 P2.5 R3+R4+R5 통합 사이클 (R2 검증 후 13 도메인 회귀 fix + hotfix + EPK 라벨, 단일 team-lead 세션 4 워커 사이클 3회 + qa-devops 3회) |
| 2026-05-05 | [R3](releases/2026-05-05_R3_ios_devlog-088-f0b7f7f2.md) | iOS 앱 변경 이력: R3 Phase 2 + 2.5 ArtistDrop 풀스택 종합 라이브 (7 라운드 + 5 워커, ArtistDropPage RUNTIME BROKEN 근본 해결 + 갤러리/QR 스캐너 출시 도입) |
| 2026-05-04 | [R2](releases/2026-05-04_R2_ios_devlog-093-7c6cbe03.md) | iOS 앱 변경 이력: P0-2 sweep R2: Backend↔Frontend Drift 풀스윕 (7 항목 + ECS 재배포 hotfix) 사용자 PWA PASS |
| 2026-05-04 | [history-20260504-095](releases/2026-05-04_history-20260504-095_ios_devlog-095-46a49d89.md) | iOS 앱 변경 이력: GuestList 미션 종료: 종합 핸드오프 메일 + 워커 전체 stop + 강프로 exit |
| 2026-04-28 | [history-20260428-110](releases/2026-04-28_history-20260428-110_ios_devlog-110-47238f6a.md) | iOS 앱 변경 이력: SoundCloud backend select fix + ECS 재배포 + 디자인 사이트 isEmbedded fallback 배포 |
| 2026-04-28 | [history-20260428-114](releases/2026-04-28_history-20260428-114_ios_devlog-114-8ac220bb.md) | iOS 앱 변경 이력: PostCreate toolbar swap revert + Capacitor 출시 시점 처리 메모 (commit 32) |
| 2026-04-28 | [history-20260428-115](releases/2026-04-28_history-20260428-115_ios_devlog-115-96782dfb.md) | iOS 앱 변경 이력: PostCreate toolbar 가 iOS accessory bar 자리로 내려옴 (commit 31) |
| 2026-04-28 | [history-20260428-118](releases/2026-04-28_history-20260428-118_ios_devlog-118-f0f0610d.md) | iOS 앱 변경 이력: PostCreate textarea auto-grow → caret 빈 영역 이탈 fix (commit 28) |
| 2026-04-28 | [history-20260428-122](releases/2026-04-28_history-20260428-122_ios_devlog-122-64810e56.md) | iOS 앱 변경 이력: PostCreate 풀스크린 architectural fix 24 commits + 검증 절반 이하 (handoff) |
| 2026-04-28 | [history-20260428-121](releases/2026-04-28_history-20260428-121_ios_devlog-121-47470f87.md) | iOS 앱 변경 이력: PostCreate 8가지 사용자 수정 요청 통합 (commit 25) |
| 2026-04-27 | [history-20260427-124](releases/2026-04-27_history-20260427-124_ios_devlog-124-b56c5560.md) | iOS 앱 변경 이력: 세션 종료 (PostCreate dropdown scroll 14+ 라운드 미해결, 다음 세션 인수인계) |
| 2026-04-27 | [history-20260427-126](releases/2026-04-27_history-20260427-126_ios_devlog-126-fb2ece1c.md) | iOS 앱 변경 이력: PostCreate vaul noBodyStyles=true (진짜 진짜 근본 — body position:fixed) |
| 2026-04-27 | [history-20260427-127](releases/2026-04-27_history-20260427-127_ios_devlog-127-56cc1df3.md) | iOS 앱 변경 이력: PostCreate @floating-ui/react 도입 (근본 production-grade) |
| 2026-04-27 | [history-20260427-128](releases/2026-04-27_history-20260427-128_ios_devlog-128-de6f4b09.md) | iOS 앱 변경 이력: PostCreate JS scroll handler 제거 + native scroll + 항목 5개 |
| 2026-04-27 | [history-20260427-131](releases/2026-04-27_history-20260427-131_ios_devlog-131-943d4a86.md) | iOS 앱 변경 이력: PostCreate Notion 스타일 floating dropdown (JS touchmove scroll) |
| 2026-04-27 | [history-20260427-132](releases/2026-04-27_history-20260427-132_ios_devlog-132-4320b0e1.md) | iOS 앱 변경 이력: PostCreate dropdown 을 ScrollPanel inline 으로 (Portal 폐기) |
| 2026-04-27 | [history-20260427-135](releases/2026-04-27_history-20260427-135_ios_devlog-135-7aebf98d.md) | iOS 앱 변경 이력: PostCreate dropdown Portal 분리 (진짜 근본 — iOS nested scroll 버그) |
| 2026-04-27 | [history-20260427-139](releases/2026-04-27_history-20260427-139_ios_devlog-139-8af99e61.md) | iOS 앱 변경 이력: PostCreate select jitter + dropdown max-h + cursor 겹침 완화 |
| 2026-04-27 | [history-20260427-140](releases/2026-04-27_history-20260427-140_ios_devlog-140-10a5aa3e.md) | iOS 앱 변경 이력: PostCreate mention=artist only + event tag title special char normalize |
| 2026-04-27 | [history-20260427-141](releases/2026-04-27_history-20260427-141_ios_devlog-141-d4a9de8d.md) | iOS 앱 변경 이력: PostCreate venue 멘션 색 entity genre 컬러 + cursor 위치 명시 |
| 2026-04-27 | [history-20260427-142](releases/2026-04-27_history-20260427-142_ios_devlog-142-7d964a5d.md) | iOS 앱 변경 이력: PostCreate dropdown 스크롤 vs 탭 분리 + venue handle '@' 강제 |
| 2026-04-27 | [history-20260427-143](releases/2026-04-27_history-20260427-143_ios_devlog-143-fe78560f.md) | iOS 앱 변경 이력: PostCreate vaul keyboard handling 직접 제어 + 멘션 색 등급 컬러 |
| 2026-04-27 | [history-20260427-144](releases/2026-04-27_history-20260427-144_ios_devlog-144-85f6a6d7.md) | iOS 앱 변경 이력: PostCreate drawer 구조 재설계 (Composer fixed + ScrollPanel 분리 + inline @/# 초록 강조 재도입) |
| 2026-04-27 | [history-20260427-145](releases/2026-04-27_history-20260427-145_ios_devlog-145-0995b836.md) | iOS 앱 변경 이력: PostCreate 폴리싱 풀스택 (Lexical mention/tag chip + Spotify/SoundCloud 임베드 + LinkPreviewCard) |
| 2026-04-27 | [history-20260427-123](releases/2026-04-27_history-20260427-123_ios_devlog-123-3e2e94bc.md) | iOS 앱 변경 이력: PostCreatePage 장소 입력 필수 변경 |
| 2026-04-26 | [history-20260426-149](releases/2026-04-26_history-20260426-149_ios_devlog-149-0037bb88.md) | iOS 앱 변경 이력: 웹 앱 PWA iOS safe-area 일괄 정리 (5회 iterate) |
| 2026-04-26 | [history-20260426-155](releases/2026-04-26_history-20260426-155_ios_devlog-155-68bb5dc7.md) | iOS 앱 변경 이력: PWA visible 시 iOS 알림 센터 누적 자동 정리 |
| 2026-04-26 | [history-20260426-156](releases/2026-04-26_history-20260426-156_ios_devlog-156-b849ae65.md) | iOS 앱 변경 이력: PWA foreground 사용 중 OS 시스템 배너 suppress |
| 2026-04-26 | [history-20260426-157](releases/2026-04-26_history-20260426-157_ios_devlog-157-0a6453c7.md) | iOS 앱 변경 이력: DM 이미지 탭 시 cloudfront URL 노출 차단 (자체 lightbox) |
| 2026-04-26 | [history-20260426-159](releases/2026-04-26_history-20260426-159_ios_devlog-159-ce15b903.md) | iOS 앱 변경 이력: DM/푸시 풀스택 다듬기 (입력바 + in-app banner + read 처리 + 권한 prompt) |
| 2026-04-26 | [history-20260426-161](releases/2026-04-26_history-20260426-161_ios_devlog-161-3719f1b9.md) | iOS 앱 변경 이력: PWA SW update 자동 감지 강화 (acc78d0a) |
| 2026-04-26 | [history-20260426-162](releases/2026-04-26_history-20260426-162_ios_devlog-162-6be8cc66.md) | iOS 앱 변경 이력: PWA 라벨 'P.O.MFS' 원복 (manifest short_name + apple-mobile-web-app-title) |
| 2026-04-26 | [history-20260426-163](releases/2026-04-26_history-20260426-163_ios_devlog-163-78b66f17.md) | iOS 앱 변경 이력: ECS 누적 stale 해소 (웹 앱-app:17, digest 3301ebd7bf6d) + 디자인 사이트 NAS 배포 |
| 2026-04-26 | [history-20260426-164](releases/2026-04-26_history-20260426-164_ios_devlog-164-0bba5ac5.md) | iOS 앱 변경 이력: push 알림 진단 + DM 배너 본문 노출 + DMListPage 좌스와이프 삭제 |
| 2026-04-26 | [history-20260426-167](releases/2026-04-26_history-20260426-167_ios_devlog-167-315bbe54.md) | iOS 앱 변경 이력: 웹 앱/AWSDevPlan 미커밋 working tree 정리 (양 repo mirror 미완 finalize) |
| 2026-04-25 | [history-20260425-169](releases/2026-04-25_history-20260425-169_ios_devlog-169-29ee6c10.md) | iOS 앱 변경 이력: DM/알림/푸시 운영 안정화 사이클 (ECS 10차 / NAS 12차) |
| 2026-04-24 | [v1.3.0](releases/2026-04-24_v1.3.0_ios_devlog-175-348857c8.md) | iOS 앱 변경 이력: design.prideofmisfits.com 접속 장애 근본 규명 + POMFS 서버 문서 v1.3.0 정비 |
| 2026-04-23 | [history-20260423-177](releases/2026-04-23_history-20260423-177_ios_devlog-177-13abf76d.md) | iOS 앱 변경 이력: POMFS 공식 홈페이지 v2 Phase 3 staging QA (1차) — 이슈 7건 수정 + 캐시 정책 개선 |
| 2026-04-23 | [history-20260423-179](releases/2026-04-23_history-20260423-179_ios_devlog-179-f3cf284e.md) | iOS 앱 변경 이력: 세션 마무리: iOS 탭 보강 + MEMORY.md 55.9→13.8 KB 대규모 압축 |
| 2026-04-22 | [history-20260422-182](releases/2026-04-22_history-20260422-182_ios_devlog-182-71a724b8.md) | iOS 앱 변경 이력: 새 포스트 카드 UX 피벗: 바텀시트 폐기 → Explore 피드 이동 + 하이라이트 |
| 2026-04-22 | [history-20260422-183](releases/2026-04-22_history-20260422-183_ios_devlog-183-83b05894.md) | iOS 앱 변경 이력: 공식 홈페이지 v2 Phase 0: 신규 리포 POMFS-official-web 생성 + SEO/스토어/폼 반영 |
| 2026-04-22 | [history-20260422-184](releases/2026-04-22_history-20260422-184_ios_devlog-184-fca45beb.md) | iOS 앱 변경 이력: PWA 업데이트 배너 iOS 잘림 해소 + 빌드 ID 주입 fast-follow |
| 2026-04-22 | [history-20260422-185](releases/2026-04-22_history-20260422-185_ios_devlog-185-dfffe2dc.md) | iOS 앱 변경 이력: Today 새 포스트 카드 클릭 상세 시트 + 본인/스태프 삭제 기능 (웹 앱) |
| 2026-04-22 | [history-20260422-186](releases/2026-04-22_history-20260422-186_ios_devlog-186-8c7fcd19.md) | iOS 앱 변경 이력: 알림 시스템 감사 + Priority A/B 풀스택 배포 (follower/staff 벨 누락 + NotificationsPage type 매핑 확장) |
| 2026-04-22 | [history-20260422-187](releases/2026-04-22_history-20260422-187_ios_devlog-187-4c291521.md) | iOS 앱 변경 이력: 디자인사이트 PWA 지원 추가 (iOS Web Push 수신 경로 개통) |
| 2026-04-22 | [history-20260422-188](releases/2026-04-22_history-20260422-188_ios_devlog-188-7c020b89.md) | iOS 앱 변경 이력: Admin Push 탭 가시성 fix + Push E2E 진단 + Members 검색/Rank API 버그 패치 |
| 2026-04-22 | [history-20260422-189](releases/2026-04-22_history-20260422-189_ios_devlog-189-eaeb438a.md) | iOS 앱 변경 이력: NotificationsPage 좌스와이프 삭제 제스처 (iOS Mail 스타일) — 디자인 사이트 배포 |
| 2026-04-22 | [v0.3](releases/2026-04-22_v0.3_ios_devlog-191-128e6d66.md) | iOS 앱 변경 이력: 비밀번호 찾기 v0.3/v0.4 이터레이션 (UI 개선 + 3분 TTL + 스팸함 대응) |
| 2026-04-22 | [v0.2](releases/2026-04-22_v0.2_ios_devlog-192-8b098e93.md) | iOS 앱 변경 이력: 비밀번호 찾기 풀스택 v0.2 구현 및 배포 완료 |
| 2026-04-22 | [v0.1](releases/2026-04-22_v0.1_ios_devlog-193-f0dd7b75.md) | iOS 앱 변경 이력: 비밀번호 찾기 풀스택 v0.1→v0.2 로컬 Multi-Agent Ultraplan 재설계 (구현 미시작) |
| 2026-04-21 | [history-20260421-198](releases/2026-04-21_history-20260421-198_ios_devlog-198-113d185b.md) | iOS 앱 변경 이력: 이메일 가입/로그인 풀스택 7 Track 통합 (SendGrid + Domain Auth + 6자리 코드 + DESIGN.md 메일) |
| 2026-04-21 | [history-20260421-202](releases/2026-04-21_history-20260421-202_ios_devlog-202-b4413ad3.md) | iOS 앱 변경 이력: Web FCM 제거, 디자인 사이트 VAPID Web Push 단독 체제로 정리 |
| 2026-04-21 | [history-20260421-203](releases/2026-04-21_history-20260421-203_ios_devlog-203-491f90bc.md) | iOS 앱 변경 이력: Push 후속 scope 완성 (FCM 프론트 + storage.updateUser + setupUserSettingsRoutes 배선) |
| 2026-04-21 | [history-20260421-204](releases/2026-04-21_history-20260421-204_ios_devlog-204-60b40c05.md) | iOS 앱 변경 이력: Push 구독 파이프라인 DOA 복구 (setupPushNotificationsRoutes 배선 + 프론트 VAPID 구독 흐름) |
| 2026-04-21 | [history-20260421-206](releases/2026-04-21_history-20260421-206_ios_devlog-206-0931e16e.md) | iOS 앱 변경 이력: 관리자 Push 캠페인 풀스택 신규 구현 + routes.ts 배선 누락 pre-existing 버그 수정 |
| 2026-04-20 | [history-20260420-208](releases/2026-04-20_history-20260420-208_ios_devlog-208-610178cf.md) | iOS 앱 변경 이력: 관리자 Push 캠페인 복원 계획 v2 (Pre-Mortem 반영 수정본) |
| 2026-04-20 | [history-20260420-209](releases/2026-04-20_history-20260420-209_ios_devlog-209-945a4f74.md) | iOS 앱 변경 이력: 관리자 Push 캠페인 풀스택 복원 계획 수립 (세션 인계) |
| 2026-04-20 | [history-20260420-210](releases/2026-04-20_history-20260420-210_ios_devlog-210-1908be47.md) | iOS 앱 변경 이력: 디자인사이트 GNB 검색 전면 구축 + 5종 고도화 + P1~P4 품질 라운드 |
| 2026-04-19 | [history-20260419-214](releases/2026-04-19_history-20260419-214_ios_devlog-214-f2c703b4.md) | iOS 앱 변경 이력: req.user canonical shape 정규화 미들웨어 (isLiked 근본 해결 + 크로스 디바이스 정확성) |
| 2026-04-19 | [history-20260419-234](releases/2026-04-19_history-20260419-234_ios_devlog-234-fccc3d6d.md) | iOS 앱 변경 이력: 댓글 좋아요 500 근본 수정 + Send 버튼 분리 + 웹 앱/ECR 재배포 |
| 2026-04-19 | [history-20260419-218](releases/2026-04-19_history-20260419-218_ios_devlog-218-f1e3ec8a.md) | iOS 앱 변경 이력: 히어로 YouTube carousel 스와이프 끊김 해소 |
| 2026-04-19 | [history-20260419-216](releases/2026-04-19_history-20260419-216_ios_devlog-216-9d716726.md) | iOS 앱 변경 이력: 공연장 상세 → 공연 탭 → 공연 상세 시트 전환 + 하트 실 API + CSP 지도 임베드 |
| 2026-04-19 | [history-20260419-235](releases/2026-04-19_history-20260419-235_ios_devlog-235-590b5991.md) | iOS 앱 변경 이력: 대댓글 UI + 배너 overflow + 전체 DB sequence 전수 resync |
| 2026-04-19 | [history-20260419-236](releases/2026-04-19_history-20260419-236_ios_devlog-236-f646eaf1.md) | iOS 앱 변경 이력: Feed 무한스크롤 쿼리 invalidate 누락 일괄 수정 |
| 2026-04-19 | [history-20260419-237](releases/2026-04-19_history-20260419-237_ios_devlog-237-f75ca1aa.md) | iOS 앱 변경 이력: CommentBottomSheet UX 3건 (이니셜 아바타 + 대댓글 scroll + 포커스 맨아래) |
| 2026-04-19 | [history-20260419-238](releases/2026-04-19_history-20260419-238_ios_devlog-238-32a48bc4.md) | iOS 앱 변경 이력: 이미지 업로드 3중 버그 해소 (필드명/응답키/nginx body size) |
| 2026-04-19 | [history-20260419-241](releases/2026-04-19_history-20260419-241_ios_devlog-241-d65e8c1d.md) | iOS 앱 변경 이력: 웹 앱 RDS serial sequence 5개 일괄 resync (댓글 500 근본 원인) |
| 2026-04-19 | [history-20260419-223](releases/2026-04-19_history-20260419-223_ios_devlog-223-f3d98833.md) | iOS 앱 변경 이력: Explore 포스트 하트 isLiked localStorage 우회 (세션 마감) |
| 2026-04-19 | [history-20260419-243](releases/2026-04-19_history-20260419-243_ios_devlog-243-bdded8d7.md) | iOS 앱 변경 이력: 댓글 iOS 자동확대 해소 + 500 진단 강화 |
| 2026-04-19 | [history-20260419-224](releases/2026-04-19_history-20260419-224_ios_devlog-224-2a49f9d2.md) | iOS 앱 변경 이력: 3차 ECR 배포: 댓글 삭제 FK cascade + iframe embedUrl + SW v2 bump |
| 2026-04-19 | [history-20260419-226](releases/2026-04-19_history-20260419-226_ios_devlog-226-273a5677.md) | iOS 앱 변경 이력: 프로필 편집 세션 마무리 후속 수정 (iOS 줌 + HTML 에러 토스트) |
| 2026-04-19 | [history-20260419-229](releases/2026-04-19_history-20260419-229_ios_devlog-229-8a9656b0.md) | iOS 앱 변경 이력: 프로필 설정 공통 기본정보 5필드 풀스택 완성 |
| 2026-04-19 | [history-20260419-228](releases/2026-04-19_history-20260419-228_ios_devlog-228-16e878fb.md) | iOS 앱 변경 이력: 2차 ECR 배포: comment_likes.user_id NOT NULL schema drift fix |
| 2026-04-19 | [history-20260419-230](releases/2026-04-19_history-20260419-230_ios_devlog-230-8c97db3b.md) | iOS 앱 변경 이력: Feed 포스트 하트 Mock 해제 + 레거시 placeholder 숨김 |
| 2026-04-18 | [history-20260418-233](releases/2026-04-18_history-20260418-233_ios_devlog-233-682b5af9.md) | iOS 앱 변경 이력: 구독 이중 POST 제거 + 버튼 UI 안정화 + 랭킹 무한 스크롤 |
| 2026-04-18 | [history-20260418-239](releases/2026-04-18_history-20260418-239_ios_devlog-239-f7e1573d.md) | iOS 앱 변경 이력: 구독 버튼 즉시 취소 버그 해결: follows/event_venue sequence resync + 프론트 방어 |
| 2026-04-18 | [history-20260418-250](releases/2026-04-18_history-20260418-250_ios_devlog-250-7dd710b7.md) | iOS 앱 변경 이력: Feed UX 자잘한 버그 3건 + 재배포 (3차) |
| 2026-04-18 | [history-20260418-254](releases/2026-04-18_history-20260418-254_ios_devlog-254-c0e7fe8c.md) | iOS 앱 변경 이력: 디자인 사이트 NAS Docker 재배포 |
| 2026-04-18 | [history-20260418-259](releases/2026-04-18_history-20260418-259_ios_devlog-259-da72291b.md) | iOS 앱 변경 이력: /venues/:id 화이트스크린 수정 |
| 2026-04-17 | [history-20260417-260](releases/2026-04-17_history-20260417-260_ios_devlog-260-8fb41e4a.md) | iOS 앱 변경 이력: /map 전체 QA (오전~심야) |
| 2026-03-20 | [v4.2](releases/2026-03-20_v4.2_ios_devlog-280-39d9c28b.md) | iOS 앱 변경 이력: 웹 앱 리디자인 와이어프레임 + Discord v4.2 + DICE/LiveNation 분석 |

### Web

| Date | Version | Summary |
|---|---|---|
| 2026-05-22 | [r1.50.3](releases/2026-05-22_r1.50.3_web_scoped-location-routes.md) | Today와 Shows에서 필요한 위치 기능을 다시 사용할 수 있도록 하면서 결제 화면에서는 위치 사용을 막았습니다. |
| 2026-05-21 | [r1.49.13](releases/2026-05-21_r1.49.13_web_event-social-links-managed-cards.md) | 공연 수정 후 상세 정보, 티켓 금액, 유튜브·인스타그램 링크 표시가 더 일관되게 반영되도록 개선했습니다. |
| 2026-05-21 | [r1.49.12](releases/2026-05-21_r1.49.12_web_managed-event-edit-navigation.md) | 공연 수정 후 관리 목록의 가격 표시와 뒤로가기 흐름을 개선했습니다. |
| 2026-05-21 | [r1.49.11](releases/2026-05-21_r1.49.11_web_likes-auth-persistence-web.md) | 앱 재실행 후에도 좋아요한 공연이 Likes 화면과 공연 상세에서 유지되도록 개선했습니다. |
| 2026-05-21 | [r1.49.10](releases/2026-05-21_r1.49.10_web_event-detail-flow.md) | 공연 상세, 좋아요, 티켓/게스트리스트, 공유 흐름의 안정성을 개선했습니다. |
| 2026-05-21 | [r1.49.10](releases/2026-05-21_r1.49.10_web_apple-login-routing-fallback-fix.md) | 운영 커뮤니티 웹에서 Apple 로그인 버튼이 잘못된 로그인 경로로 이동하던 문제를 수정했습니다. |
| 2026-05-17 | [R1.41](releases/2026-05-17_R1.41_web_devlog-008-bafb15e5.md) | 웹/프론트엔드 변경 이력: R1.41 cluster Phase B 완료 base + Phase C-E close LIVE — community.prideofmisfits.com cutover Path X (nginx reverse proxy) + 풀스택 8 워커 병렬 + Wave 1 6/6 + Wave 2 2/2 + cascade 4건 + Codex audit 2건 ALL [FINAL] LIVE + 사용자 visible 사고 0건 sustained LIVE 첫 record + R1.42+ scope cumulative 8건 보존 |
| 2026-05-17 | [R1.40](releases/2026-05-17_R1.40_web_devlog-009-40a817c3.md) | 웹/프론트엔드 변경 이력: R1.40 cluster final close GRAND TOTAL 37/37 = 100% COMPLETED LIVE 첫 record + 영구 룰 #140 정식 승격 + production endpoint design.prideofmisfits.com HTTP 200 LIVE |
| 2026-05-16 | [R1.33](releases/2026-05-16_R1.33_web_devlog-020-9b07dcf7.md) | 웹/프론트엔드 변경 이력: R1.33 + R1.34 cluster LIVE + AWS Key 영구 마스킹 (외부 모니터 자동 감지 + voice-close /exit 강화 + Codex P1 + 자율 발견 1건 cascade) |
| 2026-05-16 | [R1.38.3](releases/2026-05-16_R1.38.3_web_devlog-017-14362873.md) | 웹/프론트엔드 변경 이력: R1.38.3 cluster Phase 4 LIVE 종료 + #134/#135 영구 룰 2건 정식 승격 + LRN-NEW-118/119/120 cluster cascade |
| 2026-05-15 | [history-20260515-021](releases/2026-05-15_history-20260515-021_web_devlog-021-bda49d36.md) | 웹/프론트엔드 변경 이력: AWS Postiz 인프라 셋업 (운영 환경 NAS 호스팅용 S3 + Route53) |
| 2026-05-15 | [R1.32.x.VOICE-1.9](releases/2026-05-15_R1.32.x.VOICE-1.9_web_devlog-022-426d7c30.md) | 웹/프론트엔드 변경 이력: R1.32.x.VOICE-1.9 LIVE 영구 종료 (AF-VS-3 fix + voice-feedback.sh helper 2 함수 +4 LOC + Phase C mock TS-1 +43% over matrix) |
| 2026-05-15 | [R1.32.x.VOICE-1](releases/2026-05-15_R1.32.x.VOICE-1_web_devlog-023-b522c95e.md) | 웹/프론트엔드 변경 이력: R1.32.x.VOICE-1 LIVE 영구 종료 (voice-shutdown.sh hierarchical event-driven cascade SOP refactor + Phase B' 3 fix + LRN-NEW-101~104) |
| 2026-05-14 | [R1.28.x.HOTFIx](releases/2026-05-14_R1.28.x.HOTFIx_web_devlog-024-8d5935c7.md) | 웹/프론트엔드 변경 이력: R1.28.x.HOTFIX LIVE 영구 종료 final + ECS deploy 진정 완료 + Bug #2 fix LIVE 적용 확정 |
| 2026-05-14 | [R1.28.x](releases/2026-05-14_R1.28.x_web_devlog-025-8229bf9d.md) | 웹/프론트엔드 변경 이력: R1.28.x sub-sprint LIVE 영구 종료 final + 웹 앱 /api/logout Google IdP revocation LIVE 적용 (R1.28.4 사용자 명시 GO 정합) |
| 2026-05-14 | [R1.28](releases/2026-05-14_R1.28_web_devlog-026-72c31f18.md) | 웹/프론트엔드 변경 이력: R1.28 sub-sprint LIVE 영구 종료 final + 디자인 사이트 로그아웃 버그 fix LIVE deployed |
| 2026-05-12 | [R1.19.13](releases/2026-05-12_R1.19.13_web_devlog-027-8ff53d0f.md) | 웹/프론트엔드 변경 이력: R1.19.13 iTerm Status Bar broadcaster Phase 1~5 LIVE 종료 + 3건 사고 영구 제거 + LRN-NEW-55 등재 |
| 2026-05-12 | [R1.19.6](releases/2026-05-12_R1.19.6_web_devlog-029-52b1b6d8.md) | 웹/프론트엔드 변경 이력: R1.19.6 진정 ECS LIVE PASS (5/12 03:13 false claim 정정) + task def digest pin 영구 회피 + LRN-NEW-51 등재 |
| 2026-05-12 | [R1.19.6](releases/2026-05-12_R1.19.6_web_devlog-030-4cdc8643.md) | 웹/프론트엔드 변경 이력: R1.19.6 ECS LIVE PASS + R1.19.8 hotfix #3 loading state per-card 분리 PASS + LRN-NEW-50 등재 |
| 2026-05-12 | [R1.19.6](releases/2026-05-12_R1.19.6_web_devlog-031-4a9cfa65.md) | 웹/프론트엔드 변경 이력: R1.19.6 FF-A: 백엔드 서버 adminTickets jsonb fallback precedence commit+push + LRN-NEW-48/49 등재 (A+B-2 일괄) |
| 2026-05-11 | [R1.19.5](releases/2026-05-11_R1.19.5_web_devlog-035-9712b550.md) | 웹/프론트엔드 변경 이력: R1.19.5 Phase 1 박수 폐기 결정 + 권커맨더 단독 핸드오프 + Phase 2 prep (HOF-022 발행) |
| 2026-05-11 | [R1.19.5](releases/2026-05-11_R1.19.5_web_devlog-036-11e6ab5e.md) | 웹/프론트엔드 변경 이력: R1.19.5 Phase 1 박수 detect LIVE + 컴퓨터 재시작 핸드오프 (HOF-021 발행) |
| 2026-05-11 | [R1.19.4](releases/2026-05-11_R1.19.4_web_devlog-037-70a681f4.md) | 웹/프론트엔드 변경 이력: R1.19.4 sprint 풀스택 100% LIVE + R1.19.5 자동화 음성 trigger 100% PASS + 사용자 명시 fresh spawn 의뢰 (HOF-020 발행) |
| 2026-05-11 | [R1.19.5](releases/2026-05-11_R1.19.5_web_devlog-033-0f42f8c5.md) | 웹/프론트엔드 변경 이력: R1.19.5 Phase 3 v3 sprint 영구 종료 + 페어 명령 2단계 분리 사용자 verbatim 시연 LIVE 100% 입증 + #91 LRN-NEW-35 LIVE 7번째 + LRN-NEW-36/37 등재 |
| 2026-05-10 | [R1.18](releases/2026-05-10_R1.18_web_devlog-039-7db09b85.md) | 웹/프론트엔드 변경 이력: R1.18 sprint 영구 종료 + HOF-017 발행 + 영구 메모리 4건 등재 (#78~#81, 자율 자동화 75% LIVE 입증) |
| 2026-05-10 | [R1.15](releases/2026-05-10_R1.15_web_devlog-040-c2c413d1.md) | 웹/프론트엔드 변경 이력: R1.15 sprint 영구 종료 + HOF-016 발행 + R1.18 이메일 발송 (#77 절차 첫 입증, A+B 동시 진행) |
| 2026-05-10 | [R1.14](releases/2026-05-10_R1.14_web_devlog-041-9af86315.md) | 웹/프론트엔드 변경 이력: HOF-014 발행 (R1.14 Phase 1 + R1.12.14 사이클, 사용자 명시 의뢰) |
| 2026-05-10 | [R1.12.14](releases/2026-05-10_R1.12.14_web_devlog-042-86703d8c.md) | 웹/프론트엔드 변경 이력: R1.12.14 sprint 종료 (confirm flow db.transaction wrap + 자동 환불 mutation, 권커맨더 단독) |
| 2026-05-10 | [R1.13.2](releases/2026-05-10_R1.13.2_web_devlog-044-f5ee36a8.md) | 웹/프론트엔드 변경 이력: HOF-013 발행 (R1.13.2 + R1.13.3 + R1.13.4 사이클, 사용자 명시 의뢰) |
| 2026-05-09 | [R1.13.2](releases/2026-05-09_R1.13.2_web_devlog-047-eaa1ee8d.md) | 웹/프론트엔드 변경 이력: R1.13.2 sprint 종료 (ShowsPage 전 세계 마커 회귀 영구 제거, pg-pool + statement_timeout 강화, 권커맨더 단독) |
| 2026-05-09 | [R1.12.12.1](releases/2026-05-09_R1.12.12.1_web_devlog-048-6a3d72cb.md) | 웹/프론트엔드 변경 이력: HOF-012 발행 (R1.12.12.1 cleanup 사이클 + 이메일/SMS 샘플 검증, 사용자 명시 의뢰) |
| 2026-05-09 | [R1.13.1](releases/2026-05-09_R1.13.1_web_devlog-053-89c1480d.md) | 웹/프론트엔드 변경 이력: R1.13.1 sprint 종료 (ShowsPage list view 카드 onClick 누락 영구 제거, 권커맨더 단독) |
| 2026-05-08 | [R1.12.11](releases/2026-05-08_R1.12.11_web_devlog-054-ca404afc.md) | 웹/프론트엔드 변경 이력: R1.12.11 sprint 종료 (confirm flow entry_token NOT NULL 위반 영구 제거, 권커맨더 단독) |
| 2026-05-08 | [R1.12.10](releases/2026-05-08_R1.12.10_web_devlog-056-ea176952.md) | 웹/프론트엔드 변경 이력: R1.12.10 sprint 종료 (jsonb 분기 sold_count UPDATE + frontend remaining 차감, 권커맨더 단독) |
| 2026-05-08 | [R1.12.9](releases/2026-05-08_R1.12.9_web_devlog-057-ada1c59e.md) | 웹/프론트엔드 변경 이력: R1.12.9 sprint 종료 (Toss confirm jsonb 분기 통합, 권커맨더 단독) |
| 2026-05-08 | [R1.13](releases/2026-05-08_R1.13_web_devlog-058-85a0d313.md) | 웹/프론트엔드 변경 이력: R1.13 sprint 결제+티켓 영역 mock 100% 제거 (7 페이지 backend wire, 권커맨더 단독) |
| 2026-05-08 | [R1.12](releases/2026-05-08_R1.12_web_devlog-059-6874e3b7.md) | 웹/프론트엔드 변경 이력: R1.12 sprint #C event source-of-truth (R1.10/R1.11 잔존 회귀 hotfix, 권커맨더 단독) |
| 2026-05-08 | [R1.11](releases/2026-05-08_R1.11_web_devlog-061-dd52865e.md) | 웹/프론트엔드 변경 이력: R1.11 sprint 종료 (#B' 영구 fix backend 모든 분기 검증 통일) |
| 2026-05-08 | [R1.10](releases/2026-05-08_R1.10_web_devlog-062-d550606b.md) | 웹/프론트엔드 변경 이력: R1.10 sprint 종료 (snap=[1] revert + #B' eventType 분기 영구 fix) |
| 2026-05-08 | [R1.9](releases/2026-05-08_R1.9_web_devlog-063-be480d8a.md) | 웹/프론트엔드 변경 이력: R1.9 sprint 종료 (R1.8 PWA 회귀 P0 hotfix #3 + 사용자 명시 의지 정합) |
| 2026-05-08 | [R1.8](releases/2026-05-08_R1.8_web_devlog-064-752456aa.md) | 웹/프론트엔드 변경 이력: R1.8 sprint 종료 (R1.7 PWA 회귀 P0 hotfix #2) |
| 2026-05-08 | [R1.7](releases/2026-05-08_R1.7_web_devlog-065-1cd252c8.md) | 웹/프론트엔드 변경 이력: R1.7 sprint 종료 (R1.6 PWA 회귀 P0 hotfix) |
| 2026-05-08 | [R1.6](releases/2026-05-08_R1.6_web_devlog-066-e7c20ef5.md) | 웹/프론트엔드 변경 이력: R1.6 sprint TicketPurchase architecture refactor 종료 |
| 2026-05-08 | [R1.5.x](releases/2026-05-08_R1.5.x_web_devlog-067-37599964.md) | 웹/프론트엔드 변경 이력: R1.5.x 4 sprint 누적 후 권커맨더 + 5워커 fresh spawn 인계 (R1.5.3 진행 중 + HOF-2026-05-08-001 발행) |
| 2026-05-07 | [R1.5.1](releases/2026-05-07_R1.5.1_web_devlog-068-d82f1793.md) | 웹/프론트엔드 변경 이력: R1.5.1 + R1.5.2 hotfix 통합 종료 (사용자 PWA 시연 발견 사고 2 라운드, footer prop 분리 + BottomSheet minHeight + 숫자 입력 0 prefix) |
| 2026-05-07 | [R1.5](releases/2026-05-07_R1.5_web_devlog-069-52a18603.md) | 웹/프론트엔드 변경 이력: R1.5 sprint 종료 27 BottomSheet 시스템적 근본 fix 옵션 E 완료 (5워커 풀 정합 ~68min, ai-engineer §11 ETA 150-180min 대비 -55~-62% 단축) |
| 2026-05-07 | [R1.3](releases/2026-05-07_R1.3_web_devlog-072-7cee802b.md) | 웹/프론트엔드 변경 이력: R1.3 More + Settlement + 결제 풀구현 + R0a frontend 4건 + Fast-follow #6 통합 종료 (출시 차단 5건 → 0건 100% 달성, mock 100% 제거, 누적 R0a~R1.3 출시 차단 28건 → 0건) |
| 2026-05-07 | [R2.7](releases/2026-05-07_R2.7_web_devlog-073-6b96a426.md) | 웹/프론트엔드 변경 이력: R2.7 admin 데이터 안 보임 회귀 4건 + 신규 사고 #5 visibility mismatch 통합 hotfix 종료 (출시 차단 5건 → 0건 100% 달성, 누적 R0a~R2.7 출시 차단 23건 → 0건) |
| 2026-05-07 | [R2.5](releases/2026-05-07_R2.5_web_devlog-074-1eb80900.md) | 웹/프론트엔드 변경 이력: R2.5 + R2.6 사이클 권커맨더 단독 인계 종료 (5 워커 stuck/missed 사고 학습 + admin 5 사고 fix + bundle -26% minify) |
| 2026-05-07 | [R1.3](releases/2026-05-07_R1.3_web_devlog-071-b7fb7cdb.md) | 웹/프론트엔드 변경 이력: R1.3 PWA 시연 + 실 결제 테스트 시나리오 상세 가이드 발행 (HOF-005, 권커맨더 재진입 후 인수인계 자료) |
| 2026-05-06 | [R2](releases/2026-05-06_R2_web_devlog-075-479e916b.md) | 웹/프론트엔드 변경 이력: R2 회귀 sweep + Fast-follow 통합 hotfix 종료 + R0a~R2 누적 통합 (출시 차단 14건 → 0건 100% 달성, 거버넌스 §F 19/19 정합, 사고 1건 즉시 회피) |
| 2026-05-06 | [R1.2.d](releases/2026-05-06_R1.2.d_web_devlog-076-fc4536b6.md) | 웹/프론트엔드 변경 이력: R1.2.d admin sub-라운드 4 풀스택 종료 + R1.2 4 sub 통합 종료 (22 항목 admin 풀스택 wire 완전 종료, 출시 차단 신규 0, 마스터 플랜 in-target, 사고 0건 첫 라운드) |
| 2026-05-06 | [R1.2.c](releases/2026-05-06_R1.2.c_web_devlog-077-97514a29.md) | 웹/프론트엔드 변경 이력: R1.2.c admin sub-라운드 3 풀스택 종료 (출시 차단 신규 0, 마스터 플랜 in-target, team-lead fresh spawn 의무) |
| 2026-05-06 | [R1.2.b](releases/2026-05-06_R1.2.b_web_devlog-078-79fa072b.md) | 웹/프론트엔드 변경 이력: R1.2.b admin sub-라운드 2 풀스택 종료 (출시 차단 신규 0, 마스터 플랜 -50%) |
| 2026-05-06 | [R1.2.a](releases/2026-05-06_R1.2.a_web_devlog-284-0c6c6bce.md) | 웹/프론트엔드 변경 이력: R1.2.a admin sub-라운드 1 풀스택 종료 + 권커맨더+team-lead 동시 fresh spawn 시점 |
| 2026-05-06 | [R1.2.a](releases/2026-05-06_R1.2.a_web_devlog-079-d8d89321.md) | 웹/프론트엔드 변경 이력: R1.2.a admin sub-라운드 1 풀스택 종료 (Services hotfix 포함, 거버넌스 §F 7/7 정합) |
| 2026-05-06 | [R1.1](releases/2026-05-06_R1.1_web_devlog-080-86947c8f.md) | 웹/프론트엔드 변경 이력: R1.1 DB 정합성 풀스택 종료 (Phase A→B→E ALL PASS, G1 게이트 진입) |
| 2026-05-06 | [history-20260506-081](releases/2026-05-06_history-20260506-081_web_devlog-081-a3685a09.md) | 웹/프론트엔드 변경 이력: R0a 인프라 전수 audit 종료 (출시 차단 14건 발견) |
| 2026-05-06 | [history-20260506-084](releases/2026-05-06_history-20260506-084_web_devlog-084-3f3e3877.md) | 웹/프론트엔드 변경 이력: VenuePage 크래시 체계적 수정 (4종, 전 공연장 정상화) |
| 2026-05-06 | [R1](releases/2026-05-06_R1_web_devlog-083-0cf42716.md) | 웹/프론트엔드 변경 이력: SHOWS-INFO-1 ShowsPage 공간 정보 풀스택 리뉴얼 R1+R1.A (5인 팀모드) |
| 2026-05-06 | [history-20260506-085](releases/2026-05-06_history-20260506-085_web_devlog-085-3a821a23.md) | 웹/프론트엔드 변경 이력: SHOWS-INFO-1 Phase 3 + hotfix: VenuePage 실 API 연결 + m.map 크래시 수정 |
| 2026-05-05 | [history-20260505-086](releases/2026-05-05_history-20260505-086_web_devlog-086-693b7f20.md) | 웹/프론트엔드 변경 이력: GNB-1 공지 관리 admin 탭 + NotificationsPage 모두 삭제 제거 (단일 라운드 26분 ALL PASS) |
| 2026-05-05 | [R3](releases/2026-05-05_R3_web_devlog-089-1c825e7d.md) | 웹/프론트엔드 변경 이력: R3 Round 2-A 회귀 진단 + hotfix #3 풀스택 라이브 + 세션 종료 (auto-handoff 누락) |
| 2026-05-05 | [R3](releases/2026-05-05_R3_web_devlog-090-6272c657.md) | 웹/프론트엔드 변경 이력: R3 Round 2-A frontend quick wins 5건 NAS 배포 완료 |
| 2026-05-05 | [R3](releases/2026-05-05_R3_web_devlog-091-1baf5146.md) | 웹/프론트엔드 변경 이력: P0-2 sweep R3 Phase 1 라이브 + 세션 종료 핸드오프 (Phase 2~5 다음 세션) |
| 2026-05-04 | [R3](releases/2026-05-04_R3_web_devlog-092-51f111ff.md) | 웹/프론트엔드 변경 이력: R3 Phase 1: Tier B 6페이지 mock 의존 제거 + 실 backend 연결 |
| 2026-05-04 | [R1](releases/2026-05-04_R1_web_devlog-094-6a17eff7.md) | 웹/프론트엔드 변경 이력: P0-2 sweep R1: Cache Drift 도메인 (frontend invalidate + backend stored column hotfix) 사용자 PWA PASS |
| 2026-05-04 | [history-20260504-096](releases/2026-05-04_history-20260504-096_web_devlog-096-84ea14c2.md) | 웹/프론트엔드 변경 이력: 휴가 복귀: iTerm+tmux 팀모드 인프라 신규 + GuestList 5라운드 사이클 (D-3 출시 가능 상태) |
| 2026-04-29 | [history-20260429-101](releases/2026-04-29_history-20260429-101_web_devlog-101-a8354265.md) | 웹/프론트엔드 변경 이력: ShowsPage 마커 팝업 + Bottom Sheet snap 통일 + Guest List 풀스택 백엔드 연결 |
| 2026-04-29 | [history-20260429-100](releases/2026-04-29_history-20260429-100_web_devlog-100-05f93661.md) | 웹/프론트엔드 변경 이력: 루트 인프라 정비 사이클 (cron 화이트리스트화 + 죽은 데몬 부활 + NAS DR 백업 복구) |
| 2026-04-29 | [history-20260429-103](releases/2026-04-29_history-20260429-103_web_devlog-103-1f6e6f5d.md) | 웹/프론트엔드 변경 이력: 프로필 BottomSheet 카드 5 Phase 정리 (Listener 라벨 + RDS 실데이터 + mock 전부 삭제) |
| 2026-04-28 | [history-20260428-104](releases/2026-04-28_history-20260428-104_web_devlog-104-0bfd159a.md) | 웹/프론트엔드 변경 이력: 세션 마무리 (3 repo push + 웹 앱 main merge + 백엔드 서버 cleanup + 메일) |
| 2026-04-28 | [history-20260428-105](releases/2026-04-28_history-20260428-105_web_devlog-105-c670299e.md) | 웹/프론트엔드 변경 이력: Instagram 임베드 cropping 한계 확인 + Meta oEmbed 도입 후속 보류 |
| 2026-04-28 | [history-20260428-106](releases/2026-04-28_history-20260428-106_web_devlog-106-4a7e6e05.md) | 웹/프론트엔드 변경 이력: Instagram iframe height 540 → 480 (댓글 입력란 cropping) |
| 2026-04-28 | [history-20260428-107](releases/2026-04-28_history-20260428-107_web_devlog-107-892fef1a.md) | 웹/프론트엔드 변경 이력: createPost hook 강화 (externalLink 패턴 감지) + ECS 재배포 |
| 2026-04-28 | [history-20260428-108](releases/2026-04-28_history-20260428-108_web_devlog-108-38bd2a5d.md) | 웹/프론트엔드 변경 이력: TikTok short URL backend resolve hook 추가 + ECS 재배포 |
| 2026-04-28 | [history-20260428-109](releases/2026-04-28_history-20260428-109_web_devlog-109-20e95fb1.md) | 웹/프론트엔드 변경 이력: SoundCloud short URL backend resolve hook 추가 + ECS 재배포 |
| 2026-04-28 | [history-20260428-113](releases/2026-04-28_history-20260428-113_web_devlog-113-7b650a28.md) | 웹/프론트엔드 변경 이력: 웹 앱 백엔드 ECS 재배포 (mentionedUsers join enrichment 활성) |
| 2026-04-28 | [history-20260428-120](releases/2026-04-28_history-20260428-120_web_devlog-120-901de221.md) | 웹/프론트엔드 변경 이력: PostCreate mention chip 본문 시각화 + 가로 긴 프로필 카드 (commit 26) |
| 2026-04-28 | [history-20260428-112](releases/2026-04-28_history-20260428-112_web_devlog-112-8eec761d.md) | 웹/프론트엔드 변경 이력: 디자인 사이트 main↔feature 배포 swap (햄버거 등급 매칭 검증 후 KeyboardSheet 회귀 → 즉시 복구) |
| 2026-04-27 | [history-20260427-136](releases/2026-04-27_history-20260427-136_web_devlog-136-a923a866.md) | 웹/프론트엔드 변경 이력: PostCreate TDZ 에러 fix (dropdownActive useEffect 위치) |
| 2026-04-26 | [history-20260426-147](releases/2026-04-26_history-20260426-147_web_devlog-147-97d4f79e.md) | 웹/프론트엔드 변경 이력: Today "새 멤버" ghost user 근본 수정 (백엔드 onboarding 가드) |
| 2026-04-26 | [history-20260426-148](releases/2026-04-26_history-20260426-148_web_devlog-148-add914b7.md) | 웹/프론트엔드 변경 이력: 웹 앱 아티스트/리스너 카드 흰색 3버튼 + 공유 OG |
| 2026-04-26 | [history-20260426-150](releases/2026-04-26_history-20260426-150_web_devlog-150-e005e5ef.md) | 웹/프론트엔드 변경 이력: drift 7컬럼 fix + 출시 게이트 정지/비번찾기 정상화 + 메일 deliverability 개선 (SendGrid→SES 이전 진행) |
| 2026-04-26 | [history-20260426-151](releases/2026-04-26_history-20260426-151_web_devlog-151-026ff81a.md) | 웹/프론트엔드 변경 이력: 헬스체크 후속 3건 일괄 정리 (NAS DB 노출 / launchd retry / 메일 제목 임계값) |
| 2026-04-26 | [history-20260426-153](releases/2026-04-26_history-20260426-153_web_devlog-153-9ed1ea0f.md) | 웹/프론트엔드 변경 이력: audit v2 cleanup 보류 결정 + grep 절차 메모 캡처 |
| 2026-04-26 | [history-20260426-158](releases/2026-04-26_history-20260426-158_web_devlog-158-6edfb85a.md) | 웹/프론트엔드 변경 이력: Drift critical 2건 근본 해결 (artist_venue_events + domestic_settlements) + 자동화 cron |
| 2026-04-26 | [history-20260426-160](releases/2026-04-26_history-20260426-160_web_devlog-160-2f552d6c.md) | 웹/프론트엔드 변경 이력: 헬스체크 Warroom 12.5h false-down 근본 수정 |
| 2026-04-26 | [history-20260426-166](releases/2026-04-26_history-20260426-166_web_devlog-166-072e1f0f.md) | 웹/프론트엔드 변경 이력: RDS↔drizzle 컬럼 drift 전수 진단 (어제 사고 패턴 추가 위험 0 확인) |
| 2026-04-25 | [history-20260425-168](releases/2026-04-25_history-20260425-168_web_devlog-168-a50df303.md) | 웹/프론트엔드 변경 이력: 디자인 사이트 검색 간헐 503 근본 수정 (NAS 13차) |
| 2026-04-25 | [history-20260425-170](releases/2026-04-25_history-20260425-170_web_devlog-170-0b242ee0.md) | 웹/프론트엔드 변경 이력: 디자인 사이트 GNB 메시지 기능 실 API 연동 (mock 340줄+ 제거) |
| 2026-04-25 | [history-20260425-171](releases/2026-04-25_history-20260425-171_web_devlog-171-7a691717.md) | 웹/프론트엔드 변경 이력: Microsite 감사 v2 완료 (근본 해결 권고 8건) |
| 2026-04-24 | [history-20260424-172](releases/2026-04-24_history-20260424-172_web_devlog-172-a97b19df.md) | 웹/프론트엔드 변경 이력: community.prideofmisfits.com (AWS ECS) maintenance 모드 활성화 배포 |
| 2026-04-24 | [history-20260424-173](releases/2026-04-24_history-20260424-173_web_devlog-173-25b53f4d.md) | 웹/프론트엔드 변경 이력: Replit community 사이트 maintenance 모드 강제 활성화 (kkwon 1회 예외 승인) |
| 2026-04-24 | [history-20260424-174](releases/2026-04-24_history-20260424-174_web_devlog-174-35e61da6.md) | 웹/프론트엔드 변경 이력: Today 히어로 카운터 RDS 실시간화 (하드코딩 23/1247/384 → 104/1097/2103) |
| 2026-04-23 | [history-20260423-178](releases/2026-04-23_history-20260423-178_web_devlog-178-6f90d3d5.md) | 웹/프론트엔드 변경 이력: POMFS 공식 홈페이지 v2 Phase 2-b 완료 (문의 폼 Lambda + SSM SecureString) |
| 2026-04-22 | [history-20260422-181](releases/2026-04-22_history-20260422-181_web_devlog-181-9777c9b6.md) | 웹/프론트엔드 변경 이력: FeedPage TDZ 에러 핫픽스 (useEffect 순서 재배치) |
| 2026-04-22 | [history-20260422-180](releases/2026-04-22_history-20260422-180_web_devlog-180-2d47ada3.md) | 웹/프론트엔드 변경 이력: POMFS 공식 홈페이지 v2 Phase 1 + 2-a 완료 (AWS CloudFront+S3 staging 가동) |
| 2026-04-22 | [history-20260422-190](releases/2026-04-22_history-20260422-190_web_devlog-190-956462d0.md) | 웹/프론트엔드 변경 이력: 슈퍼관리자 allowlist 확장 (kk*******@*****.com 추가) — Members 탭 destructive action 게이트 |
| 2026-04-22 | [history-20260422-194](releases/2026-04-22_history-20260422-194_web_devlog-194-7d47f699.md) | 웹/프론트엔드 변경 이력: 관리자 Members 탭 "일괄 삭제" 풀스택 배포 (헤더 휴지통 → 선택 모드 → Bulk Delete) |
| 2026-04-21 | [history-20260421-195](releases/2026-04-21_history-20260421-195_web_devlog-195-6a9dc739.md) | 웹/프론트엔드 변경 이력: 디자인 사이트 관리자 Rank Apps 신청서 Instagram/외부 링크 버튼 작동 수정 + NAS 배포 |
| 2026-04-21 | [history-20260421-196](releases/2026-04-21_history-20260421-196_web_devlog-196-98d3cecf.md) | 웹/프론트엔드 변경 이력: 디자인 사이트 관리자 Blocklist 탭 풀스택 복구 (POST 완화 + DELETE 신규) |
| 2026-04-21 | [history-20260421-197](releases/2026-04-21_history-20260421-197_web_devlog-197-249b2a41.md) | 웹/프론트엔드 변경 이력: 디자인 사이트 관리자 Members 탭 3종 개선 풀스택 배포 (프로필 BottomSheet · 정지 기능 작동 · 강제 삭제 버튼) |
| 2026-04-21 | [history-20260421-199](releases/2026-04-21_history-20260421-199_web_devlog-199-1654a8d5.md) | 웹/프론트엔드 변경 이력: Onboarding 완료 신호 근본 해결 (users.onboarding_completed_at 도입) |
| 2026-04-21 | [history-20260421-200](releases/2026-04-21_history-20260421-200_web_devlog-200-4c4f6a50.md) | 웹/프론트엔드 변경 이력: 관리자 Blocklist 탭 복구 플랜 재검증 (구현 0건, 플랜만 확정) |
| 2026-04-21 | [history-20260421-205](releases/2026-04-21_history-20260421-205_web_devlog-205-fdca596f.md) | 웹/프론트엔드 변경 이력: GNB 벨/메세지 배지 실 DB 연결 + Push Campaign → notifications 미러링 (B 플랜 실행) |
| 2026-04-21 | [history-20260421-207](releases/2026-04-21_history-20260421-207_web_devlog-207-08cbcfba.md) | 웹/프론트엔드 변경 이력: KPI 회원 국가 분포 풀스택 복원 (country 입력 경로 도입 + ECS/NAS 배포) |
| 2026-04-20 | [history-20260420-211](releases/2026-04-20_history-20260420-211_web_devlog-211-2f84a1cb.md) | 웹/프론트엔드 변경 이력: Rank Apps schema drift 근본 해소 (ALTER TABLE IF NOT EXISTS 자동) |
| 2026-04-19 | [history-20260419-212](releases/2026-04-19_history-20260419-212_web_devlog-212-48042a83.md) | 웹/프론트엔드 변경 이력: 관리자 패널 Rank Apps 탭 풀스택 연동 (Figma Make 디자인 활성화) |
| 2026-04-19 | [history-20260419-215](releases/2026-04-19_history-20260419-215_web_devlog-215-910b1c44.md) | 웹/프론트엔드 변경 이력: 디자인사이트 관리자 패널 31개 탭 실 API 연동 (Phase 0~5) |
| 2026-04-19 | [history-20260419-217](releases/2026-04-19_history-20260419-217_web_devlog-217-43703f5d.md) | 웹/프론트엔드 변경 이력: Likes 공연 카드 우상단 "-" 제거 (가격 fallback 가드) |
| 2026-04-19 | [history-20260419-219](releases/2026-04-19_history-20260419-219_web_devlog-219-29a46fa6.md) | 웹/프론트엔드 변경 이력: Today "더 보기" 타겟 탭 지정 라우팅 |
| 2026-04-19 | [history-20260419-220](releases/2026-04-19_history-20260419-220_web_devlog-220-2bd7b498.md) | 웹/프론트엔드 변경 이력: 디자인사이트 Staff 관리자 패널 ReferenceError 수정 |
| 2026-04-19 | [history-20260419-221](releases/2026-04-19_history-20260419-221_web_devlog-221-8f4102f6.md) | 웹/프론트엔드 변경 이력: Today 소셜/미디어 UX 다듬기 + isLiked 서버 근본 수정 |
| 2026-04-19 | [history-20260419-222](releases/2026-04-19_history-20260419-222_web_devlog-222-55b1918d.md) | 웹/프론트엔드 변경 이력: Feed Project 탭 실 DB 연동 + 포스터 fallback 컴포넌트 |
| 2026-04-19 | [history-20260419-242](releases/2026-04-19_history-20260419-242_web_devlog-242-57efafe9.md) | 웹/프론트엔드 변경 이력: ProfileSettingsPage 이미지 업로드 실 연동 + 가입일 검증 |
| 2026-04-19 | [history-20260419-227](releases/2026-04-19_history-20260419-227_web_devlog-227-d20010bf.md) | 웹/프론트엔드 변경 이력: 디자인 사이트 Likes 페이지 실 데이터 연동 (포스트/공연 탭 버그 수정) |
| 2026-04-19 | [history-20260419-225](releases/2026-04-19_history-20260419-225_web_devlog-225-085ba525.md) | 웹/프론트엔드 변경 이력: Today 소셜 반응 3종 실 DB 연동 (팔로우 + 포스트 하트 + 공연 하트 신규 엔드포인트) |
| 2026-04-19 | [history-20260419-244](releases/2026-04-19_history-20260419-244_web_devlog-244-de019b6f.md) | 웹/프론트엔드 변경 이력: Feed 포스트/모집/토론 작성 실 DB 연동 (Mock 해소) |
| 2026-04-19 | [history-20260419-245](releases/2026-04-19_history-20260419-245_web_devlog-245-c0a94833.md) | 웹/프론트엔드 변경 이력: ProfileSettingsPage 실유저 데이터 연동 재복원 |
| 2026-04-19 | [history-20260419-231](releases/2026-04-19_history-20260419-231_web_devlog-231-808c2956.md) | 웹/프론트엔드 변경 이력: 댓글 첨부 이미지/링크 렌더 복구 + iframe 임베드 (1차 배포분) |
| 2026-04-19 | [history-20260419-213](releases/2026-04-19_history-20260419-213_web_devlog-213-c4fdc6a1.md) | 웹/프론트엔드 변경 이력: scraped_artists 분리 + Discovery UI 감사 v1 + 정책 확정 (세션 인수인계) |
| 2026-04-18 | [history-20260418-247](releases/2026-04-18_history-20260418-247_web_devlog-247-ebdcbaa5.md) | 웹/프론트엔드 변경 이력: Task #9 해결: CSP 헤더 누락 원인 재진단 (Synology 무고) |
| 2026-04-18 | [v3.6.0](releases/2026-04-18_v3.6.0_web_devlog-248-ed577ba9.md) | 웹/프론트엔드 변경 이력: v3.6.0 문서 현행화 + Synology CSP SDD (#8 / #9) |
| 2026-04-18 | [history-20260418-249](releases/2026-04-18_history-20260418-249_web_devlog-249-7dedbceb.md) | 웹/프론트엔드 변경 이력: 댓글 실 DB 연동 풀 피처 + 재배포 |
| 2026-04-18 | [history-20260418-240](releases/2026-04-18_history-20260418-240_web_devlog-240-1f0d145a.md) | 웹/프론트엔드 변경 이력: Artists 페이지 Figma Make mock 제거 + 랭킹/구독 실 DB 전면 연동 |
| 2026-04-18 | [history-20260418-251](releases/2026-04-18_history-20260418-251_web_devlog-251-18eb4a5f.md) | 웹/프론트엔드 변경 이력: Feed UX 라이브 피드백 6건 수정 + 재배포 (2차) |
| 2026-04-18 | [history-20260418-252](releases/2026-04-18_history-20260418-252_web_devlog-252-29c0e51e.md) | 웹/프론트엔드 변경 이력: Feed UX 라이브 피드백 4건 수정 + 재배포 |
| 2026-04-18 | [history-20260418-253](releases/2026-04-18_history-20260418-253_web_devlog-253-a5c86c34.md) | 웹/프론트엔드 변경 이력: Feed 플랫폼 임베드 Phase 2~5 완료 + 재배포 |
| 2026-04-18 | [history-20260418-255](releases/2026-04-18_history-20260418-255_web_devlog-255-8b0c07a5.md) | 웹/프론트엔드 변경 이력: Feed rank bug 해제 (Phase 1) |
| 2026-04-18 | [history-20260418-257](releases/2026-04-18_history-20260418-257_web_devlog-257-25b559fb.md) | 웹/프론트엔드 변경 이력: NEON→웹 앱 리네이밍 완료 + auto-sync 이슈 해결 |
| 2026-04-18 | [history-20260418-258](releases/2026-04-18_history-20260418-258_web_devlog-258-452785d0.md) | 웹/프론트엔드 변경 이력: 이미지 S3 마이그레이션 + Today 페이지 개선 (낮) |
| 2026-04-18 | [history-20260418-246](releases/2026-04-18_history-20260418-246_web_devlog-246-102a3ee7.md) | 웹/프론트엔드 변경 이력: Discovery S3/CloudFront 이식 재적용 (핸드오프 복구) |
| 2026-04-15 | [history-20260415-262](releases/2026-04-15_history-20260415-262_web_devlog-262-fce7d852.md) | 웹/프론트엔드 변경 이력: 웹 앱 리디자인 백엔드 연결 |
| 2026-03-22 | [history-20260322-278](releases/2026-03-22_history-20260322-278_web_devlog-278-7f49c8ba.md) | 웹/프론트엔드 변경 이력: Figma 워크플로우 D-1~D-13 완료 |
| 2026-03-21 | [history-20260321-279](releases/2026-03-21_history-20260321-279_web_devlog-279-fb1c1fcc.md) | 웹/프론트엔드 변경 이력: 웹 앱 Stitch 워크플로우 완료 + Penpot→Stitch 전환 |
| 2026-03-19 | [v1.0.0](releases/2026-03-19_v1.0.0_web_devlog-281-d5a04d1c.md) | 웹/프론트엔드 변경 이력: CSS 토큰화 + 다크모드 + Knowledge Map v1.0.0 + Serena 제거 |
| 2026-03-15 | [v2.0](releases/2026-03-15_v2.0_web_devlog-283-df3b666c.md) | 웹/프론트엔드 변경 이력: 다중팀 v2.0 재편 + Knowledge Map 설계 |

### Backend

| Date | Version | Summary |
|---|---|---|
| 2026-05-23 | [r1.50.7](releases/2026-05-23_r1.50.7_backend_settlement-payout-reconciliation.md) | 정산 화면과 관리자 정산 흐름에서 PayPal 지급과 결제 대사 흐름을 더 정확하게 확인할 수 있도록 보강했습니다. |
| 2026-05-23 | [r1.50.7](releases/2026-05-23_r1.50.7_backend_my-settlement-aggregation.md) | 정산 화면이 최신 공연 티켓 주문 구조까지 반영해서 판매 금액을 집계하도록 보강했습니다. |
| 2026-05-22 | [r1.50.6](releases/2026-05-22_r1.50.6_backend_paypal-refund-cascade.md) | PayPal로 결제한 티켓도 환불 완료 후 안내 메일, 공연 생성자 알림, 환불 상태 표시가 Toss 결제와 같은 흐름으로 처리되도록 보강했습니다. |
| 2026-05-22 | [r1.50.5](releases/2026-05-22_r1.50.5_backend_ticket-refund-notifications-management.md) | 티켓 환불 완료 후 안내 메일과 공연 관리 화면의 환불 상태 표시가 더 정확해지도록 보강했습니다. |
| 2026-05-22 | [r1.50.5](releases/2026-05-22_r1.50.5_backend_ticket-refund-host-notifications.md) | 티켓 환불이 완료되면 공연 생성자가 알림에서 관련 티켓 관리 화면으로 이동할 수 있도록 알림 흐름을 보강했습니다. |
| 2026-05-22 | [r1.50.4](releases/2026-05-22_r1.50.4_backend_ticket-email-detail-scanner-recovery.md) | 결제 완료와 티켓 발급 메일, 나의 티켓 상세 보기, QR 확인, 티켓 스캐너 흐름을 실제 발급 티켓 기준으로 보강했습니다. |
| 2026-05-22 | [r1.50.2](releases/2026-05-22_r1.50.2_backend_ticket-visibility-recovery.md) | 실제 승인된 티켓 결제가 나의 티켓에 표시되도록 결제 확정과 티켓 조회 흐름을 보강했습니다. |
| 2026-05-22 | [r1.50.1](releases/2026-05-22_r1.50.1_backend_payment-completion.md) | 티켓 결제가 실제 승인 후 구매 완료와 티켓 발급으로 이어지도록 결제 완료 흐름을 개선했습니다. |
| 2026-05-21 | [r1.49.11](releases/2026-05-21_r1.49.11_backend_likes-auth-persistence-api.md) | 공연 좋아요 상태를 더 정확히 조회하도록 서버 응답을 보강했습니다. |
| 2026-05-21 | [r1.49.10](releases/2026-05-21_r1.49.10_backend_event-owner-api-guard.md) | 공연을 만든 계정이 자신의 공연에 티켓 구매나 게스트리스트 신청을 하지 않도록 서버 검증을 추가했습니다. |
| 2026-05-16 | [R1.38.x](releases/2026-05-16_R1.38.x_backend_devlog-018-e96d4b4c.md) | 백엔드/API 변경 이력: R1.38.x cluster cascade LIVE 영구 종료 final (R1.37.0.1.X 5개월 cascade 진짜 root cause 100% 해소 ) |
| 2026-05-16 | [R1.38.0](releases/2026-05-16_R1.38.0_backend_devlog-019-883ea31e.md) | 백엔드/API 변경 이력: R1.38.0 cluster LIVE (spec-kit 정상 도입 + dispatch_observer daemon + voice cascade screencapture + LRN-NEW-114 진짜 root cause + LRN-NEW-115 chicken-and-egg #133 후보) |
| 2026-05-16 | [R1.38.x](releases/2026-05-16_R1.38.x_backend_devlog-010-d8e232c2.md) | 백엔드/API 변경 이력: R1.38.x Phase 9 cascade chain hard termination 첫 적용 LIVE 첫 record (iter 7 MAJOR META-META IRONY + #134 Rule F 15회차 +200% surplus triple sustained record + 세션 종료 base) |
| 2026-05-16 | [R1.38.x](releases/2026-05-16_R1.38.x_backend_devlog-012-1c384d19.md) | 백엔드/API 변경 이력: R1.38.x cluster cascade close + #136 정식 승격 (audit cascade chained finding pattern + cascade chain termination LIVE 첫 입증 record) |
| 2026-05-16 | [R1.38.3.4](releases/2026-05-16_R1.38.3.4_backend_devlog-013-2a18424f.md) | 백엔드/API 변경 이력: R1.38.3.4 hotfix #135 L100 명시적 pane target + LRN-NEW-121 6 step matrix (cascade chain termination 첫 적용 LIVE 첫 record + #134 Rule F dogfooding 8회차 +60% surplus) |
| 2026-05-16 | [R1.38.3.3](releases/2026-05-16_R1.38.3.3_backend_devlog-014-201379a8.md) | 백엔드/API 변경 이력: R1.38.3.3 hotfix #135 L100 Option C + LRN-NEW-121 정식 등재 (audit cascade chained finding pattern + trade-off recursive cascade 영구 회피 SOP base + #134 Rule F dogfooding 6회차 sustained record 갱신 LIVE + #136 후보 base) |
| 2026-05-16 | [R1.38.3.2](releases/2026-05-16_R1.38.3.2_backend_devlog-015-684917f8.md) | 백엔드/API 변경 이력: R1.38.3.2 hotfix #135 L100 Option A + L123 SUMMARY 정정 (Codex P2 finding 2건 + #134 Rule F dogfooding 5회차 첫 도달 LIVE) |
| 2026-05-16 | [R1.38.3.1](releases/2026-05-16_R1.38.3.1_backend_devlog-016-95090466.md) | 백엔드/API 변경 이력: R1.38.3.1 hotfix #135 effective scope 11 한정 정정 (Codex P2 finding) |
| 2026-05-12 | [R1.19.10](releases/2026-05-12_R1.19.10_backend_devlog-028-f546e466.md) | 백엔드/API 변경 이력: R1.19.10 Security Hotfix LIVE PASS (#NEW-α IPv6 keyGenerator + #NEW-β Toss log masking) + LRN-NEW-51 SOP 2회차 정합 입증 |
| 2026-05-11 | [R1.19.5](releases/2026-05-11_R1.19.5_backend_devlog-034-4e2a6e64.md) | 백엔드/API 변경 이력: R1.19.5 Phase 2 sprint 영구 종료 + #90 9 Rule LIVE 입증 + 권커맨더 자율 commit + HOF-023 발행 |
| 2026-05-11 | [R1.19.x](releases/2026-05-11_R1.19.x_backend_devlog-038-f9cfc6fd.md) | 백엔드/API 변경 이력: R1.19.x sprint 통합 종료 + 자율 자동화 100% 영구 입증 + R1.18 fast-follow #NEW-1 진정 종료 (HOF-018 발행) |
| 2026-05-09 | [R1.12.13](releases/2026-05-09_R1.12.13_backend_devlog-049-6b48f25f.md) | 백엔드/API 변경 이력: R1.12.13 sprint 종료 (cleanup endpoint 완전 제거, security 우선) |
| 2026-05-08 | [R1.6](releases/2026-05-08_R1.6_backend_devlog-060-356cf36b.md) | 백엔드/API 변경 이력: R1.6~R1.11 8 sprint 누적 핸드오프 발행 (HOF-008, 사용자 명시 의뢰) |
| 2026-05-04 | [history-20260504-097](releases/2026-05-04_history-20260504-097_backend_devlog-097-c691a096.md) | 백엔드/API 변경 이력: GuestList 라운드 5: 호스트 invalidate 누락 + status 메시지 단순화 |
| 2026-05-04 | [history-20260504-098](releases/2026-05-04_history-20260504-098_backend_devlog-098-c01a63fc.md) | 백엔드/API 변경 이력: Warroom UI 헬스체크 false-down 해소 (URL → Tailscale) |
| 2026-04-30 | [history-20260430-099](releases/2026-04-30_history-20260430-099_backend_devlog-099-02da76ee.md) | 백엔드/API 변경 이력: health-check 이메일 발송 빈도 완화 (cooldown 1h→6h, 정기 4h→8h) |
| 2026-04-28 | [history-20260428-111](releases/2026-04-28_history-20260428-111_backend_devlog-111-bbbe3b14.md) | 백엔드/API 변경 이력: Threads 자동포스팅용 내부 항목 셋업 + NAS 노출 하드닝 |
| 2026-04-28 | [history-20260428-119](releases/2026-04-28_history-20260428-119_backend_devlog-119-b28c3d03.md) | 백엔드/API 변경 이력: PostCreate mention chip 카드 X 본문 동기화 + caret 정렬 (commit 27) |
| 2026-04-26 | [history-20260426-152](releases/2026-04-26_history-20260426-152_backend_devlog-152-bf2c93a6.md) | 백엔드/API 변경 이력: 헬스체크 GitHub CLI ❌ 근본 수정 (revoke된 옛 인증값 동기화) |
| 2026-04-26 | [history-20260426-154](releases/2026-04-26_history-20260426-154_backend_devlog-154-46b369f5.md) | 백엔드/API 변경 이력: sync 카운트 정확화 (synced_events vs skipped_events 분리) |
| 2026-04-26 | [history-20260426-165](releases/2026-04-26_history-20260426-165_backend_devlog-165-e385dcc3.md) | 백엔드/API 변경 이력: chat 디버그 로그 cleanup + push subscription stale 검증 |
| 2026-04-21 | [history-20260421-201](releases/2026-04-21_history-20260421-201_backend_devlog-201-a63b6acc.md) | 백엔드/API 변경 이력: 관리자 패널 Email 탭 Phase 1 (+T1/T2/T4/E1 선행 보강) |
| 2026-04-18 | [history-20260418-256](releases/2026-04-18_history-20260418-256_backend_devlog-256-135faed8.md) | 백엔드/API 변경 이력: 단일 Dev Log 도입 (CLAUDE_DEV_LOG.md) |
| 2026-04-15 | [history-20260415-261](releases/2026-04-15_history-20260415-261_backend_devlog-261-57785ae5.md) | 백엔드/API 변경 이력: 웹 앱 AWS 마이그레이션 최종 완료 |
| 2026-04-10 | [history-20260410-266](releases/2026-04-10_history-20260410-266_backend_devlog-266-a181c518.md) | 백엔드/API 변경 이력: 인프라 일일 보고서 + Tailscale IP 변경 |
| 2026-04-09 | [history-20260409-267](releases/2026-04-09_history-20260409-267_backend_devlog-267-93e08ff1.md) | 백엔드/API 변경 이력: Warroom 캘린더 복구 |
| 2026-04-04 | [history-20260404-271](releases/2026-04-04_history-20260404-271_backend_devlog-271-c4cfa7c8.md) | 백엔드/API 변경 이력: 헬스체크 + PostgreSQL 복구 + 커맨더 설정 |
| 2026-03-29 | [history-20260329-274](releases/2026-03-29_history-20260329-274_backend_devlog-274-659654de.md) | 백엔드/API 변경 이력: Harness 대시보드 구축 |
| 2026-03-28 | [history-20260328-275](releases/2026-03-28_history-20260328-275_backend_devlog-275-6b471951.md) | 백엔드/API 변경 이력: 미완료 작업 완료 + gitsafe-backup 복구 |
| 2026-03-26 | [history-20260326-276](releases/2026-03-26_history-20260326-276_backend_devlog-276-c0889bd9.md) | 백엔드/API 변경 이력: 서버 재구성 Phase 1-5 완료 |
| 2026-03-18 | [history-20260318-282](releases/2026-03-18_history-20260318-282_backend_devlog-282-ce683bfd.md) | 백엔드/API 변경 이력: 에이전트 이름 변경 + Claude Code 로그아웃 해결 |

### Data Pipeline

| Date | Version | Summary |
|---|---|---|
| 2026-05-16 | [R1.38.x](releases/2026-05-16_R1.38.x_data-pipeline_devlog-011-fb51290a.md) | 데이터 파이프라인 변경 이력: R1.38.x Phase 8 #136 Option A rollback (MAJOR IRONY = #136 SOP 자체 측 cascade chain 재개 LIVE 첫 입증, meta-level cascade recursion) |
| 2026-04-28 | [history-20260428-116](releases/2026-04-28_history-20260428-116_data-pipeline_devlog-116-25885a4a.md) | 데이터 파이프라인 변경 이력: PostCreate toolbar 위치 / paddingBottom dynamic / KeyboardSheet bottomOffset (commit 30) |
| 2026-04-13 | [history-20260413-264](releases/2026-04-13_history-20260413-264_data-pipeline_devlog-264-351991f6.md) | 데이터 파이프라인 변경 이력: Warroom 안정화 |
| 2026-04-11 | [history-20260411-265](releases/2026-04-11_history-20260411-265_data-pipeline_devlog-265-135b1e8d.md) | 데이터 파이프라인 변경 이력: NAS 알림 + 헬스체크 + 대시보드 수정 |

### Infra

| Date | Version | Summary |
|---|---|---|
| 2026-04-28 | [history-20260428-117](releases/2026-04-28_history-20260428-117_infra_devlog-117-7adc47e0.md) | 인프라/배포 변경 이력: PostCreate toolbar 키보드 위 fixed + mention sheet 빈 결과 (commit 29) |
| 2026-04-27 | [history-20260427-129](releases/2026-04-27_history-20260427-129_infra_devlog-129-828e3b01.md) | 인프라/배포 변경 이력: PostCreate TDZ 'ze' fix (useDropdownScroll active 인자) |
| 2026-04-27 | [history-20260427-130](releases/2026-04-27_history-20260427-130_infra_devlog-130-45ff19d7.md) | 인프라/배포 변경 이력: PostCreate scroll rAF + useEffect 분리 + max-h + cursor gap (round 10) |
| 2026-04-27 | [history-20260427-133](releases/2026-04-27_history-20260427-133_infra_devlog-133-76dc523b.md) | 인프라/배포 변경 이력: PostCreate dropdown anchor textareaRef + 외부 click 감지 |
| 2026-04-27 | [history-20260427-134](releases/2026-04-27_history-20260427-134_infra_devlog-134-282873b9.md) | 인프라/배포 변경 이력: PostCreate portal dropdown 위치 rAF loop 추적 |
| 2026-04-27 | [history-20260427-137](releases/2026-04-27_history-20260427-137_infra_devlog-137-5bfe7b17.md) | 인프라/배포 변경 이력: PostCreate dropdown scroll 진짜 근본 해결 (textarea blur 자동 닫기 제거 + 외부 클릭 감지) |
| 2026-04-27 | [history-20260427-138](releases/2026-04-27_history-20260427-138_infra_devlog-138-6559320e.md) | 인프라/배포 변경 이력: PostCreate dropdown 에 data-vaul-no-drag (native scroll 회복) |
| 2026-04-23 | [history-20260423-176](releases/2026-04-23_history-20260423-176_infra_devlog-176-ddc2b7a4.md) | 인프라/배포 변경 이력: POMFS 공식 홈페이지 v2 Phase 3 QA (2차) — 폼 UI + 메일 디자인 5건 추가 수정 |
| 2026-04-18 | [history-20260418-232](releases/2026-04-18_history-20260418-232_infra_devlog-232-34c04572.md) | 인프라/배포 변경 이력: 구독 중 버튼 색 일관성 이터레이션 (3 커밋) |
| 2026-04-08 | [history-20260408-268](releases/2026-04-08_history-20260408-268_infra_devlog-268-aa5578d0.md) | 인프라/배포 변경 이력: Discord 취소 기능 구현 |
| 2026-04-01 | [history-20260401-272](releases/2026-04-01_history-20260401-272_infra_devlog-272-8d2cc200.md) | 인프라/배포 변경 이력: Phase 3 구현 + 대시보드 시각화 |
| 2026-03-25 | [history-20260325-277](releases/2026-03-25_history-20260325-277_infra_devlog-277-7598d21a.md) | 인프라/배포 변경 이력: Tailscale IP 마이그레이션 |

### Operations

| Date | Version | Summary |
|---|---|---|
| 2026-05-22 | [release-history-v3](releases/2026-05-22_release-history-v3_operations_release-history-claude-code-token-snapshots.md) | Public release notes에서 Claude Code 누적 토큰 사용량도 함께 확인할 수 있도록 자동화를 보강했습니다. |
| 2026-05-22 | [release-history-v2](releases/2026-05-22_release-history-v2_operations_release-history-codex-token-snapshots.md) | Public release notes와 iOS README가 같은 Codex 누적 토큰 스냅샷을 표시하도록 release history 자동화를 보강했습니다. |
| 2026-05-21 | [release-history-v1](releases/2026-05-21_release-history-v1_operations_release-history-scaffold.md) | POMFS 변경 이력을 구조적으로 기록하고 검증하는 release history 체계를 추가했습니다. |
| 2026-05-17 | [r1.43](releases/2026-05-17_r1.43_operations_session-handoff-automation.md) | 내부 릴리스 및 세션 handoff 자동화를 개선했습니다. |
| 2026-05-12 | [R1.19.5](releases/2026-05-12_R1.19.5_operations_devlog-032-f0b121f9.md) | 운영 자동화 변경 이력: R1.19.5 fast-follow: handoff-respawn-commander.sh set -u P2 fix + 신규 추적 + audit 100% PASS + #91 LIVE 8번째 누적 |
| 2026-05-09 | [R1.12.11](releases/2026-05-09_R1.12.11_operations_devlog-052-ba3969a2.md) | 운영 자동화 변경 이력: R1.12.11 + R1.12.12 + R1.13.1 사이클 핸드오프 발행 (HOF-011, 사용자 명시 의뢰) |
| 2026-05-08 | [R1.12.9](releases/2026-05-08_R1.12.9_operations_devlog-055-e14049ed.md) | 운영 자동화 변경 이력: R1.12.9 + R1.12.10 사이클 핸드오프 발행 (HOF-010, 사용자 명시 의뢰) |
| 2026-04-29 | [history-20260429-102](releases/2026-04-29_history-20260429-102_operations_devlog-102-a1128a50.md) | 운영 자동화 변경 이력: Shows 지도 내 위치 마커 녹색→보라(#8B29D8) |
| 2026-04-27 | [history-20260427-125](releases/2026-04-27_history-20260427-125_operations_devlog-125-2678f387.md) | 운영 자동화 변경 이력: PostCreate floating-ui strategy:'fixed' |
| 2026-04-14 | [history-20260414-263](releases/2026-04-14_history-20260414-263_operations_devlog-263-8393be50.md) | 운영 자동화 변경 이력: 워치독 스팸 + 대시보드 복구 + 권커맨더 라우팅 |
| 2026-04-07 | [history-20260407-269](releases/2026-04-07_history-20260407-269_operations_devlog-269-d6748d57.md) | 운영 자동화 변경 이력: Discord 미션컨트롤 v2 구현 |
| 2026-04-06 | [history-20260406-270](releases/2026-04-06_history-20260406-270_operations_devlog-270-eab088ba.md) | 운영 자동화 변경 이력: Mac Mini B Figma + Phase 4 전체 구현 |
| 2026-03-31 | [history-20260331-273](releases/2026-03-31_history-20260331-273_operations_devlog-273-457238d6.md) | 운영 자동화 변경 이력: Meta Orchestrator Phase 2 구현 완료 |

## Browse / Filters

- All releases
- iOS
- Web
- Backend
- Data Pipeline
- Infra
- Operations
- Monthly archive
