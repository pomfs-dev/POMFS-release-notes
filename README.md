# POMFS Release History

이 저장소는 POMFS의 공개 릴리즈 히스토리입니다.

각 항목은 private source repo의 release metadata에서 생성되며, 공개 가능한 요약만 포함합니다. iOS, Web, Backend, Data Pipeline, Infra, Operations 변경을 시간순으로 모아 보여줍니다.

공개 노트에는 source code, 내부 경로, 개인 이메일, private infrastructure detail, token/key, raw commit hash, sensitive security detail을 포함하지 않습니다.

상세 항목에는 Summary, Changes, Known Issues가 있으며, 시간이 확인된 항목은 `Released at`을 함께 표시합니다.

## About P.O.MFS Dev Team

P.O.MFS Dev Team은 P.O.MFS와 MiSFY 생태계를 설계하고 운영하는 제품·엔지니어링 팀입니다. 커뮤니티 앱, 백엔드/API, 데이터 파이프라인, 운영 자동화, AI 기반 개발 워크플로우, 오픈소스 도구를 함께 만들며 실제 서비스 운영에서 검증된 개선 사항을 공개 가능한 형태로 정리합니다.

이 공개 릴리즈 히스토리는 P.O.MFS Dev Team의 David Kwon이 만들고 관리합니다. P.O.MFS 공식 홈페이지는 [prideofmisfits.com](https://www.prideofmisfits.com)입니다.

릴리즈 노트 정리와 공개 문서 유지보수에는 Codex와 Claude Code 기반 AI-assisted workflow도 함께 사용합니다.

## AI Lifetime Token Usage

Codex와 Claude Code의 전체 누적 토큰량을 함께 보여줍니다. 각 값은 public release notes가 갱신될 때 기록되는 정적 스냅샷입니다.

### Codex

Codex 전체 누적 토큰량입니다. 이 값은 실시간 대시보드가 아니라 public release notes가 갱신될 때 함께 기록되는 정적 스냅샷입니다.

<table>
  <tr>
    <th align="left">Snapshot</th>
    <td>2026-06-15 18:37 KST</td>
  </tr>
  <tr>
    <th align="left">Scope</th>
    <td>Codex session logs</td>
  </tr>
  <tr>
    <th align="left">Sessions</th>
    <td>374 sessions</td>
  </tr>
  <tr>
    <th align="left">Cumulative total</th>
    <td><strong>5,730,319,138 tokens</strong></td>
  </tr>
  <tr>
    <th align="left">Input</th>
    <td>5,708,330,652 tokens</td>
  </tr>
  <tr>
    <th align="left">Cached input</th>
    <td>5,418,128,000 tokens</td>
  </tr>
  <tr>
    <th align="left">Output</th>
    <td>21,988,486 tokens</td>
  </tr>
  <tr>
    <th align="left">Reasoning output</th>
    <td>7,140,330 tokens</td>
  </tr>
</table>

<table>
  <tr>
    <th align="left">Scale</th>
    <th align="left">Usage Graph</th>
    <th align="right">Percent</th>
  </tr>
  <tr>
    <td>5,800,000,000 tokens</td>
    <td><code>████████████████████</code></td>
    <td align="right">98.8%</td>
  </tr>
</table>

### Claude Code

Claude Code 전체 누적 토큰량입니다. 이 값은 tui-monitor 집계기가 Claude Code session logs를 다시 계산해 기록한 정적 스냅샷입니다.

<table>
  <tr>
    <th align="left">Snapshot</th>
    <td>2026-06-15 18:37 KST</td>
  </tr>
  <tr>
    <th align="left">Scope</th>
    <td>Claude Code session logs</td>
  </tr>
  <tr>
    <th align="left">Session files</th>
    <td>1,294 files</td>
  </tr>
  <tr>
    <th align="left">Assistant entries</th>
    <td>79,595 entries</td>
  </tr>
  <tr>
    <th align="left">Cumulative total</th>
    <td><strong>22,619,367,937 tokens</strong></td>
  </tr>
  <tr>
    <th align="left">Input</th>
    <td>152,464,556 tokens</td>
  </tr>
  <tr>
    <th align="left">Cache creation</th>
    <td>1,346,153,706 tokens</td>
  </tr>
  <tr>
    <th align="left">Cache read</th>
    <td>20,946,836,379 tokens</td>
  </tr>
  <tr>
    <th align="left">Output</th>
    <td>173,913,296 tokens</td>
  </tr>
  <tr>
    <th align="left">Weekly 7d</th>
    <td>1,668,699,540 tokens</td>
  </tr>
  <tr>
    <th align="left">Monthly 30d</th>
    <td>22,420,683,594 tokens</td>
  </tr>
  <tr>
    <th align="left">Daily avg</th>
    <td>869,975,689 tokens/day</td>
  </tr>
</table>

<table>
  <tr>
    <th align="left">Scale</th>
    <th align="left">Usage Graph</th>
    <th align="right">Percent</th>
  </tr>
  <tr>
    <td>22,700,000,000 tokens</td>
    <td><code>████████████████████</code></td>
    <td align="right">99.6%</td>
  </tr>
</table>

## Latest

| Date | Version | Component | Summary |
|---|---|---|---|
| 2026-06-15 | [r1.53.6](releases/2026-06-15_r1.53.6_backend_admin-member-delete-fix.md) | Backend | 관리자 회원 관리에서 일부 회원을 삭제할 때 오류가 나던 문제를 해결해, 회원 삭제가 정상적으로 완료되도록 했습니다. |
| 2026-06-13 | [r1.53.5](releases/2026-06-13_r1.53.5_web_shared-event-link-blank-screen.md) | Web | 외부로 공유한 공연 링크를 열면 화면이 비어 보이던 문제를 해결했습니다. |
| 2026-06-12 | [r1.53.4](releases/2026-06-12_r1.53.4_operations_artist-hide-public-surface.md) | Operations | 관리 도구에서 아티스트를 숨김 처리하면 공개 화면에 곧바로 반영되도록 개선했습니다. |
| 2026-06-12 | [r1.53.3](releases/2026-06-12_r1.53.3_data-pipeline_today-card-images.md) | Data Pipeline | Today 화면의 추천 공연 카드에서 일부 이미지가 보이지 않던 문제를 해결해, 공연 이미지가 정상적으로 표시되도록 했습니다. |
| 2026-06-12 | [release-assistant-v0.1](releases/2026-06-12_release-assistant-v0.1_operations_ios-release-assistant-open-source.md) | Operations | iOS 앱 출시 준비를 단계별로 도와주는 iOS Release Assistant를 오픈소스 도구로 정리하고, 초보자도 따라갈 수 있도록 문서를 보강했습니다. |
| 2026-06-12 | [3.0.0](releases/2026-06-12_3.0.0_ios_app-store-review-submission.md) | iOS | MiSFY iOS 3.0.0 빌드를 App Store 심사에 제출하고, App Store Connect에서 심사 대기 상태까지 확인했습니다. |
| 2026-06-09 | [release-history-v4](releases/2026-06-09_release-history-v4_operations_public-release-history-sanitized-refresh.md) | Operations | 공개 릴리즈 히스토리를 정제해 내부 개발 로그성 항목을 제거하고, 실제 사용자에게 설명할 수 있는 변경 이력 중심으로 다시 정리했습니다. |
| 2026-06-09 | [r1.53.2](releases/2026-06-09_r1.53.2_operations_report-notification-routing.md) | Operations | POMFS 운영 보고와 자동 알림 메일의 기본 수신 경로를 정리해, 중요한 운영 알림이 한 곳으로 모이도록 개선했습니다. |
| 2026-06-09 | [r1.53.1](releases/2026-06-09_r1.53.1_web_feed-genre-badges.md) | Web | Feed 카드에서 일반 AI 표시 대신 공연과 콘텐츠의 장르를 더 분명하게 볼 수 있도록 장르 뱃지를 표시했습니다. |
| 2026-06-08 | [r1.53.0](releases/2026-06-08_r1.53.0_web_today-nearby-new-shows.md) | Web | Today 화면의 "새로운 공연"을 내 주변과 가까운 날짜를 기준으로 똑똑하게 추천하도록 개선했습니다. |
| 2026-06-07 | [r1.52.13](releases/2026-06-07_r1.52.13_web_curation-post-comments.md) | Web | 피드의 큐레이션 글에도 댓글로 의견을 나눌 수 있도록 댓글 기능을 추가했습니다. |
| 2026-06-07 | [r1.52.12](releases/2026-06-07_r1.52.12_data-pipeline_map-data-quality.md) | Data Pipeline | 공연 지도에 잘못 수집되거나 잘못된 위치에 표시되던 항목을 정리하고, 앞으로 더 정확한 공연 정보만 노출되도록 데이터 품질을 개선했습니다. |
| 2026-06-07 | [r1.52.11](releases/2026-06-07_r1.52.11_operations_app-homepage-stats-alignment.md) | Operations | 앱과 공식 홈페이지에 표시되는 공연장·아티스트·국가 수치가 항상 동일한 기준의 최신 값으로 함께 정렬되도록 정비했습니다. |
| 2026-06-06 | [r1.52.7](releases/2026-06-06_r1.52.7_web_venue-detail-upcoming-cards-fix.md) | Web | 공연 지도에서 공연장 상세로 들어갔을 때 예정 공연 카드가 비어 보이던 문제를 수정해, 예정 공연 정보가 정상적으로 표시됩니다. |
| 2026-06-06 | [r1.52.10](releases/2026-06-06_r1.52.10_data-pipeline_ai-event-geocode-enrichment.md) | Data Pipeline | AI로 수집된 공연이 지도에 올바른 위치로 표시되도록 위치 정보를 보강하고, 매일 진행되는 데이터 정리 과정을 더 빠르고 안정적으로 개선했습니다. |
| 2026-06-06 | [r1.52.8](releases/2026-06-06_r1.52.8_web_shows-list-viewport-scope.md) | Web | 공연 지도의 리스트 보기가 항상 현재 보이는 지도 화면 범위의 공연만 보여주도록 개선했습니다. |
| 2026-06-06 | [r1.52.9](releases/2026-06-06_r1.52.9_operations_event-auto-publish.md) | Operations | 매일 자동으로 수집된 공연 중 발행 기준을 충족하는 공연이 자동으로 앱에 올라가도록 개선했습니다. |
| 2026-06-06 | [r1.52.6](releases/2026-06-06_r1.52.6_backend_artist-follow-foundation.md) | Backend | 더 다양한 아티스트를 팔로우할 수 있는 기반을 마련하고, 일부 프로필에서 참석한 공연 목록이 보이지 않던 문제를 해결했습니다. |
| 2026-06-05 | [r1.52.4](releases/2026-06-05_r1.52.4_backend_public-pii-hardening-rollout.md) | Backend | 공개 화면에 제공되는 정보가 꼭 필요한 항목만 포함되도록 개인정보 보호를 한층 더 확대했습니다. |
| 2026-06-05 | [r1.52.5](releases/2026-06-05_r1.52.5_operations_release-deploy-automation.md) | Operations | 앱 업데이트가 더 빠르고 안정적으로 반영되도록 배포 과정을 정비했으며, 사용자가 체감하는 기능 변화는 없습니다. |
| 2026-06-05 | [r1.52.3](releases/2026-06-05_r1.52.3_web_event-map-image-display.md) | Web | 공연 지도의 리스트 보기에서 일부 공연 항목의 이미지가 깨져 보이던 문제를 개선해, 깔끔한 이미지로 표시되도록 했습니다. |
| 2026-06-05 | [r1.52.2](releases/2026-06-05_r1.52.2_backend_signup-email-duplicate-prevention.md) | Backend | 같은 이메일 주소로 서로 다른 로그인 방식을 쓰면 별개의 계정이 따로 만들어지던 문제를 개선해, 한 사람이 하나의 계정으로 일관되게 이용할 수 있도록 회원가입·로그인 처리를 강화했습니다. |
| 2026-06-05 | [r1.52.1](releases/2026-06-05_r1.52.1_backend_privacy-hardening.md) | Backend | 공개 화면에 제공되는 정보가 꼭 필요한 항목만 포함되도록 개인정보 보호를 강화했습니다. |
| 2026-06-05 | [r1.51.1](releases/2026-06-05_r1.51.1_web_shows-venue-detail-crash-fix.md) | Web | 공연 지도에서 공연장 상세 화면에 들어갈 때 모든 공연장에서 오류 페이지가 뜨던 문제를 해결했습니다. |
| 2026-06-05 | [r1.52.0](releases/2026-06-05_r1.52.0_operations_discovery-collection-publish-pipeline.md) | Operations | 공연·공연장 정보가 매일 자동으로 수집·정리되어 더 많은 공연장과 한국 공연이 앱에 노출됩니다. |
| 2026-06-05 | [r1.51.9](releases/2026-06-05_r1.51.9_backend_curation-feed-auto-publish.md) | Backend | 월간 큐레이션 일정의 공연 영상이 앱 피드에 자동으로 올라오는 과정을 정비해 더 자연스럽고 정확하게 발행됩니다. |
| 2026-06-05 | [r1.51.4](releases/2026-06-05_r1.51.4_web_legal-docs-bizinfo-toggle.md) | Web | 개인정보처리방침과 이용약관을 관련 법 기준에 맞게 보강하고, 법률 페이지에서 한국어와 영어를 바로 전환해 볼 수 있게 했습니다. |
| 2026-06-04 | [r1.51.2](releases/2026-06-04_r1.51.2_web_shows-list-4category-order.md) | Web | 공연 지도의 리스트 보기에서 공연이 더 직관적인 순서로 정렬되도록 개선했습니다. |
| 2026-06-04 | [r1.51.3](releases/2026-06-04_r1.51.3_web_refund-policy-consistency.md) | Web | 공연별 환불 정책이 구매 화면, 환불 화면, 실제 환불 처리에 일관되게 표시·적용되도록 정리했습니다. |
| 2026-06-04 | [r1.51.5](releases/2026-06-04_r1.51.5_web_artist-share-drop-card.md) | Web | 아티스트 프로필 공유 링크가 예시 데이터 대신 실제 정보가 담긴 "드롭 명함" 화면으로 곧바로 연결됩니다. |
| 2026-06-04 | [r1.51.7](releases/2026-06-04_r1.51.7_web_onboarding-nickname-duplicate-check.md) | Web | 가입 온보딩에서 이미 사용 중인 닉네임을 고르면 곧바로 알려주고 막아줍니다. |
| 2026-06-04 | [r1.51.8](releases/2026-06-04_r1.51.8_web_paypal-unsupported-notice.md) | Web | PayPal 미지원 국가에서의 안내 문구를 명확히 다듬고, 결제 후 주최자 알림과 환불 흐름을 함께 개선했습니다. |
| 2026-06-04 | [r1.51.6](releases/2026-06-04_r1.51.6_web_share-deeplink.md) | Web | 공유한 아티스트·공연장·게시물 링크가 앱의 알맞은 화면으로 더 정확하게 열립니다. |
| 2026-06-04 | [r1.51.10](releases/2026-06-04_r1.51.10_ios_onboarding-complete-fix.md) | iOS | 신규 가입 마지막 "시작하기" 단계에서 일부 사용자가 튕기던 문제를 찾아 수정했습니다. |
| 2026-06-03 | [r1.50.20](releases/2026-06-03_r1.50.20_web_sidebar-profile-sheet.md) | Web | 햄버거 메뉴 안의 프로필 사진을 눌러도 반응하지 않던 문제를 수정했습니다. |
| 2026-06-03 | [r1.50.19](releases/2026-06-03_r1.50.19_web_search-event-result-navigation.md) | Web | 검색 결과에서 이벤트를 선택해도 상세 화면으로 이동하지 않던 문제를 수정했습니다. |
| 2026-06-02 | [r1.51.0](releases/2026-06-02_r1.51.0_web_global-chat-full-go.md) | Web | MiSFY 커뮤니티에서 메시지와 이벤트 채팅을 더 안정적으로 사용할 수 있도록 글로벌 채팅 기반을 정식 적용했습니다. |
| 2026-06-01 | [r1.50.22](releases/2026-06-01_r1.50.22_backend_admin-member-delete-transactional-cleanup.md) | Backend | 관리자 패널에서 회원 삭제가 더 안정적으로 완료되도록 서버 삭제 흐름을 보강했습니다. |
| 2026-06-01 | [r1.50.21](releases/2026-06-01_r1.50.21_backend_misfy-email-template-delivery.md) | Backend | 회원가입, 인증, 비밀번호, 티켓, 문의 관련 메일을 MiSFY 브랜드 디자인 템플릿으로 보낼 수 있도록 메일 발송 구조를 정리했습니다. |
| 2026-06-01 | [r1.50.18](releases/2026-06-01_r1.50.18_web_today-sub-banners.md) | Web | Today 화면 상단 서브배너를 About Us, YouTube, Instagram 중심으로 정리하고, About Us 외부 링크와 YouTube 카드 테두리 가시성을 개선했습니다. |
| 2026-05-31 | [r1.50.20](releases/2026-05-31_r1.50.20_operations_multilingual-rollup.md) | Operations | POMFS의 다국어 작업 범위를 한 번에 정리했습니다. 커뮤니티 웹 active route, 알림/푸시, 기기 언어 자동 선택, iOS 언어 전달, 메일 템플릿까지 ko/en/ja/es/th 기준으로 일관된 언어 경험을 제공하도록 정리했습니다. |
| 2026-05-31 | [r1.50.19](releases/2026-05-31_r1.50.19_backend_notification-language-i18n.md) | Backend | 알림 목록과 푸시 알림이 사용자의 선택 언어 또는 기기 언어를 더 잘 따르도록 다국어 처리를 보강했습니다. |
| 2026-05-31 | [r1.50.17](releases/2026-05-31_r1.50.17_web_web-i18n-admin-checkpoint.md) | Web | 커뮤니티 웹 active route의 ko/en/ja/es/th 선택 UI 언어 전환 범위를 정리하고, 각 route family의 smoke 검증과 운영 배포를 완료했습니다. |
| 2026-05-28 | [r1.50.16](releases/2026-05-28_r1.50.16_web_paypal-checkout-redirect-recovery.md) | Web | 티켓 구매에서 PayPal 결제 승인 화면으로 이동하는 방식을 조정해 결제 테스트 중 PayPal 오류 페이지가 열리던 문제를 완화했습니다. |
| 2026-05-28 | [r1.50.15](releases/2026-05-28_r1.50.15_web_profile-payout-account-delete-fix.md) | Web | 프로필 설정의 정산 계좌 등록 이동과 계정 삭제 확인 흐름을 복구했습니다. |
| 2026-05-28 | [r1.50.14](releases/2026-05-28_r1.50.14_web_paypal-oauth-onboarding-payouts.md) | Web | 아티스트와 베뉴 회원가입 온보딩에서 국가에 따라 국내 계좌와 PayPal 정산 계정 연동을 안내하도록 확장했습니다. |
| 2026-05-28 | [r1.50.9](releases/2026-05-28_r1.50.9_web_paypal-live-settlement-fee-config.md) | Web | PayPal 결제 선택 흐름을 다시 활성화하고, 관리자 Payments 화면에서 정산 수수료를 직접 조정할 수 있게 했습니다. |
| 2026-05-28 | [r1.50.13](releases/2026-05-28_r1.50.13_backend_email-auth-session-member-delete-recovery.md) | Backend | 이메일 인증 완료 후 로그인 상태 유지와 관리자 회원 삭제 흐름을 서버에서 보강했습니다. |
| 2026-05-28 | [r1.50.12](releases/2026-05-28_r1.50.12_web_email-code-session-recovery.md) | Web | 이메일 인증번호 입력 후 인증 완료 상태가 바로 유지되도록 웹 인증 흐름을 보강했습니다. |
| 2026-05-28 | [r1.50.11](releases/2026-05-28_r1.50.11_web_share-actions-deeplink-recovery.md) | Web | 공유하기 버튼과 공연 상세 링크가 더 안정적으로 동작하도록 개선했습니다. |
| 2026-05-28 | [r1.50.10](releases/2026-05-28_r1.50.10_web_legacy-password-login-recovery.md) | Web | 기존 이메일 계정의 로그인 입력 검증과 비밀번호 재설정 진입 흐름을 보강했습니다. |
| 2026-05-25 | [r1.50.8](releases/2026-05-25_r1.50.8_backend_ticket-payment-email-delivery.md) | Backend | 티켓 결제 후 완료 화면으로 이어지는 흐름과 결제/환불 메일 발송 흐름을 안정화했습니다. |
| 2026-05-25 | [r1.50.8](releases/2026-05-25_r1.50.8_ios_ios-payment-return-flow.md) | iOS | iOS 앱에서 Npay와 Toss 결제 후 POMFS 화면으로 돌아오는 흐름을 보강했습니다. |
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
| 2026-05-17 | [r1.43](releases/2026-05-17_r1.43_operations_session-handoff-automation.md) | Operations | 내부 릴리스 및 세션 handoff 자동화를 개선했습니다. |

## By Component

### iOS

| Date | Version | Summary |
|---|---|---|
| 2026-06-12 | [3.0.0](releases/2026-06-12_3.0.0_ios_app-store-review-submission.md) | MiSFY iOS 3.0.0 빌드를 App Store 심사에 제출하고, App Store Connect에서 심사 대기 상태까지 확인했습니다. |
| 2026-06-04 | [r1.51.10](releases/2026-06-04_r1.51.10_ios_onboarding-complete-fix.md) | 신규 가입 마지막 "시작하기" 단계에서 일부 사용자가 튕기던 문제를 찾아 수정했습니다. |
| 2026-05-25 | [r1.50.8](releases/2026-05-25_r1.50.8_ios_ios-payment-return-flow.md) | iOS 앱에서 Npay와 Toss 결제 후 POMFS 화면으로 돌아오는 흐름을 보강했습니다. |
| 2026-05-22 | [r1.50.5](releases/2026-05-22_r1.50.5_ios_ios-ticket-deeplink-scheme.md) | iOS 앱에서 티켓 메일의 앱 열기 버튼이 티켓 화면으로 이어질 수 있도록 딥링크 처리를 보강했습니다. |
| 2026-05-22 | [r1.50.3](releases/2026-05-22_r1.50.3_ios_ios-scoped-location-webview.md) | iOS 앱에서 위치 기능이 필요한 화면에서만 동작하도록 허용 범위를 조정했습니다. |
| 2026-05-22 | [r1.50.4](releases/2026-05-22_r1.50.4_ios_ios-codex-token-usage-snapshot.md) | iOS 앱 README에서 Codex 누적 토큰 사용량을 확인할 수 있도록 공개 스냅샷을 추가했습니다. |
| 2026-05-22 | [r1.50.1](releases/2026-05-22_r1.50.1_ios_ios-payment-webview.md) | iOS 앱에서 결제 앱으로 이동하고 다시 돌아오는 흐름을 개선했습니다. |

### Web

| Date | Version | Summary |
|---|---|---|
| 2026-06-13 | [r1.53.5](releases/2026-06-13_r1.53.5_web_shared-event-link-blank-screen.md) | 외부로 공유한 공연 링크를 열면 화면이 비어 보이던 문제를 해결했습니다. |
| 2026-06-09 | [r1.53.1](releases/2026-06-09_r1.53.1_web_feed-genre-badges.md) | Feed 카드에서 일반 AI 표시 대신 공연과 콘텐츠의 장르를 더 분명하게 볼 수 있도록 장르 뱃지를 표시했습니다. |
| 2026-06-08 | [r1.53.0](releases/2026-06-08_r1.53.0_web_today-nearby-new-shows.md) | Today 화면의 "새로운 공연"을 내 주변과 가까운 날짜를 기준으로 똑똑하게 추천하도록 개선했습니다. |
| 2026-06-07 | [r1.52.13](releases/2026-06-07_r1.52.13_web_curation-post-comments.md) | 피드의 큐레이션 글에도 댓글로 의견을 나눌 수 있도록 댓글 기능을 추가했습니다. |
| 2026-06-06 | [r1.52.7](releases/2026-06-06_r1.52.7_web_venue-detail-upcoming-cards-fix.md) | 공연 지도에서 공연장 상세로 들어갔을 때 예정 공연 카드가 비어 보이던 문제를 수정해, 예정 공연 정보가 정상적으로 표시됩니다. |
| 2026-06-06 | [r1.52.8](releases/2026-06-06_r1.52.8_web_shows-list-viewport-scope.md) | 공연 지도의 리스트 보기가 항상 현재 보이는 지도 화면 범위의 공연만 보여주도록 개선했습니다. |
| 2026-06-05 | [r1.52.3](releases/2026-06-05_r1.52.3_web_event-map-image-display.md) | 공연 지도의 리스트 보기에서 일부 공연 항목의 이미지가 깨져 보이던 문제를 개선해, 깔끔한 이미지로 표시되도록 했습니다. |
| 2026-06-05 | [r1.51.1](releases/2026-06-05_r1.51.1_web_shows-venue-detail-crash-fix.md) | 공연 지도에서 공연장 상세 화면에 들어갈 때 모든 공연장에서 오류 페이지가 뜨던 문제를 해결했습니다. |
| 2026-06-05 | [r1.51.4](releases/2026-06-05_r1.51.4_web_legal-docs-bizinfo-toggle.md) | 개인정보처리방침과 이용약관을 관련 법 기준에 맞게 보강하고, 법률 페이지에서 한국어와 영어를 바로 전환해 볼 수 있게 했습니다. |
| 2026-06-04 | [r1.51.2](releases/2026-06-04_r1.51.2_web_shows-list-4category-order.md) | 공연 지도의 리스트 보기에서 공연이 더 직관적인 순서로 정렬되도록 개선했습니다. |
| 2026-06-04 | [r1.51.3](releases/2026-06-04_r1.51.3_web_refund-policy-consistency.md) | 공연별 환불 정책이 구매 화면, 환불 화면, 실제 환불 처리에 일관되게 표시·적용되도록 정리했습니다. |
| 2026-06-04 | [r1.51.5](releases/2026-06-04_r1.51.5_web_artist-share-drop-card.md) | 아티스트 프로필 공유 링크가 예시 데이터 대신 실제 정보가 담긴 "드롭 명함" 화면으로 곧바로 연결됩니다. |
| 2026-06-04 | [r1.51.7](releases/2026-06-04_r1.51.7_web_onboarding-nickname-duplicate-check.md) | 가입 온보딩에서 이미 사용 중인 닉네임을 고르면 곧바로 알려주고 막아줍니다. |
| 2026-06-04 | [r1.51.8](releases/2026-06-04_r1.51.8_web_paypal-unsupported-notice.md) | PayPal 미지원 국가에서의 안내 문구를 명확히 다듬고, 결제 후 주최자 알림과 환불 흐름을 함께 개선했습니다. |
| 2026-06-04 | [r1.51.6](releases/2026-06-04_r1.51.6_web_share-deeplink.md) | 공유한 아티스트·공연장·게시물 링크가 앱의 알맞은 화면으로 더 정확하게 열립니다. |
| 2026-06-03 | [r1.50.20](releases/2026-06-03_r1.50.20_web_sidebar-profile-sheet.md) | 햄버거 메뉴 안의 프로필 사진을 눌러도 반응하지 않던 문제를 수정했습니다. |
| 2026-06-03 | [r1.50.19](releases/2026-06-03_r1.50.19_web_search-event-result-navigation.md) | 검색 결과에서 이벤트를 선택해도 상세 화면으로 이동하지 않던 문제를 수정했습니다. |
| 2026-06-02 | [r1.51.0](releases/2026-06-02_r1.51.0_web_global-chat-full-go.md) | MiSFY 커뮤니티에서 메시지와 이벤트 채팅을 더 안정적으로 사용할 수 있도록 글로벌 채팅 기반을 정식 적용했습니다. |
| 2026-06-01 | [r1.50.18](releases/2026-06-01_r1.50.18_web_today-sub-banners.md) | Today 화면 상단 서브배너를 About Us, YouTube, Instagram 중심으로 정리하고, About Us 외부 링크와 YouTube 카드 테두리 가시성을 개선했습니다. |
| 2026-05-31 | [r1.50.17](releases/2026-05-31_r1.50.17_web_web-i18n-admin-checkpoint.md) | 커뮤니티 웹 active route의 ko/en/ja/es/th 선택 UI 언어 전환 범위를 정리하고, 각 route family의 smoke 검증과 운영 배포를 완료했습니다. |
| 2026-05-28 | [r1.50.16](releases/2026-05-28_r1.50.16_web_paypal-checkout-redirect-recovery.md) | 티켓 구매에서 PayPal 결제 승인 화면으로 이동하는 방식을 조정해 결제 테스트 중 PayPal 오류 페이지가 열리던 문제를 완화했습니다. |
| 2026-05-28 | [r1.50.15](releases/2026-05-28_r1.50.15_web_profile-payout-account-delete-fix.md) | 프로필 설정의 정산 계좌 등록 이동과 계정 삭제 확인 흐름을 복구했습니다. |
| 2026-05-28 | [r1.50.14](releases/2026-05-28_r1.50.14_web_paypal-oauth-onboarding-payouts.md) | 아티스트와 베뉴 회원가입 온보딩에서 국가에 따라 국내 계좌와 PayPal 정산 계정 연동을 안내하도록 확장했습니다. |
| 2026-05-28 | [r1.50.9](releases/2026-05-28_r1.50.9_web_paypal-live-settlement-fee-config.md) | PayPal 결제 선택 흐름을 다시 활성화하고, 관리자 Payments 화면에서 정산 수수료를 직접 조정할 수 있게 했습니다. |
| 2026-05-28 | [r1.50.12](releases/2026-05-28_r1.50.12_web_email-code-session-recovery.md) | 이메일 인증번호 입력 후 인증 완료 상태가 바로 유지되도록 웹 인증 흐름을 보강했습니다. |
| 2026-05-28 | [r1.50.11](releases/2026-05-28_r1.50.11_web_share-actions-deeplink-recovery.md) | 공유하기 버튼과 공연 상세 링크가 더 안정적으로 동작하도록 개선했습니다. |
| 2026-05-28 | [r1.50.10](releases/2026-05-28_r1.50.10_web_legacy-password-login-recovery.md) | 기존 이메일 계정의 로그인 입력 검증과 비밀번호 재설정 진입 흐름을 보강했습니다. |
| 2026-05-22 | [r1.50.3](releases/2026-05-22_r1.50.3_web_scoped-location-routes.md) | Today와 Shows에서 필요한 위치 기능을 다시 사용할 수 있도록 하면서 결제 화면에서는 위치 사용을 막았습니다. |
| 2026-05-21 | [r1.49.13](releases/2026-05-21_r1.49.13_web_event-social-links-managed-cards.md) | 공연 수정 후 상세 정보, 티켓 금액, 유튜브·인스타그램 링크 표시가 더 일관되게 반영되도록 개선했습니다. |
| 2026-05-21 | [r1.49.12](releases/2026-05-21_r1.49.12_web_managed-event-edit-navigation.md) | 공연 수정 후 관리 목록의 가격 표시와 뒤로가기 흐름을 개선했습니다. |
| 2026-05-21 | [r1.49.11](releases/2026-05-21_r1.49.11_web_likes-auth-persistence-web.md) | 앱 재실행 후에도 좋아요한 공연이 Likes 화면과 공연 상세에서 유지되도록 개선했습니다. |
| 2026-05-21 | [r1.49.10](releases/2026-05-21_r1.49.10_web_event-detail-flow.md) | 공연 상세, 좋아요, 티켓/게스트리스트, 공유 흐름의 안정성을 개선했습니다. |
| 2026-05-21 | [r1.49.10](releases/2026-05-21_r1.49.10_web_apple-login-routing-fallback-fix.md) | 운영 커뮤니티 웹에서 Apple 로그인 버튼이 잘못된 로그인 경로로 이동하던 문제를 수정했습니다. |

### Backend

| Date | Version | Summary |
|---|---|---|
| 2026-06-15 | [r1.53.6](releases/2026-06-15_r1.53.6_backend_admin-member-delete-fix.md) | 관리자 회원 관리에서 일부 회원을 삭제할 때 오류가 나던 문제를 해결해, 회원 삭제가 정상적으로 완료되도록 했습니다. |
| 2026-06-06 | [r1.52.6](releases/2026-06-06_r1.52.6_backend_artist-follow-foundation.md) | 더 다양한 아티스트를 팔로우할 수 있는 기반을 마련하고, 일부 프로필에서 참석한 공연 목록이 보이지 않던 문제를 해결했습니다. |
| 2026-06-05 | [r1.52.4](releases/2026-06-05_r1.52.4_backend_public-pii-hardening-rollout.md) | 공개 화면에 제공되는 정보가 꼭 필요한 항목만 포함되도록 개인정보 보호를 한층 더 확대했습니다. |
| 2026-06-05 | [r1.52.2](releases/2026-06-05_r1.52.2_backend_signup-email-duplicate-prevention.md) | 같은 이메일 주소로 서로 다른 로그인 방식을 쓰면 별개의 계정이 따로 만들어지던 문제를 개선해, 한 사람이 하나의 계정으로 일관되게 이용할 수 있도록 회원가입·로그인 처리를 강화했습니다. |
| 2026-06-05 | [r1.52.1](releases/2026-06-05_r1.52.1_backend_privacy-hardening.md) | 공개 화면에 제공되는 정보가 꼭 필요한 항목만 포함되도록 개인정보 보호를 강화했습니다. |
| 2026-06-05 | [r1.51.9](releases/2026-06-05_r1.51.9_backend_curation-feed-auto-publish.md) | 월간 큐레이션 일정의 공연 영상이 앱 피드에 자동으로 올라오는 과정을 정비해 더 자연스럽고 정확하게 발행됩니다. |
| 2026-06-01 | [r1.50.22](releases/2026-06-01_r1.50.22_backend_admin-member-delete-transactional-cleanup.md) | 관리자 패널에서 회원 삭제가 더 안정적으로 완료되도록 서버 삭제 흐름을 보강했습니다. |
| 2026-06-01 | [r1.50.21](releases/2026-06-01_r1.50.21_backend_misfy-email-template-delivery.md) | 회원가입, 인증, 비밀번호, 티켓, 문의 관련 메일을 MiSFY 브랜드 디자인 템플릿으로 보낼 수 있도록 메일 발송 구조를 정리했습니다. |
| 2026-05-31 | [r1.50.19](releases/2026-05-31_r1.50.19_backend_notification-language-i18n.md) | 알림 목록과 푸시 알림이 사용자의 선택 언어 또는 기기 언어를 더 잘 따르도록 다국어 처리를 보강했습니다. |
| 2026-05-28 | [r1.50.13](releases/2026-05-28_r1.50.13_backend_email-auth-session-member-delete-recovery.md) | 이메일 인증 완료 후 로그인 상태 유지와 관리자 회원 삭제 흐름을 서버에서 보강했습니다. |
| 2026-05-25 | [r1.50.8](releases/2026-05-25_r1.50.8_backend_ticket-payment-email-delivery.md) | 티켓 결제 후 완료 화면으로 이어지는 흐름과 결제/환불 메일 발송 흐름을 안정화했습니다. |
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

### Data Pipeline

| Date | Version | Summary |
|---|---|---|
| 2026-06-12 | [r1.53.3](releases/2026-06-12_r1.53.3_data-pipeline_today-card-images.md) | Today 화면의 추천 공연 카드에서 일부 이미지가 보이지 않던 문제를 해결해, 공연 이미지가 정상적으로 표시되도록 했습니다. |
| 2026-06-07 | [r1.52.12](releases/2026-06-07_r1.52.12_data-pipeline_map-data-quality.md) | 공연 지도에 잘못 수집되거나 잘못된 위치에 표시되던 항목을 정리하고, 앞으로 더 정확한 공연 정보만 노출되도록 데이터 품질을 개선했습니다. |
| 2026-06-06 | [r1.52.10](releases/2026-06-06_r1.52.10_data-pipeline_ai-event-geocode-enrichment.md) | AI로 수집된 공연이 지도에 올바른 위치로 표시되도록 위치 정보를 보강하고, 매일 진행되는 데이터 정리 과정을 더 빠르고 안정적으로 개선했습니다. |

### Infra

| Date | Version | Summary |
|---|---|---|
| - | - | - |

### Operations

| Date | Version | Summary |
|---|---|---|
| 2026-06-12 | [r1.53.4](releases/2026-06-12_r1.53.4_operations_artist-hide-public-surface.md) | 관리 도구에서 아티스트를 숨김 처리하면 공개 화면에 곧바로 반영되도록 개선했습니다. |
| 2026-06-12 | [release-assistant-v0.1](releases/2026-06-12_release-assistant-v0.1_operations_ios-release-assistant-open-source.md) | iOS 앱 출시 준비를 단계별로 도와주는 iOS Release Assistant를 오픈소스 도구로 정리하고, 초보자도 따라갈 수 있도록 문서를 보강했습니다. |
| 2026-06-09 | [release-history-v4](releases/2026-06-09_release-history-v4_operations_public-release-history-sanitized-refresh.md) | 공개 릴리즈 히스토리를 정제해 내부 개발 로그성 항목을 제거하고, 실제 사용자에게 설명할 수 있는 변경 이력 중심으로 다시 정리했습니다. |
| 2026-06-09 | [r1.53.2](releases/2026-06-09_r1.53.2_operations_report-notification-routing.md) | POMFS 운영 보고와 자동 알림 메일의 기본 수신 경로를 정리해, 중요한 운영 알림이 한 곳으로 모이도록 개선했습니다. |
| 2026-06-07 | [r1.52.11](releases/2026-06-07_r1.52.11_operations_app-homepage-stats-alignment.md) | 앱과 공식 홈페이지에 표시되는 공연장·아티스트·국가 수치가 항상 동일한 기준의 최신 값으로 함께 정렬되도록 정비했습니다. |
| 2026-06-06 | [r1.52.9](releases/2026-06-06_r1.52.9_operations_event-auto-publish.md) | 매일 자동으로 수집된 공연 중 발행 기준을 충족하는 공연이 자동으로 앱에 올라가도록 개선했습니다. |
| 2026-06-05 | [r1.52.5](releases/2026-06-05_r1.52.5_operations_release-deploy-automation.md) | 앱 업데이트가 더 빠르고 안정적으로 반영되도록 배포 과정을 정비했으며, 사용자가 체감하는 기능 변화는 없습니다. |
| 2026-06-05 | [r1.52.0](releases/2026-06-05_r1.52.0_operations_discovery-collection-publish-pipeline.md) | 공연·공연장 정보가 매일 자동으로 수집·정리되어 더 많은 공연장과 한국 공연이 앱에 노출됩니다. |
| 2026-05-31 | [r1.50.20](releases/2026-05-31_r1.50.20_operations_multilingual-rollup.md) | POMFS의 다국어 작업 범위를 한 번에 정리했습니다. 커뮤니티 웹 active route, 알림/푸시, 기기 언어 자동 선택, iOS 언어 전달, 메일 템플릿까지 ko/en/ja/es/th 기준으로 일관된 언어 경험을 제공하도록 정리했습니다. |
| 2026-05-22 | [release-history-v3](releases/2026-05-22_release-history-v3_operations_release-history-claude-code-token-snapshots.md) | Public release notes에서 Claude Code 누적 토큰 사용량도 함께 확인할 수 있도록 자동화를 보강했습니다. |
| 2026-05-22 | [release-history-v2](releases/2026-05-22_release-history-v2_operations_release-history-codex-token-snapshots.md) | Public release notes와 iOS README가 같은 Codex 누적 토큰 스냅샷을 표시하도록 release history 자동화를 보강했습니다. |
| 2026-05-21 | [release-history-v1](releases/2026-05-21_release-history-v1_operations_release-history-scaffold.md) | POMFS 변경 이력을 구조적으로 기록하고 검증하는 release history 체계를 추가했습니다. |
| 2026-05-17 | [r1.43](releases/2026-05-17_r1.43_operations_session-handoff-automation.md) | 내부 릴리스 및 세션 handoff 자동화를 개선했습니다. |

## Browse / Filters

- All releases
- iOS
- Web
- Backend
- Data Pipeline
- Infra
- Operations
- Monthly archive
