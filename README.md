# POMFS Release History

이 저장소는 POMFS의 공개 릴리즈 히스토리입니다.

각 항목은 private source repo의 release metadata에서 생성되며, 공개 가능한 요약만 포함합니다. iOS, Android, Web, Backend, Data Pipeline, Operations 변경을 시간순으로 모아 보여줍니다.

공개 노트에는 source code, 내부 경로, 개인 이메일, private infrastructure detail, token/key, raw commit hash, sensitive security detail을 포함하지 않습니다.

상세 항목에는 Summary, Changes, Known Issues가 있으며, 시간이 확인된 항목은 `Released at`을 함께 표시합니다.

## About P.O.MFS Dev Team

P.O.MFS Dev Team은 P.O.MFS와 MiSFY 생태계를 설계하고 운영하는 제품·엔지니어링 팀입니다. 커뮤니티 앱, 백엔드/API, 데이터 파이프라인, 운영 자동화, AI 기반 개발 워크플로우, 오픈소스 도구를 함께 만들며 실제 서비스 운영에서 검증된 개선 사항을 공개 가능한 형태로 정리합니다.

이 공개 릴리즈 히스토리는 P.O.MFS Dev Team의 David Kwon이 만들고 관리합니다. P.O.MFS 공식 홈페이지는 [prideofmisfits.com](https://www.prideofmisfits.com)입니다.

## AI Lifetime Token Usage

Codex와 Claude Code의 전체 누적 토큰량입니다. 로컬 세션 로그는 시간이 지나면 정리되므로, 정리와 무관하게 누적값이 단조 증가(감소하지 않음)하도록 영구 ledger로 보존합니다. 각 값은 release notes 갱신 시 기록되는 정적 스냅샷이며, Weekly/Monthly는 최근 기간 윈도 값입니다.

### Codex

Codex 전체 누적 토큰량입니다. 이 값은 실시간 대시보드가 아니라 public release notes가 갱신될 때 함께 기록되는 정적 스냅샷입니다.

<table>
  <tr>
    <th align="left">Snapshot</th>
    <td>2026-08-14 12:09 KST</td>
  </tr>
  <tr>
    <th align="left">Scope</th>
    <td>Codex session logs</td>
  </tr>
  <tr>
    <th align="left">Sessions</th>
    <td>704 sessions</td>
  </tr>
  <tr>
    <th align="left">Cumulative total</th>
    <td><strong>10,006,954,774 tokens</strong></td>
  </tr>
  <tr>
    <th align="left">Input</th>
    <td>9,965,812,904 tokens</td>
  </tr>
  <tr>
    <th align="left">Cached input</th>
    <td>9,509,630,720 tokens</td>
  </tr>
  <tr>
    <th align="left">Output</th>
    <td>41,141,870 tokens</td>
  </tr>
  <tr>
    <th align="left">Reasoning output</th>
    <td>13,908,847 tokens</td>
  </tr>
</table>

<table>
  <tr>
    <th align="left">Scale</th>
    <th align="left">Usage Graph</th>
    <th align="right">Percent</th>
  </tr>
  <tr>
    <td>10,050,000,000 tokens</td>
    <td><code>████████████████████</code></td>
    <td align="right">99.6%</td>
  </tr>
</table>

### Claude Code

Claude Code 전체 누적 토큰량입니다. 이 값은 tui-monitor 집계기가 Claude Code session logs를 다시 계산해 기록한 정적 스냅샷입니다.

<table>
  <tr>
    <th align="left">Snapshot</th>
    <td>2026-08-14 12:09 KST</td>
  </tr>
  <tr>
    <th align="left">Scope</th>
    <td>Claude Code session logs</td>
  </tr>
  <tr>
    <th align="left">Session files</th>
    <td>3,896 files</td>
  </tr>
  <tr>
    <th align="left">Assistant entries</th>
    <td>221,947 entries</td>
  </tr>
  <tr>
    <th align="left">Cumulative total</th>
    <td><strong>53,066,702,263 tokens</strong></td>
  </tr>
  <tr>
    <th align="left">Input</th>
    <td>246,494,555 tokens</td>
  </tr>
  <tr>
    <th align="left">Cache creation</th>
    <td>2,810,435,355 tokens</td>
  </tr>
  <tr>
    <th align="left">Cache read</th>
    <td>49,701,239,746 tokens</td>
  </tr>
  <tr>
    <th align="left">Output</th>
    <td>308,532,607 tokens</td>
  </tr>
  <tr>
    <th align="left">Weekly 7d</th>
    <td>1,831,937,513 tokens</td>
  </tr>
  <tr>
    <th align="left">Monthly 30d</th>
    <td>9,035,199,365 tokens</td>
  </tr>
  <tr>
    <th align="left">Daily avg</th>
    <td>445,938,674 tokens/day</td>
  </tr>
</table>

<table>
  <tr>
    <th align="left">Scale</th>
    <th align="left">Usage Graph</th>
    <th align="right">Percent</th>
  </tr>
  <tr>
    <td>53,100,000,000 tokens</td>
    <td><code>████████████████████</code></td>
    <td align="right">99.9%</td>
  </tr>
</table>

## Latest

| Date | Version | Component | Summary |
|---|---|---|---|
| 2026-08-14 | [r1.56.61](releases/2026-08-14_r1.56.61_web_guidance-and-security-improvements.md) | Web | 잘못된 안내 문구와 표시 오류를 바로잡고 보안을 강화했습니다. |
| 2026-08-14 | [r1.56.60](releases/2026-08-14_r1.56.60_web_likes-bookmarks-fixes.md) | Web | 좋아요와 즐겨찾기의 표시·동작 오류를 수정했습니다. |
| 2026-08-14 | [r1.56.59](releases/2026-08-14_r1.56.59_web_project-collaboration-fixes.md) | Web | 프로젝트 관리와 협업 화면의 동작 오류를 수정했습니다. |
| 2026-08-14 | [r1.56.58](releases/2026-08-14_r1.56.58_web_date-time-display-accuracy.md) | Web | 앱 곳곳의 날짜와 시간 표시를 한국 시간 기준으로 정확하게 바로잡았습니다. |
| 2026-08-14 | [r1.56.57](releases/2026-08-14_r1.56.57_web_venue-map-photo-display.md) | Web | 콘서트맵에서 공연장 사진이 올바르게 표시되도록 개선했습니다. |
| 2026-08-14 | [r1.56.56](releases/2026-08-14_r1.56.56_web_service-store-application-revamp.md) | Web | 서비스 스토어의 신청 과정을 개편하고 표시 오류를 정리했습니다. |
| 2026-08-14 | [r1.56.55](releases/2026-08-14_r1.56.55_web_language-and-screen-fixes.md) | Web | 앱 언어 표시와 아티스트 전용 화면 등 여러 화면의 오류를 수정했습니다. |
| 2026-08-14 | [r1.56.54](releases/2026-08-14_r1.56.54_web_security-and-privacy.md) | Web | 개인정보 보호와 계정 안전을 위한 보안을 강화했습니다. |
| 2026-08-14 | [r1.56.53](releases/2026-08-14_r1.56.53_web_service-store-and-my-projects.md) | Web | 서비스 스토어의 신청 과정이 정상 동작하도록 완성되고, 내 프로젝트·공지 관련 편의 기능이 더해졌습니다. |
| 2026-08-14 | [r1.56.52](releases/2026-08-14_r1.56.52_web_ranking-and-apply-improvements.md) | Web | 아티스트·공연장 등록 신청 과정의 안내가 자세해지고 랭킹 화면 이용이 편해졌습니다. |
| 2026-08-14 | [r1.56.51](releases/2026-08-14_r1.56.51_web_event-create-and-discovery.md) | Web | 공연 등록 시 날짜와 시간을 화면에서 바로 선택할 수 있고, 지도와 공연 목록이 더 정확하게 표시됩니다. |
| 2026-08-14 | [r1.56.50](releases/2026-08-14_r1.56.50_web_group-chat-upgrade.md) | Web | 활동 단체 채팅방에 멤버 확인·초대·공유·사진 전송 기능이 더해지고 채팅 사용성이 개선되었습니다. |
| 2026-08-11 | [r1.56.49](releases/2026-08-11_r1.56.49_web_venue-apply-sns-check.md) | Web | 공연장 신청 시 입력한 SNS 계정이 실제로 존재하는지 확인합니다. |
| 2026-08-11 | [r1.56.48](releases/2026-08-11_r1.56.48_web_display-glitch-fixes.md) | Web | 지도 화면과 운영자 회원 화면의 표시 오류를 수정했습니다. |
| 2026-08-11 | [r1.56.47](releases/2026-08-11_r1.56.47_web_chat-channel-name-language.md) | Web | 1:1 대화와 랭킹 채널의 이름이 앱 언어 설정에 맞게 표시됩니다. |
| 2026-08-11 | [r1.56.46](releases/2026-08-11_r1.56.46_web_subscribed-venue-photos.md) | Web | 프로필의 구독 공연장 카드에 공연장 대표 사진이 함께 표시됩니다. |
| 2026-08-11 | [r1.56.45](releases/2026-08-11_r1.56.45_web_display-and-link-stability.md) | Web | 공유 링크로 게시글이 열리지 않던 문제와 여러 화면 표시 오류를 수정했습니다. |
| 2026-08-11 | [r1.56.44](releases/2026-08-11_r1.56.44_web_notification-tab-and-translations.md) | Web | 알림함에 운영 탭을 추가하고 알림 개수 표시와 번역 누락 문제를 수정했습니다. |
| 2026-08-11 | [r1.56.43](releases/2026-08-11_r1.56.43_web_chat-welcome-and-notices.md) | Web | 채팅방 입장 안내와 신규 회원 환영 메시지를 추가하고 운영진 공지 범위를 넓혔습니다. |
| 2026-08-11 | [r1.56.42](releases/2026-08-11_r1.56.42_web_artist-tier-directory-profile.md) | Web | 아티스트를 티어별로 둘러볼 수 있는 목록과 프로필 포스트 관리 기능을 추가했습니다. |
| 2026-08-11 | [r1.56.41](releases/2026-08-11_r1.56.41_web_seller-settlement-accuracy.md) | Web | 판매자 정산 화면의 수수료 표시와 계산 기준을 바로잡고 정산 절차를 정비했습니다. |
| 2026-08-11 | [r1.56.40](releases/2026-08-11_r1.56.40_web_payment-refund-improvements.md) | Web | 티켓 결제 완료 화면 오류를 수정하고 환불 안내와 영수증 처리를 정비했습니다. |
| 2026-08-10 | [r1.56.39](releases/2026-08-10_r1.56.39_web_overseas-payout-support.md) | Web | 해외 42개국에서 정산 계정을 등록하고 수익을 받을 수 있게 되었습니다. |
| 2026-08-10 | [r1.56.38](releases/2026-08-10_r1.56.38_web_app-stability-and-security.md) | Web | 앱 실행과 저장 과정에서 발생하던 오류를 해결하고 보안을 강화했습니다. |
| 2026-08-10 | [r1.56.37](releases/2026-08-10_r1.56.37_web_chat-notification-display.md) | Web | 채팅과 알림, 공유 문구가 제대로 보이도록 여러 표시 문제를 수정했습니다. |
| 2026-08-10 | [r1.56.36](releases/2026-08-10_r1.56.36_web_map-search-date-accuracy.md) | Web | 지도와 검색에서 공연 수와 '오늘' 기준이 정확하게 표시되도록 수정했습니다. |
| 2026-08-10 | [r1.56.35](releases/2026-08-10_r1.56.35_web_live-video-playback.md) | Web | 공연 상세 화면에서 영상을 바로 재생할 수 있게 되었습니다. |
| 2026-08-10 | [r1.56.34](releases/2026-08-10_r1.56.34_web_artist-profile-ranking-improvements.md) | Web | 아티스트 프로필과 랭킹이 실제 활동 내용을 정확하게 보여주도록 개선했습니다. |
| 2026-08-10 | [r1.56.33](releases/2026-08-10_r1.56.33_web_promo-code-management.md) | Web | 프로모션 코드를 직접 삭제하거나 사용 중지할 수 있도록 하고 보안을 강화했습니다. |
| 2026-08-10 | [r1.56.32](releases/2026-08-10_r1.56.32_web_map-display-fixes.md) | Web | 지도에서 공연장 표시가 실제 공연 상황과 다르게 보이던 문제를 해결했습니다. |
| 2026-08-10 | [r1.56.31](releases/2026-08-10_r1.56.31_web_venue-management-fixes.md) | Web | 공연장 공지와 공연 정보 저장이 정상적으로 처리되도록 수정했습니다. |
| 2026-08-10 | [r1.56.30](releases/2026-08-10_r1.56.30_web_artist-profile-improvements.md) | Web | 아티스트 프로필과 공개 카드에 실제 활동 정보가 정확히 표시되도록 개선했습니다. |
| 2026-08-10 | [r1.56.29](releases/2026-08-10_r1.56.29_web_artist-rank-application.md) | Web | '나의 등급' 화면을 신청 상태에 맞춰 개편하고 신청 자료 첨부 과정을 개선했습니다. |
| 2026-08-10 | [r1.56.28](releases/2026-08-10_r1.56.28_web_notification-link-fix.md) | Web | 알림과 안내 메일에서 눌렀을 때 화면이 열리지 않던 문제를 해결했습니다. |
| 2026-08-03 | [r1.56.27](releases/2026-08-03_r1.56.27_web_legal-and-settlement-notices.md) | Web | 법적 고지와 취소·환불 정책 안내를 정비하고 사업자 정보 표기를 정리했습니다. |
| 2026-08-03 | [r1.56.26](releases/2026-08-03_r1.56.26_web_admin-active-user-stats.md) | Web | 관리자 통계 화면에 주간·월간 활성 사용자 수를 새로 제공합니다. |
| 2026-08-03 | [r1.56.25](releases/2026-08-03_r1.56.25_web_admin-tools-stability.md) | Web | 등급 신청 관리와 프로모션 코드 발행 화면의 오류를 바로잡았습니다. |
| 2026-08-03 | [r1.56.24](releases/2026-08-03_r1.56.24_web_notification-and-email-cleanup.md) | Web | 저녁 요약 알림의 내용 누락과 중복 알림 문제를 해결하고 메일 발신 이름을 통일했습니다. |
| 2026-08-03 | [r1.56.23](releases/2026-08-03_r1.56.23_web_show-list-display-fixes.md) | Web | 첫 화면과 공연 목록에서 공연이 빠지거나 잘못 보이던 문제를 바로잡았습니다. |
| 2026-08-03 | [r1.56.22](releases/2026-08-03_r1.56.22_web_rank-application-revamp.md) | Web | 아티스트·공연장 등급을 유료 상품 없이 무료 신청과 승인으로 받도록 절차를 정비했습니다. |
| 2026-07-25 | [r1.56.18](releases/2026-07-25_r1.56.18_web_mail-sender-identity.md) | Web | MiSFY에서 보내는 모든 메일의 발신 주소를 공식 주소로 통일했습니다. |
| 2026-07-24 | [r1.56.21](releases/2026-07-24_r1.56.21_web_security-hardening.md) | Web | 결제와 티켓, 로그인 관련 요청이 항상 올바르게 처리되도록 앱의 보안을 강화했습니다. |
| 2026-07-24 | [r1.56.20](releases/2026-07-24_r1.56.20_web_seo-crawler-info.md) | Web | 검색엔진이 MiSFY의 화면을 제대로 찾아갈 수 있도록 안내 정보 제공 방식을 바로잡았습니다. |
| 2026-07-24 | [r1.56.19](releases/2026-07-24_r1.56.19_web_collab-service-order-fix.md) | Web | 협업 제안 화면과 서비스 주문 과정에서 발생하던 오류를 수정했습니다. |
| 2026-07-24 | [r1.56.17](releases/2026-07-24_r1.56.17_web_ticket-email-event-name.md) | Web | 티켓 결제 완료 이메일과 알림에 다른 공연 이름이 표시되던 문제를 수정했습니다. |
| 2026-07-24 | [r1.56.16](releases/2026-07-24_r1.56.16_web_refund-request-restore.md) | Web | 티켓 환불 예상 금액 조회와 환불 신청이 정상적으로 진행되지 않던 문제를 수정했습니다. |
| 2026-07-24 | [r1.56.15](releases/2026-07-24_r1.56.15_web_chat-message-edit-followup.md) | Web | 채팅 메시지 수정 기능에서 발생하던 불편을 개선했습니다. |
| 2026-07-24 | [r1.56.14](releases/2026-07-24_r1.56.14_web_ticket-order-failure-fix.md) | Web | 티켓 구매 시 주문이 생성되지 않아 결제를 진행할 수 없던 문제를 수정했습니다. |
| 2026-07-23 | [r1.56.13](releases/2026-07-23_r1.56.13_web_artist-bio-sync-fix.md) | Web | 프로필 설정에서 아티스트 소개를 수정해도 공개 명함(DROP)과 프로필에 옛 소개가 남아 있던 문제를 긴급 수정했습니다. |
| 2026-07-23 | [r1.56.12](releases/2026-07-23_r1.56.12_web_chat-message-edit.md) | Web | 채팅에서 내가 보낸 메시지를 밀어서 수정할 수 있는 기능을 추가했습니다. |
| 2026-07-23 | [r1.56.11](releases/2026-07-23_r1.56.11_web_home-social-links.md) | Web | 홈 화면의 소셜 바로가기가 MiSFY 공식 유튜브·인스타그램 계정으로 올바르게 연결되도록 수정했습니다. |
| 2026-07-23 | [r1.56.10](releases/2026-07-23_r1.56.10_web_staff-channel-monitoring.md) | Web | 전체 채팅과 아티스트·공연장 채널에 새 메시지가 올라오면 스태프에게 알림이 전달되어 운영 대응이 더 빨라졌습니다. |
| 2026-07-23 | [r1.56.9](releases/2026-07-23_r1.56.9_web_artist-ranking-tiebreak.md) | Web | 아티스트 랭킹에서 점수가 같은 경우, 실제 프로필 사진과 장르 정보를 갖춘 아티스트가 먼저 표시되도록 정렬을 개선했습니다. |
| 2026-07-23 | [r1.56.8](releases/2026-07-23_r1.56.8_web_announce-self-receive.md) | Web | 공지를 보낸 스태프 본인도 알림을 받아 발송이 잘 되었는지 바로 확인할 수 있도록 개선했습니다. |
| 2026-07-22 | [3.0.2](releases/2026-07-22_3.0.2_android_google-login-fix.md) | Android | 안드로이드 앱 첫 화면에서 구글 로그인이 실패하던 문제를 근본적으로 해결했습니다. |
| 2026-07-22 | [r1.56.7](releases/2026-07-22_r1.56.7_web_app-update-detection.md) | Web | 업데이트 배포 후에도 일부 기기에서 이전 화면이 계속 실행되던 문제를 수정하고, 새 버전 안내가 정상적으로 표시되도록 복구했습니다. |
| 2026-07-22 | [r1.56.6](releases/2026-07-22_r1.56.6_web_chat-composer-improvements.md) | Web | 채팅에서 줄바꿈 입력, 길게 눌러 반응하기, 이모지 선택창 표시가 더 자연스럽게 동작하도록 개선했습니다. |
| 2026-07-22 | [r1.56.5](releases/2026-07-22_r1.56.5_web_staff-announce-broadcast.md) | Web | 스태프가 채팅에서 '공지로 보내기'를 켜고 메시지를 보내면 아티스트·공연장·스태프 전원에게 알림이 발송됩니다. |
| 2026-07-22 | [r1.56.4](releases/2026-07-22_r1.56.4_web_chat-link-thumbnails.md) | Web | 채팅에서 유튜브·사운드클라우드·틱톡 링크를 보내면 주소 대신 큰 썸네일 카드로 표시됩니다. |
| 2026-07-21 | [r1.56.3](releases/2026-07-21_r1.56.3_web_search-event-title-fix.md) | Web | 검색 결과에서 공연 포스트 제목이 표시되지 않던 문제와 국가 필터가 올바르게 동작하지 않던 문제를 수정했습니다. |
| 2026-07-20 | [r1.56.2](releases/2026-07-20_r1.56.2_web_hardening-privacy.md) | Web | 티켓 조회 시 개인정보 보호를 강화하고, 채팅 메시지 삭제가 모든 화면에 실시간으로 반영되도록 개선했습니다. |
| 2026-07-20 | [r1.56.1](releases/2026-07-20_r1.56.1_web_chat-translate-reactions.md) | Web | 모든 채팅 화면에서 메시지를 번역해 보고, 이모지로 반응할 수 있는 기능을 추가했습니다. |
| 2026-07-20 | [r1.56.0](releases/2026-07-20_r1.56.0_web_together-v3-map-hub.md) | Web | 함께 즐기기가 공연 지도와 하나로 통합되어, 지도에서 바로 모임을 찾고 공연 카드에서 곧장 모임을 만들거나 참여할 수 있게 되었습니다. |
| 2026-07-19 | [r1.55.42](releases/2026-07-19_r1.55.42_web_image-thumbnails.md) | Web | 업로드된 이미지에 경량 썸네일을 자동 생성하고 목록·지도·홈 화면에 적용하여 앱 전반의 이미지 로딩 속도를 크게 개선했습니다. |
| 2026-07-17 | [r1.55.41](releases/2026-07-17_r1.55.41_web_chat-participants-avatars.md) | Web | 전체 채팅 방 상단에서 지금 접속 중인 참여자들의 프로필 사진과 인원수를 한눈에 확인할 수 있게 되었습니다. |
| 2026-07-16 | [r1.55.40](releases/2026-07-16_r1.55.40_web_delete-reliability.md) | Web | 구독자나 판매 이력이 있는 공연·공연장, 피드 글을 삭제할 때 오류로 실패하던 문제를 수정하고, 삭제할 수 없는 경우 이유를 명확히 안내하도록 개선했습니다. |
| 2026-07-16 | [r1.55.39](releases/2026-07-16_r1.55.39_web_ux-error-polish.md) | Web | 공연장 이벤트 게스트리스트 오표시와 리뷰 제출 결과 안내를 바로잡고, 오류 상황에서의 안내를 전반적으로 개선했습니다. |
| 2026-07-15 | [r1.55.38](releases/2026-07-15_r1.55.38_web_paypal-copy-cleanup.md) | Web | 결제·정산 화면에 남아 있던 사용하지 않는 결제 수단(PayPal) 표기를 정리하여 현재 지원하는 결제 수단 기준으로 안내를 통일했습니다. |
| 2026-07-15 | [r1.55.37](releases/2026-07-15_r1.55.37_web_ai-venue-map-markers.md) | Web | 공연 지도에서 AI 수집 공연장도 마커로 표시되고, 상세 화면에서 배지로 구분할 수 있게 되었습니다. |
| 2026-07-15 | [r1.55.36](releases/2026-07-15_r1.55.36_web_together-polish.md) | Web | 함께 즐기기 모임 목록에서 각 모임이 어떤 공연과 연결되어 있는지 한눈에 확인할 수 있도록 개선했습니다. |
| 2026-07-14 | [r1.55.35](releases/2026-07-14_r1.55.35_web_initial-bundle-chat-realtime.md) | Web | 첫 접속 시 앱이 더 빠르게 열리고, 채팅이 새로고침 없이 실시간으로 반영되도록 개선했습니다. |
| 2026-07-14 | [r1.55.34](releases/2026-07-14_r1.55.34_web_map-home-payload-slim.md) | Web | 공연 지도와 홈 화면이 불러오는 데이터 양을 대폭 줄여 화면이 훨씬 빠르게 열리도록 개선했습니다. |
| 2026-07-13 | [r1.55.33](releases/2026-07-13_r1.55.33_web_loading-speed-phase1.md) | Web | 앱 첫 화면이 뜨는 속도를 크게 개선하고, 공연장 목록과 채팅의 데이터 처리를 가볍게 다듬었습니다. |
| 2026-07-13 | [r1.55.32](releases/2026-07-13_r1.55.32_web_intl-settlement-notice.md) | Web | 해외(한국 외) 정산 등록을 일시적으로 중단하고, 2026년 9월 중 지원 예정임을 미리 안내하도록 했습니다. |
| 2026-07-13 | [r1.55.31](releases/2026-07-13_r1.55.31_web_feed-link-embeds.md) | Web | 피드와 Today 게시글 본문에 적힌 링크가 자동으로 썸네일·영상 미리보기 카드로 표시됩니다. |
| 2026-07-13 | [r1.55.30](releases/2026-07-13_r1.55.30_web_notification-prompt-tap-fix.md) | Web | 알림 허용 안내 창의 버튼이 눌리지 않던 문제를 수정했습니다. |
| 2026-07-12 | [r1.55.29](releases/2026-07-12_r1.55.29_web_admin-theme-color-editor.md) | Web | 운영 관리자가 앱의 테마 색상을 직접 편집할 수 있는 관리 도구를 추가했습니다(현재 기본 색상은 그대로이며, 관리자가 값을 저장하기 전까지 사용자 화면은 변하지 않습니다). |
| 2026-07-11 | [r1.55.28](releases/2026-07-11_r1.55.28_web_legal-paypal-to-stripe.md) | Web | 이용약관·개인정보 처리방침에서 더 이상 사용하지 않는 PayPal 관련 문구를 정리하고, 결제·정산 안내를 현재 수단(토스·Stripe)에 맞게 갱신했습니다. |
| 2026-07-11 | [r1.55.27](releases/2026-07-11_r1.55.27_web_paypal-retirement.md) | Web | 결제 수단을 국내 토스·해외 Stripe로 일원화하고, 더 이상 사용하지 않는 PayPal 결제를 앱에서 전면 정리했습니다. |
| 2026-07-11 | [r1.55.26](releases/2026-07-11_r1.55.26_web_venue-edit-fields.md) | Web | 공연장 정보 수정 화면에서 전화번호·웹사이트·수용 인원·운영 시간을 저장해도 반영되지 않던 문제를 수정했습니다. |
| 2026-07-11 | [r1.55.25](releases/2026-07-11_r1.55.25_web_payment-region-routing.md) | Web | 티켓 결제 화면에서 결제사 선택 버튼을 없애고, 지역에 따라 결제 방식을 자동으로 정하도록 바꿨습니다. |
| 2026-07-11 | [r1.55.24](releases/2026-07-11_r1.55.24_web_admin-refund-approvals.md) | Web | 운영 관리자가 앱에서 직접 티켓 환불을 승인·거절할 수 있는 화면을 추가했습니다. |
| 2026-07-10 | [r1.55.23](releases/2026-07-10_r1.55.23_web_partial-refund-fix.md) | Web | 해외 티켓 부분 환불이 결제사에서는 처리됐으나 앱 기록이 갱신되지 않던 문제를 수정했습니다. |
| 2026-07-10 | [r1.55.22](releases/2026-07-10_r1.55.22_web_refund-request-feedback.md) | Web | 티켓 환불 신청이 접수돼도 화면에 아무 안내가 없어 여러 번 눌리던 문제를 수정했습니다. |
| 2026-07-10 | [r1.55.21](releases/2026-07-10_r1.55.21_web_venue-event-edit.md) | Web | 공연장 관리에서 등록한 공연의 수정 버튼이 동작하지 않던 문제를 수정했습니다. |
| 2026-07-10 | [r1.55.20](releases/2026-07-10_r1.55.20_web_intl-payment-stabilization.md) | Web | 해외 티켓 결제에서 주문이 거절되거나 카드 입력 화면이 나타나지 않던 문제를 수정하고, 첫 해외 실결제(태국 바트)를 검증했습니다. |
| 2026-07-10 | [r1.55.19](releases/2026-07-10_r1.55.19_web_intl-stripe-ticket-payment.md) | Web | 해외 공연 티켓을 현지 통화로 Stripe 카드 결제할 수 있게 했습니다. |
| 2026-07-09 | [r1.55.18](releases/2026-07-09_r1.55.18_web_admin-stripe-settlement.md) | Web | 운영 스태프가 해외 정산 대상을 미리 확인하고 일괄 정산을 실행할 수 있는 관리자 콘솔을 추가했습니다. |
| 2026-07-09 | [r1.55.17](releases/2026-07-09_r1.55.17_web_deploy-stability.md) | Web | 서비스 업데이트 직후 일부 브라우저에서 빈 화면이 나타날 수 있던 문제를 방지하도록 배포 방식을 개선했습니다. |
| 2026-07-09 | [r1.55.16](releases/2026-07-09_r1.55.16_web_global-payouts-groundwork.md) | Web | 해외 아티스트·공연장 정산을 더 많은 국가로 확장하기 위한 기반을 준비했습니다(순차 활성화 예정). |
| 2026-07-09 | [r1.55.15](releases/2026-07-09_r1.55.15_web_paypal-surface-cleanup.md) | Web | 결제 수단을 국내(Toss)/해외(Stripe)로 일원화하는 과정에서, 화면에 남아 있던 PayPal 관련 표시를 정리했습니다. |
| 2026-07-09 | [r1.55.14](releases/2026-07-09_r1.55.14_web_admin-venue-images.md) | Web | 운영 스태프가 관리자 화면에서 공연장의 로고와 커버 이미지를 직접 등록·수정할 수 있습니다. |
| 2026-07-09 | [r1.55.13](releases/2026-07-09_r1.55.13_web_hangout-entry-on-map.md) | Web | 함께 즐기기를 별도 화면 이동 없이 공연 지도 위에서 바로 시작할 수 있습니다. |
| 2026-07-09 | [r1.55.12](releases/2026-07-09_r1.55.12_web_payment-amount-simplify.md) | Web | 결제 화면 상단의 중복 금액 카드를 없애고 금액을 결제 버튼에서 바로 확인하도록 정리해, 필수 동의가 한 화면에 보이게 했습니다. |
| 2026-07-09 | [r1.55.11](releases/2026-07-09_r1.55.11_web_collab-delete-hero-fallback.md) | Web | 협업·모집 글 상세에서 작성자와 운영 스태프가 글을 삭제할 수 있고, 포스터가 없을 때 장르색 배경이 표시됩니다. |
| 2026-07-09 | [r1.55.10](releases/2026-07-09_r1.55.10_web_payment-selector-cleanup.md) | Web | 티켓 결제 화면을 정리하고, 국내(Toss) 결제 시 필수 약관 동의 절차를 추가했습니다. 해외 결제 옵션은 준비 중입니다. |
| 2026-07-09 | [r1.55.9](releases/2026-07-09_r1.55.9_web_ticket-intl-phone.md) | Web | 티켓 구매 정보 입력 화면에서 국가 번호를 선택해 해외 전화번호도 입력할 수 있게 했습니다. |
| 2026-07-09 | [r1.55.8](releases/2026-07-09_r1.55.8_web_collab-post-edit.md) | Web | 작성자와 운영 스태프가 등록한 협업·모집 글을 나중에 수정할 수 있게 했습니다. |
| 2026-07-09 | [r1.55.7](releases/2026-07-09_r1.55.7_web_venue-profile-image-edit.md) | Web | 공연장 관리자가 공연장 프로필 사진을 직접 올리고 수정할 수 있게 했습니다. |
| 2026-07-09 | [r1.55.6](releases/2026-07-09_r1.55.6_web_feed-story-rail-align.md) | Web | 피드 상단 스토리 줄에서 새 게시물이 있는 항목과 없는 항목의 크기·정렬이 어긋나던 부분을 맞췄습니다. |
| 2026-07-09 | [r1.55.5](releases/2026-07-09_r1.55.5_web_map-layer-source-split.md) | Web | 공연 지도의 상단 탭에서 '공연장'은 실제 등록된 공연장만, 'AI'는 AI로 수집한 공연장을 보여주도록 데이터 구분을 명확히 했습니다. |
| 2026-07-09 | [r1.55.4](releases/2026-07-09_r1.55.4_web_artist-youtube-preview.md) | Web | 아티스트 프로필 음악 탭에 YouTube 채널 링크만 넣어도 최신 영상이 자동으로 재생 미리보기로 뜨도록 인식 범위를 넓혔습니다. |
| 2026-07-08 | [r1.55.3](releases/2026-07-08_r1.55.3_web_feed-ai-author-profile.md) | Web | 피드에서 AI가 작성한 글의 작성자 프로필을 열 때 프로필을 불러오지 못하던 문제를 해결하고, 해당 프로필에서 AI 글이 함께 보이도록 했습니다. |
| 2026-07-08 | [r1.55.2](releases/2026-07-08_r1.55.2_web_feed-following-stories.md) | Web | 피드 상단에 팔로우한 프로필과 추천 아티스트를 가로로 보여주는 스토리 레일을 추가하고, 새 글이 올라온 프로필은 링으로 눈에 띄게 표시합니다. |
| 2026-07-08 | [r1.55.1](releases/2026-07-08_r1.55.1_web_chat-link-preview.md) | Web | 채팅 메시지 속 링크를 자동으로 눌러서 열 수 있게 하고, 링크의 제목·설명·이미지를 담은 미리보기 카드를 함께 보여줍니다. |
| 2026-07-08 | [r1.55.0](releases/2026-07-08_r1.55.0_web_chat-photo-attach.md) | Web | 전체 채팅(채널)에서도 사진을 첨부해 보낼 수 있도록 했습니다. 그동안 개인 메시지에서만 가능하던 사진 전송을 커뮤니티 채팅으로 넓혔습니다. |
| 2026-06-25 | [r1.54.12](releases/2026-06-25_r1.54.12_web_venue-photo-ai-fallback.md) | Web | 공연장 사진이 없을 때 빈 화면 대신 AI 포스터나 아바타 이미지로 자연스럽게 대체 표시되도록 해, 어떤 공연장이든 보기 좋은 화면을 보여줍니다. |
| 2026-06-25 | [r1.54.11](releases/2026-06-25_r1.54.11_web_pull-to-refresh.md) | Web | 메인 탭에서 화면을 아래로 당겨서 새로고침하는 기능을 지원해, 최신 콘텐츠를 더 쉽게 불러올 수 있도록 했습니다. |
| 2026-06-25 | [r1.54.10](releases/2026-06-25_r1.54.10_web_guest-list-checkin-tabs.md) | Web | 게스트리스트 관리 화면을 입장 전과 입장 완료로 구분한 탭으로 개편해, 행사 현장에서 입장 현황을 더 빠르게 파악할 수 있도록 했습니다. |
| 2026-06-25 | [r1.54.9](releases/2026-06-25_r1.54.9_web_map-source-toggle.md) | Web | 공연 지도에서 아티스트 소스와 AI 수집 소스를 토글로 구분해 볼 수 있게 했습니다. |
| 2026-06-25 | [r1.54.8](releases/2026-06-25_r1.54.8_web_map-artist-profiles.md) | Web | 공연 지도와 목록에 표시되는 AI 수집 아티스트를 실제 아티스트 프로필 기반으로 개편했습니다. 핀이나 행을 누르면 해당 아티스트의 상세 정보와 공연 목록을 함께 볼 수 있습니다. |
| 2026-06-24 | [r1.54.13](releases/2026-06-24_r1.54.13_web_android-app-links-verification.md) | Web | 외부에서 공유한 공연 링크를 Android 앱에서 열면 브라우저를 거치지 않고 앱이 바로 열리도록 앱 링크 검증을 추가했습니다. |
| 2026-06-24 | [r1.54.6](releases/2026-06-24_r1.54.6_operations_admin-member-profile-edit.md) | Operations | 관리 도구에 회원 통합 프로필 편집 기능을 추가하고, 아티스트 소개와 SNS 정보 저장이 제대로 반영되도록 관리 기능을 개선했습니다. 운영자 전용 기능입니다. |
| 2026-06-23 | [r1.54.7](releases/2026-06-23_r1.54.7_data-pipeline_ai-model-update.md) | Data Pipeline | 공연 정보 분석과 검색에 사용되는 AI 모델을 업데이트해 안정성을 높였습니다. |
| 2026-06-22 | [r1.54.5](releases/2026-06-22_r1.54.5_backend_rank-promotion-authz-hardening.md) | Backend | 등급 승격 권한 검증을 강화해 잘못된 자가 승격을 방지했습니다. |
| 2026-06-22 | [r1.54.4](releases/2026-06-22_r1.54.4_backend_curation-feed-publish-date-sort.md) | Backend | 큐레이션 피드를 발행일 기준으로 정렬해 최신 콘텐츠가 먼저 보이도록 개선했습니다. |
| 2026-06-22 | [r1.54.3](releases/2026-06-22_r1.54.3_web_map-blank-cache-recovery.md) | Web | 일부 기기에서 공연 지도가 빈 화면으로 표시되던 문제를 지도 데이터 캐시 자동 복구로 해소했습니다. |
| 2026-06-22 | [r1.54.2](releases/2026-06-22_r1.54.2_web_event-like-guest-artist.md) | Web | 이벤트 상세에서 좋아요 상태가 유지되도록 수정하고 게스트 아티스트 표시 동작을 개선했습니다. |
| 2026-06-21 | [r1.54.1](releases/2026-06-21_r1.54.1_web_music-links-external-i18n.md) | Web | 아티스트 음악 링크에 외부 열기 버튼을 추가하고 입력 오류 메시지를 다국어로 제공하는 등 음악 링크의 표시와 저장 경험을 개선했습니다. |
| 2026-06-20 | [r1.54.0](releases/2026-06-20_r1.54.0_web_event-cohost.md) | Web | 공연에 공동 주최자를 초대해 함께 관리할 수 있는 기능을 추가했습니다. |
| 2026-06-20 | [r1.53.17](releases/2026-06-20_r1.53.17_web_shared-link-app-deeplink.md) | Web | 공유한 공연 링크를 앱에서 열면 해당 공연이 바로 보이도록 수정했습니다. |
| 2026-06-20 | [r1.53.16](releases/2026-06-20_r1.53.16_web_artist-lineup.md) | Web | 공연을 등록할 때 출연 아티스트(라인업)를 검색해 추가할 수 있게 했습니다. |
| 2026-06-20 | [r1.53.15](releases/2026-06-20_r1.53.15_web_staff-event-highlight.md) | Web | 운영진이 직접 올린 공연이 앱에서 눈에 띄게 강조되도록 했습니다. |
| 2026-06-18 | [3.0.2](releases/2026-06-18_3.0.2_android_play-closed-testing-prep.md) | Android | MiSFY 안드로이드 앱(3.0.2)을 Google Play 비공개 테스트에 올리기 위한 준비를 진행했습니다. |
| 2026-06-18 | [r1.53.12](releases/2026-06-18_r1.53.12_web_beta-tester-signup-page.md) | Web | 안드로이드 비공개 베타 테스터를 모집하는 신청 페이지를 추가했습니다. |
| 2026-06-18 | [r1.53.11](releases/2026-06-18_r1.53.11_web_account-deletion-page.md) | Web | 계정과 데이터 삭제 방법을 안내하는 공개 페이지를 추가했습니다. |
| 2026-06-18 | [r1.53.10](releases/2026-06-18_r1.53.10_web_ticket-organizer-name-snapshot.md) | Web | 공연 주최자 계정이 삭제되어도, 구매한 티켓에 구매 당시의 주최자 이름이 그대로 표시되도록 했습니다. |
| 2026-06-17 | [r1.53.14](releases/2026-06-17_r1.53.14_operations_admin-member-pagination.md) | Operations | 관리 도구의 회원 목록에서 전체 회원을 페이지로 나눠 보고, 등급별로 빠르게 필터링할 수 있도록 개선했습니다. |
| 2026-06-17 | [r1.53.13](releases/2026-06-17_r1.53.13_operations_admin-member-grade-change.md) | Operations | 관리 도구의 회원 관리에서 회원의 등급을 직접 변경할 수 있는 기능을 추가했습니다. |
| 2026-06-16 | [r1.53.9](releases/2026-06-16_r1.53.9_backend_artist-rank-profile-fields.md) | Backend | 아티스트 등업이 승인된 뒤에도 프로필에 장르가 "기타"로 보이거나 자기소개가 비어 있던 문제를 해결해, 등업 신청 시 입력한 정보가 프로필에 그대로 반영되도록 했습니다. |
| 2026-06-16 | [r1.53.8](releases/2026-06-16_r1.53.8_web_profile-photo-edit-touch.md) | Web | 프로필 사진 편집 화면에서 사진을 손가락으로 움직이거나 확대·축소할 수 없고, 완료를 눌러도 저장되지 않던 문제를 해결했습니다. |
| 2026-06-16 | [r1.53.7](releases/2026-06-16_r1.53.7_web_profile-photo-quality.md) | Web | 프로필 사진을 더 높은 화질로 저장하도록 개선해, 아티스트·리스너 프로필 카드의 큰 배경 이미지가 또렷하게 보입니다. |
| 2026-06-15 | [r1.53.6](releases/2026-06-15_r1.53.6_backend_admin-member-delete-fix.md) | Backend | 관리자 회원 관리에서 일부 회원을 삭제할 때 오류가 나던 문제를 해결해, 회원 삭제가 정상적으로 완료되도록 했습니다. |
| 2026-06-13 | [r1.53.5](releases/2026-06-13_r1.53.5_web_shared-event-link-blank-screen.md) | Web | 외부로 공유한 공연 링크를 열면 화면이 비어 보이던 문제를 해결했습니다. |
| 2026-06-12 | [3.0.0](releases/2026-06-12_3.0.0_ios_app-store-review-submission.md) | iOS | MiSFY iOS 3.0.0 빌드를 App Store 심사에 제출하고, App Store Connect에서 심사 대기 상태까지 확인했습니다. |
| 2026-06-12 | [r1.53.4](releases/2026-06-12_r1.53.4_operations_artist-hide-public-surface.md) | Operations | 관리 도구에서 아티스트를 숨김 처리하면 공개 화면에 곧바로 반영되도록 개선했습니다. |
| 2026-06-12 | [r1.53.3](releases/2026-06-12_r1.53.3_data-pipeline_today-card-images.md) | Data Pipeline | Today 화면의 추천 공연 카드에서 일부 이미지가 보이지 않던 문제를 해결해, 공연 이미지가 정상적으로 표시되도록 했습니다. |
| 2026-06-12 | [release-assistant-v0.1](releases/2026-06-12_release-assistant-v0.1_operations_ios-release-assistant-open-source.md) | Operations | iOS 앱 출시 준비를 단계별로 도와주는 iOS Release Assistant를 오픈소스 도구로 정리하고, 초보자도 따라갈 수 있도록 문서를 보강했습니다. |
| 2026-06-09 | [r1.53.2](releases/2026-06-09_r1.53.2_operations_report-notification-routing.md) | Operations | POMFS 운영 보고와 자동 알림 메일의 기본 수신 경로를 정리해, 중요한 운영 알림이 한 곳으로 모이도록 개선했습니다. |
| 2026-06-09 | [r1.53.1](releases/2026-06-09_r1.53.1_web_feed-genre-badges.md) | Web | Feed 카드에서 일반 AI 표시 대신 공연과 콘텐츠의 장르를 더 분명하게 볼 수 있도록 장르 뱃지를 표시했습니다. |
| 2026-06-09 | [release-history-v4](releases/2026-06-09_release-history-v4_operations_public-release-history-sanitized-refresh.md) | Operations | 공개 릴리즈 히스토리를 정제해 내부 개발 로그성 항목을 제거하고, 실제 사용자에게 설명할 수 있는 변경 이력 중심으로 다시 정리했습니다. |
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
| 2026-05-25 | [r1.50.8](releases/2026-05-25_r1.50.8_ios_ios-payment-return-flow.md) | iOS | iOS 앱에서 Npay와 Toss 결제 후 POMFS 화면으로 돌아오는 흐름을 보강했습니다. |
| 2026-05-25 | [r1.50.8](releases/2026-05-25_r1.50.8_backend_ticket-payment-email-delivery.md) | Backend | 티켓 결제 후 완료 화면으로 이어지는 흐름과 결제/환불 메일 발송 흐름을 안정화했습니다. |
| 2026-05-23 | [r1.50.7](releases/2026-05-23_r1.50.7_backend_settlement-payout-reconciliation.md) | Backend | 정산 화면과 관리자 정산 흐름에서 PayPal 지급과 결제 대사 흐름을 더 정확하게 확인할 수 있도록 보강했습니다. |
| 2026-05-23 | [r1.50.7](releases/2026-05-23_r1.50.7_backend_my-settlement-aggregation.md) | Backend | 정산 화면이 최신 공연 티켓 주문 구조까지 반영해서 판매 금액을 집계하도록 보강했습니다. |
| 2026-05-22 | [r1.50.6](releases/2026-05-22_r1.50.6_backend_paypal-refund-cascade.md) | Backend | PayPal로 결제한 티켓도 환불 완료 후 안내 메일, 공연 생성자 알림, 환불 상태 표시가 Toss 결제와 같은 흐름으로 처리되도록 보강했습니다. |
| 2026-05-22 | [r1.50.5](releases/2026-05-22_r1.50.5_ios_ios-ticket-deeplink-scheme.md) | iOS | iOS 앱에서 티켓 메일의 앱 열기 버튼이 티켓 화면으로 이어질 수 있도록 딥링크 처리를 보강했습니다. |
| 2026-05-22 | [r1.50.5](releases/2026-05-22_r1.50.5_backend_ticket-refund-notifications-management.md) | Backend | 티켓 환불 완료 후 안내 메일과 공연 관리 화면의 환불 상태 표시가 더 정확해지도록 보강했습니다. |
| 2026-05-22 | [r1.50.5](releases/2026-05-22_r1.50.5_backend_ticket-refund-host-notifications.md) | Backend | 티켓 환불이 완료되면 공연 생성자가 알림에서 관련 티켓 관리 화면으로 이동할 수 있도록 알림 흐름을 보강했습니다. |
| 2026-05-22 | [release-history-v3](releases/2026-05-22_release-history-v3_operations_release-history-claude-code-token-snapshots.md) | Operations | Public release notes에서 Claude Code 누적 토큰 사용량도 함께 확인할 수 있도록 자동화를 보강했습니다. |
| 2026-05-22 | [r1.50.4](releases/2026-05-22_r1.50.4_backend_ticket-email-detail-scanner-recovery.md) | Backend | 결제 완료와 티켓 발급 메일, 나의 티켓 상세 보기, QR 확인, 티켓 스캐너 흐름을 실제 발급 티켓 기준으로 보강했습니다. |
| 2026-05-22 | [release-history-v2](releases/2026-05-22_release-history-v2_operations_release-history-codex-token-snapshots.md) | Operations | Public release notes와 iOS README가 같은 Codex 누적 토큰 스냅샷을 표시하도록 release history 자동화를 보강했습니다. |
| 2026-05-22 | [r1.50.3](releases/2026-05-22_r1.50.3_ios_ios-scoped-location-webview.md) | iOS | iOS 앱에서 위치 기능이 필요한 화면에서만 동작하도록 허용 범위를 조정했습니다. |
| 2026-05-22 | [r1.50.3](releases/2026-05-22_r1.50.3_web_scoped-location-routes.md) | Web | Today와 Shows에서 필요한 위치 기능을 다시 사용할 수 있도록 하면서 결제 화면에서는 위치 사용을 막았습니다. |
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

### Android

| Date | Version | Summary |
|---|---|---|
| 2026-07-22 | [3.0.2](releases/2026-07-22_3.0.2_android_google-login-fix.md) | 안드로이드 앱 첫 화면에서 구글 로그인이 실패하던 문제를 근본적으로 해결했습니다. |
| 2026-06-18 | [3.0.2](releases/2026-06-18_3.0.2_android_play-closed-testing-prep.md) | MiSFY 안드로이드 앱(3.0.2)을 Google Play 비공개 테스트에 올리기 위한 준비를 진행했습니다. |

### Web

| Date | Version | Summary |
|---|---|---|
| 2026-08-14 | [r1.56.61](releases/2026-08-14_r1.56.61_web_guidance-and-security-improvements.md) | 잘못된 안내 문구와 표시 오류를 바로잡고 보안을 강화했습니다. |
| 2026-08-14 | [r1.56.60](releases/2026-08-14_r1.56.60_web_likes-bookmarks-fixes.md) | 좋아요와 즐겨찾기의 표시·동작 오류를 수정했습니다. |
| 2026-08-14 | [r1.56.59](releases/2026-08-14_r1.56.59_web_project-collaboration-fixes.md) | 프로젝트 관리와 협업 화면의 동작 오류를 수정했습니다. |
| 2026-08-14 | [r1.56.58](releases/2026-08-14_r1.56.58_web_date-time-display-accuracy.md) | 앱 곳곳의 날짜와 시간 표시를 한국 시간 기준으로 정확하게 바로잡았습니다. |
| 2026-08-14 | [r1.56.57](releases/2026-08-14_r1.56.57_web_venue-map-photo-display.md) | 콘서트맵에서 공연장 사진이 올바르게 표시되도록 개선했습니다. |
| 2026-08-14 | [r1.56.56](releases/2026-08-14_r1.56.56_web_service-store-application-revamp.md) | 서비스 스토어의 신청 과정을 개편하고 표시 오류를 정리했습니다. |
| 2026-08-14 | [r1.56.55](releases/2026-08-14_r1.56.55_web_language-and-screen-fixes.md) | 앱 언어 표시와 아티스트 전용 화면 등 여러 화면의 오류를 수정했습니다. |
| 2026-08-14 | [r1.56.54](releases/2026-08-14_r1.56.54_web_security-and-privacy.md) | 개인정보 보호와 계정 안전을 위한 보안을 강화했습니다. |
| 2026-08-14 | [r1.56.53](releases/2026-08-14_r1.56.53_web_service-store-and-my-projects.md) | 서비스 스토어의 신청 과정이 정상 동작하도록 완성되고, 내 프로젝트·공지 관련 편의 기능이 더해졌습니다. |
| 2026-08-14 | [r1.56.52](releases/2026-08-14_r1.56.52_web_ranking-and-apply-improvements.md) | 아티스트·공연장 등록 신청 과정의 안내가 자세해지고 랭킹 화면 이용이 편해졌습니다. |
| 2026-08-14 | [r1.56.51](releases/2026-08-14_r1.56.51_web_event-create-and-discovery.md) | 공연 등록 시 날짜와 시간을 화면에서 바로 선택할 수 있고, 지도와 공연 목록이 더 정확하게 표시됩니다. |
| 2026-08-14 | [r1.56.50](releases/2026-08-14_r1.56.50_web_group-chat-upgrade.md) | 활동 단체 채팅방에 멤버 확인·초대·공유·사진 전송 기능이 더해지고 채팅 사용성이 개선되었습니다. |
| 2026-08-11 | [r1.56.49](releases/2026-08-11_r1.56.49_web_venue-apply-sns-check.md) | 공연장 신청 시 입력한 SNS 계정이 실제로 존재하는지 확인합니다. |
| 2026-08-11 | [r1.56.48](releases/2026-08-11_r1.56.48_web_display-glitch-fixes.md) | 지도 화면과 운영자 회원 화면의 표시 오류를 수정했습니다. |
| 2026-08-11 | [r1.56.47](releases/2026-08-11_r1.56.47_web_chat-channel-name-language.md) | 1:1 대화와 랭킹 채널의 이름이 앱 언어 설정에 맞게 표시됩니다. |
| 2026-08-11 | [r1.56.46](releases/2026-08-11_r1.56.46_web_subscribed-venue-photos.md) | 프로필의 구독 공연장 카드에 공연장 대표 사진이 함께 표시됩니다. |
| 2026-08-11 | [r1.56.45](releases/2026-08-11_r1.56.45_web_display-and-link-stability.md) | 공유 링크로 게시글이 열리지 않던 문제와 여러 화면 표시 오류를 수정했습니다. |
| 2026-08-11 | [r1.56.44](releases/2026-08-11_r1.56.44_web_notification-tab-and-translations.md) | 알림함에 운영 탭을 추가하고 알림 개수 표시와 번역 누락 문제를 수정했습니다. |
| 2026-08-11 | [r1.56.43](releases/2026-08-11_r1.56.43_web_chat-welcome-and-notices.md) | 채팅방 입장 안내와 신규 회원 환영 메시지를 추가하고 운영진 공지 범위를 넓혔습니다. |
| 2026-08-11 | [r1.56.42](releases/2026-08-11_r1.56.42_web_artist-tier-directory-profile.md) | 아티스트를 티어별로 둘러볼 수 있는 목록과 프로필 포스트 관리 기능을 추가했습니다. |
| 2026-08-11 | [r1.56.41](releases/2026-08-11_r1.56.41_web_seller-settlement-accuracy.md) | 판매자 정산 화면의 수수료 표시와 계산 기준을 바로잡고 정산 절차를 정비했습니다. |
| 2026-08-11 | [r1.56.40](releases/2026-08-11_r1.56.40_web_payment-refund-improvements.md) | 티켓 결제 완료 화면 오류를 수정하고 환불 안내와 영수증 처리를 정비했습니다. |
| 2026-08-10 | [r1.56.39](releases/2026-08-10_r1.56.39_web_overseas-payout-support.md) | 해외 42개국에서 정산 계정을 등록하고 수익을 받을 수 있게 되었습니다. |
| 2026-08-10 | [r1.56.38](releases/2026-08-10_r1.56.38_web_app-stability-and-security.md) | 앱 실행과 저장 과정에서 발생하던 오류를 해결하고 보안을 강화했습니다. |
| 2026-08-10 | [r1.56.37](releases/2026-08-10_r1.56.37_web_chat-notification-display.md) | 채팅과 알림, 공유 문구가 제대로 보이도록 여러 표시 문제를 수정했습니다. |
| 2026-08-10 | [r1.56.36](releases/2026-08-10_r1.56.36_web_map-search-date-accuracy.md) | 지도와 검색에서 공연 수와 '오늘' 기준이 정확하게 표시되도록 수정했습니다. |
| 2026-08-10 | [r1.56.35](releases/2026-08-10_r1.56.35_web_live-video-playback.md) | 공연 상세 화면에서 영상을 바로 재생할 수 있게 되었습니다. |
| 2026-08-10 | [r1.56.34](releases/2026-08-10_r1.56.34_web_artist-profile-ranking-improvements.md) | 아티스트 프로필과 랭킹이 실제 활동 내용을 정확하게 보여주도록 개선했습니다. |
| 2026-08-10 | [r1.56.33](releases/2026-08-10_r1.56.33_web_promo-code-management.md) | 프로모션 코드를 직접 삭제하거나 사용 중지할 수 있도록 하고 보안을 강화했습니다. |
| 2026-08-10 | [r1.56.32](releases/2026-08-10_r1.56.32_web_map-display-fixes.md) | 지도에서 공연장 표시가 실제 공연 상황과 다르게 보이던 문제를 해결했습니다. |
| 2026-08-10 | [r1.56.31](releases/2026-08-10_r1.56.31_web_venue-management-fixes.md) | 공연장 공지와 공연 정보 저장이 정상적으로 처리되도록 수정했습니다. |
| 2026-08-10 | [r1.56.30](releases/2026-08-10_r1.56.30_web_artist-profile-improvements.md) | 아티스트 프로필과 공개 카드에 실제 활동 정보가 정확히 표시되도록 개선했습니다. |
| 2026-08-10 | [r1.56.29](releases/2026-08-10_r1.56.29_web_artist-rank-application.md) | '나의 등급' 화면을 신청 상태에 맞춰 개편하고 신청 자료 첨부 과정을 개선했습니다. |
| 2026-08-10 | [r1.56.28](releases/2026-08-10_r1.56.28_web_notification-link-fix.md) | 알림과 안내 메일에서 눌렀을 때 화면이 열리지 않던 문제를 해결했습니다. |
| 2026-08-03 | [r1.56.27](releases/2026-08-03_r1.56.27_web_legal-and-settlement-notices.md) | 법적 고지와 취소·환불 정책 안내를 정비하고 사업자 정보 표기를 정리했습니다. |
| 2026-08-03 | [r1.56.26](releases/2026-08-03_r1.56.26_web_admin-active-user-stats.md) | 관리자 통계 화면에 주간·월간 활성 사용자 수를 새로 제공합니다. |
| 2026-08-03 | [r1.56.25](releases/2026-08-03_r1.56.25_web_admin-tools-stability.md) | 등급 신청 관리와 프로모션 코드 발행 화면의 오류를 바로잡았습니다. |
| 2026-08-03 | [r1.56.24](releases/2026-08-03_r1.56.24_web_notification-and-email-cleanup.md) | 저녁 요약 알림의 내용 누락과 중복 알림 문제를 해결하고 메일 발신 이름을 통일했습니다. |
| 2026-08-03 | [r1.56.23](releases/2026-08-03_r1.56.23_web_show-list-display-fixes.md) | 첫 화면과 공연 목록에서 공연이 빠지거나 잘못 보이던 문제를 바로잡았습니다. |
| 2026-08-03 | [r1.56.22](releases/2026-08-03_r1.56.22_web_rank-application-revamp.md) | 아티스트·공연장 등급을 유료 상품 없이 무료 신청과 승인으로 받도록 절차를 정비했습니다. |
| 2026-07-25 | [r1.56.18](releases/2026-07-25_r1.56.18_web_mail-sender-identity.md) | MiSFY에서 보내는 모든 메일의 발신 주소를 공식 주소로 통일했습니다. |
| 2026-07-24 | [r1.56.21](releases/2026-07-24_r1.56.21_web_security-hardening.md) | 결제와 티켓, 로그인 관련 요청이 항상 올바르게 처리되도록 앱의 보안을 강화했습니다. |
| 2026-07-24 | [r1.56.20](releases/2026-07-24_r1.56.20_web_seo-crawler-info.md) | 검색엔진이 MiSFY의 화면을 제대로 찾아갈 수 있도록 안내 정보 제공 방식을 바로잡았습니다. |
| 2026-07-24 | [r1.56.19](releases/2026-07-24_r1.56.19_web_collab-service-order-fix.md) | 협업 제안 화면과 서비스 주문 과정에서 발생하던 오류를 수정했습니다. |
| 2026-07-24 | [r1.56.17](releases/2026-07-24_r1.56.17_web_ticket-email-event-name.md) | 티켓 결제 완료 이메일과 알림에 다른 공연 이름이 표시되던 문제를 수정했습니다. |
| 2026-07-24 | [r1.56.16](releases/2026-07-24_r1.56.16_web_refund-request-restore.md) | 티켓 환불 예상 금액 조회와 환불 신청이 정상적으로 진행되지 않던 문제를 수정했습니다. |
| 2026-07-24 | [r1.56.15](releases/2026-07-24_r1.56.15_web_chat-message-edit-followup.md) | 채팅 메시지 수정 기능에서 발생하던 불편을 개선했습니다. |
| 2026-07-24 | [r1.56.14](releases/2026-07-24_r1.56.14_web_ticket-order-failure-fix.md) | 티켓 구매 시 주문이 생성되지 않아 결제를 진행할 수 없던 문제를 수정했습니다. |
| 2026-07-23 | [r1.56.13](releases/2026-07-23_r1.56.13_web_artist-bio-sync-fix.md) | 프로필 설정에서 아티스트 소개를 수정해도 공개 명함(DROP)과 프로필에 옛 소개가 남아 있던 문제를 긴급 수정했습니다. |
| 2026-07-23 | [r1.56.12](releases/2026-07-23_r1.56.12_web_chat-message-edit.md) | 채팅에서 내가 보낸 메시지를 밀어서 수정할 수 있는 기능을 추가했습니다. |
| 2026-07-23 | [r1.56.11](releases/2026-07-23_r1.56.11_web_home-social-links.md) | 홈 화면의 소셜 바로가기가 MiSFY 공식 유튜브·인스타그램 계정으로 올바르게 연결되도록 수정했습니다. |
| 2026-07-23 | [r1.56.10](releases/2026-07-23_r1.56.10_web_staff-channel-monitoring.md) | 전체 채팅과 아티스트·공연장 채널에 새 메시지가 올라오면 스태프에게 알림이 전달되어 운영 대응이 더 빨라졌습니다. |
| 2026-07-23 | [r1.56.9](releases/2026-07-23_r1.56.9_web_artist-ranking-tiebreak.md) | 아티스트 랭킹에서 점수가 같은 경우, 실제 프로필 사진과 장르 정보를 갖춘 아티스트가 먼저 표시되도록 정렬을 개선했습니다. |
| 2026-07-23 | [r1.56.8](releases/2026-07-23_r1.56.8_web_announce-self-receive.md) | 공지를 보낸 스태프 본인도 알림을 받아 발송이 잘 되었는지 바로 확인할 수 있도록 개선했습니다. |
| 2026-07-22 | [r1.56.7](releases/2026-07-22_r1.56.7_web_app-update-detection.md) | 업데이트 배포 후에도 일부 기기에서 이전 화면이 계속 실행되던 문제를 수정하고, 새 버전 안내가 정상적으로 표시되도록 복구했습니다. |
| 2026-07-22 | [r1.56.6](releases/2026-07-22_r1.56.6_web_chat-composer-improvements.md) | 채팅에서 줄바꿈 입력, 길게 눌러 반응하기, 이모지 선택창 표시가 더 자연스럽게 동작하도록 개선했습니다. |
| 2026-07-22 | [r1.56.5](releases/2026-07-22_r1.56.5_web_staff-announce-broadcast.md) | 스태프가 채팅에서 '공지로 보내기'를 켜고 메시지를 보내면 아티스트·공연장·스태프 전원에게 알림이 발송됩니다. |
| 2026-07-22 | [r1.56.4](releases/2026-07-22_r1.56.4_web_chat-link-thumbnails.md) | 채팅에서 유튜브·사운드클라우드·틱톡 링크를 보내면 주소 대신 큰 썸네일 카드로 표시됩니다. |
| 2026-07-21 | [r1.56.3](releases/2026-07-21_r1.56.3_web_search-event-title-fix.md) | 검색 결과에서 공연 포스트 제목이 표시되지 않던 문제와 국가 필터가 올바르게 동작하지 않던 문제를 수정했습니다. |
| 2026-07-20 | [r1.56.2](releases/2026-07-20_r1.56.2_web_hardening-privacy.md) | 티켓 조회 시 개인정보 보호를 강화하고, 채팅 메시지 삭제가 모든 화면에 실시간으로 반영되도록 개선했습니다. |
| 2026-07-20 | [r1.56.1](releases/2026-07-20_r1.56.1_web_chat-translate-reactions.md) | 모든 채팅 화면에서 메시지를 번역해 보고, 이모지로 반응할 수 있는 기능을 추가했습니다. |
| 2026-07-20 | [r1.56.0](releases/2026-07-20_r1.56.0_web_together-v3-map-hub.md) | 함께 즐기기가 공연 지도와 하나로 통합되어, 지도에서 바로 모임을 찾고 공연 카드에서 곧장 모임을 만들거나 참여할 수 있게 되었습니다. |
| 2026-07-19 | [r1.55.42](releases/2026-07-19_r1.55.42_web_image-thumbnails.md) | 업로드된 이미지에 경량 썸네일을 자동 생성하고 목록·지도·홈 화면에 적용하여 앱 전반의 이미지 로딩 속도를 크게 개선했습니다. |
| 2026-07-17 | [r1.55.41](releases/2026-07-17_r1.55.41_web_chat-participants-avatars.md) | 전체 채팅 방 상단에서 지금 접속 중인 참여자들의 프로필 사진과 인원수를 한눈에 확인할 수 있게 되었습니다. |
| 2026-07-16 | [r1.55.40](releases/2026-07-16_r1.55.40_web_delete-reliability.md) | 구독자나 판매 이력이 있는 공연·공연장, 피드 글을 삭제할 때 오류로 실패하던 문제를 수정하고, 삭제할 수 없는 경우 이유를 명확히 안내하도록 개선했습니다. |
| 2026-07-16 | [r1.55.39](releases/2026-07-16_r1.55.39_web_ux-error-polish.md) | 공연장 이벤트 게스트리스트 오표시와 리뷰 제출 결과 안내를 바로잡고, 오류 상황에서의 안내를 전반적으로 개선했습니다. |
| 2026-07-15 | [r1.55.38](releases/2026-07-15_r1.55.38_web_paypal-copy-cleanup.md) | 결제·정산 화면에 남아 있던 사용하지 않는 결제 수단(PayPal) 표기를 정리하여 현재 지원하는 결제 수단 기준으로 안내를 통일했습니다. |
| 2026-07-15 | [r1.55.37](releases/2026-07-15_r1.55.37_web_ai-venue-map-markers.md) | 공연 지도에서 AI 수집 공연장도 마커로 표시되고, 상세 화면에서 배지로 구분할 수 있게 되었습니다. |
| 2026-07-15 | [r1.55.36](releases/2026-07-15_r1.55.36_web_together-polish.md) | 함께 즐기기 모임 목록에서 각 모임이 어떤 공연과 연결되어 있는지 한눈에 확인할 수 있도록 개선했습니다. |
| 2026-07-14 | [r1.55.35](releases/2026-07-14_r1.55.35_web_initial-bundle-chat-realtime.md) | 첫 접속 시 앱이 더 빠르게 열리고, 채팅이 새로고침 없이 실시간으로 반영되도록 개선했습니다. |
| 2026-07-14 | [r1.55.34](releases/2026-07-14_r1.55.34_web_map-home-payload-slim.md) | 공연 지도와 홈 화면이 불러오는 데이터 양을 대폭 줄여 화면이 훨씬 빠르게 열리도록 개선했습니다. |
| 2026-07-13 | [r1.55.33](releases/2026-07-13_r1.55.33_web_loading-speed-phase1.md) | 앱 첫 화면이 뜨는 속도를 크게 개선하고, 공연장 목록과 채팅의 데이터 처리를 가볍게 다듬었습니다. |
| 2026-07-13 | [r1.55.32](releases/2026-07-13_r1.55.32_web_intl-settlement-notice.md) | 해외(한국 외) 정산 등록을 일시적으로 중단하고, 2026년 9월 중 지원 예정임을 미리 안내하도록 했습니다. |
| 2026-07-13 | [r1.55.31](releases/2026-07-13_r1.55.31_web_feed-link-embeds.md) | 피드와 Today 게시글 본문에 적힌 링크가 자동으로 썸네일·영상 미리보기 카드로 표시됩니다. |
| 2026-07-13 | [r1.55.30](releases/2026-07-13_r1.55.30_web_notification-prompt-tap-fix.md) | 알림 허용 안내 창의 버튼이 눌리지 않던 문제를 수정했습니다. |
| 2026-07-12 | [r1.55.29](releases/2026-07-12_r1.55.29_web_admin-theme-color-editor.md) | 운영 관리자가 앱의 테마 색상을 직접 편집할 수 있는 관리 도구를 추가했습니다(현재 기본 색상은 그대로이며, 관리자가 값을 저장하기 전까지 사용자 화면은 변하지 않습니다). |
| 2026-07-11 | [r1.55.28](releases/2026-07-11_r1.55.28_web_legal-paypal-to-stripe.md) | 이용약관·개인정보 처리방침에서 더 이상 사용하지 않는 PayPal 관련 문구를 정리하고, 결제·정산 안내를 현재 수단(토스·Stripe)에 맞게 갱신했습니다. |
| 2026-07-11 | [r1.55.27](releases/2026-07-11_r1.55.27_web_paypal-retirement.md) | 결제 수단을 국내 토스·해외 Stripe로 일원화하고, 더 이상 사용하지 않는 PayPal 결제를 앱에서 전면 정리했습니다. |
| 2026-07-11 | [r1.55.26](releases/2026-07-11_r1.55.26_web_venue-edit-fields.md) | 공연장 정보 수정 화면에서 전화번호·웹사이트·수용 인원·운영 시간을 저장해도 반영되지 않던 문제를 수정했습니다. |
| 2026-07-11 | [r1.55.25](releases/2026-07-11_r1.55.25_web_payment-region-routing.md) | 티켓 결제 화면에서 결제사 선택 버튼을 없애고, 지역에 따라 결제 방식을 자동으로 정하도록 바꿨습니다. |
| 2026-07-11 | [r1.55.24](releases/2026-07-11_r1.55.24_web_admin-refund-approvals.md) | 운영 관리자가 앱에서 직접 티켓 환불을 승인·거절할 수 있는 화면을 추가했습니다. |
| 2026-07-10 | [r1.55.23](releases/2026-07-10_r1.55.23_web_partial-refund-fix.md) | 해외 티켓 부분 환불이 결제사에서는 처리됐으나 앱 기록이 갱신되지 않던 문제를 수정했습니다. |
| 2026-07-10 | [r1.55.22](releases/2026-07-10_r1.55.22_web_refund-request-feedback.md) | 티켓 환불 신청이 접수돼도 화면에 아무 안내가 없어 여러 번 눌리던 문제를 수정했습니다. |
| 2026-07-10 | [r1.55.21](releases/2026-07-10_r1.55.21_web_venue-event-edit.md) | 공연장 관리에서 등록한 공연의 수정 버튼이 동작하지 않던 문제를 수정했습니다. |
| 2026-07-10 | [r1.55.20](releases/2026-07-10_r1.55.20_web_intl-payment-stabilization.md) | 해외 티켓 결제에서 주문이 거절되거나 카드 입력 화면이 나타나지 않던 문제를 수정하고, 첫 해외 실결제(태국 바트)를 검증했습니다. |
| 2026-07-10 | [r1.55.19](releases/2026-07-10_r1.55.19_web_intl-stripe-ticket-payment.md) | 해외 공연 티켓을 현지 통화로 Stripe 카드 결제할 수 있게 했습니다. |
| 2026-07-09 | [r1.55.18](releases/2026-07-09_r1.55.18_web_admin-stripe-settlement.md) | 운영 스태프가 해외 정산 대상을 미리 확인하고 일괄 정산을 실행할 수 있는 관리자 콘솔을 추가했습니다. |
| 2026-07-09 | [r1.55.17](releases/2026-07-09_r1.55.17_web_deploy-stability.md) | 서비스 업데이트 직후 일부 브라우저에서 빈 화면이 나타날 수 있던 문제를 방지하도록 배포 방식을 개선했습니다. |
| 2026-07-09 | [r1.55.16](releases/2026-07-09_r1.55.16_web_global-payouts-groundwork.md) | 해외 아티스트·공연장 정산을 더 많은 국가로 확장하기 위한 기반을 준비했습니다(순차 활성화 예정). |
| 2026-07-09 | [r1.55.15](releases/2026-07-09_r1.55.15_web_paypal-surface-cleanup.md) | 결제 수단을 국내(Toss)/해외(Stripe)로 일원화하는 과정에서, 화면에 남아 있던 PayPal 관련 표시를 정리했습니다. |
| 2026-07-09 | [r1.55.14](releases/2026-07-09_r1.55.14_web_admin-venue-images.md) | 운영 스태프가 관리자 화면에서 공연장의 로고와 커버 이미지를 직접 등록·수정할 수 있습니다. |
| 2026-07-09 | [r1.55.13](releases/2026-07-09_r1.55.13_web_hangout-entry-on-map.md) | 함께 즐기기를 별도 화면 이동 없이 공연 지도 위에서 바로 시작할 수 있습니다. |
| 2026-07-09 | [r1.55.12](releases/2026-07-09_r1.55.12_web_payment-amount-simplify.md) | 결제 화면 상단의 중복 금액 카드를 없애고 금액을 결제 버튼에서 바로 확인하도록 정리해, 필수 동의가 한 화면에 보이게 했습니다. |
| 2026-07-09 | [r1.55.11](releases/2026-07-09_r1.55.11_web_collab-delete-hero-fallback.md) | 협업·모집 글 상세에서 작성자와 운영 스태프가 글을 삭제할 수 있고, 포스터가 없을 때 장르색 배경이 표시됩니다. |
| 2026-07-09 | [r1.55.10](releases/2026-07-09_r1.55.10_web_payment-selector-cleanup.md) | 티켓 결제 화면을 정리하고, 국내(Toss) 결제 시 필수 약관 동의 절차를 추가했습니다. 해외 결제 옵션은 준비 중입니다. |
| 2026-07-09 | [r1.55.9](releases/2026-07-09_r1.55.9_web_ticket-intl-phone.md) | 티켓 구매 정보 입력 화면에서 국가 번호를 선택해 해외 전화번호도 입력할 수 있게 했습니다. |
| 2026-07-09 | [r1.55.8](releases/2026-07-09_r1.55.8_web_collab-post-edit.md) | 작성자와 운영 스태프가 등록한 협업·모집 글을 나중에 수정할 수 있게 했습니다. |
| 2026-07-09 | [r1.55.7](releases/2026-07-09_r1.55.7_web_venue-profile-image-edit.md) | 공연장 관리자가 공연장 프로필 사진을 직접 올리고 수정할 수 있게 했습니다. |
| 2026-07-09 | [r1.55.6](releases/2026-07-09_r1.55.6_web_feed-story-rail-align.md) | 피드 상단 스토리 줄에서 새 게시물이 있는 항목과 없는 항목의 크기·정렬이 어긋나던 부분을 맞췄습니다. |
| 2026-07-09 | [r1.55.5](releases/2026-07-09_r1.55.5_web_map-layer-source-split.md) | 공연 지도의 상단 탭에서 '공연장'은 실제 등록된 공연장만, 'AI'는 AI로 수집한 공연장을 보여주도록 데이터 구분을 명확히 했습니다. |
| 2026-07-09 | [r1.55.4](releases/2026-07-09_r1.55.4_web_artist-youtube-preview.md) | 아티스트 프로필 음악 탭에 YouTube 채널 링크만 넣어도 최신 영상이 자동으로 재생 미리보기로 뜨도록 인식 범위를 넓혔습니다. |
| 2026-07-08 | [r1.55.3](releases/2026-07-08_r1.55.3_web_feed-ai-author-profile.md) | 피드에서 AI가 작성한 글의 작성자 프로필을 열 때 프로필을 불러오지 못하던 문제를 해결하고, 해당 프로필에서 AI 글이 함께 보이도록 했습니다. |
| 2026-07-08 | [r1.55.2](releases/2026-07-08_r1.55.2_web_feed-following-stories.md) | 피드 상단에 팔로우한 프로필과 추천 아티스트를 가로로 보여주는 스토리 레일을 추가하고, 새 글이 올라온 프로필은 링으로 눈에 띄게 표시합니다. |
| 2026-07-08 | [r1.55.1](releases/2026-07-08_r1.55.1_web_chat-link-preview.md) | 채팅 메시지 속 링크를 자동으로 눌러서 열 수 있게 하고, 링크의 제목·설명·이미지를 담은 미리보기 카드를 함께 보여줍니다. |
| 2026-07-08 | [r1.55.0](releases/2026-07-08_r1.55.0_web_chat-photo-attach.md) | 전체 채팅(채널)에서도 사진을 첨부해 보낼 수 있도록 했습니다. 그동안 개인 메시지에서만 가능하던 사진 전송을 커뮤니티 채팅으로 넓혔습니다. |
| 2026-06-25 | [r1.54.12](releases/2026-06-25_r1.54.12_web_venue-photo-ai-fallback.md) | 공연장 사진이 없을 때 빈 화면 대신 AI 포스터나 아바타 이미지로 자연스럽게 대체 표시되도록 해, 어떤 공연장이든 보기 좋은 화면을 보여줍니다. |
| 2026-06-25 | [r1.54.11](releases/2026-06-25_r1.54.11_web_pull-to-refresh.md) | 메인 탭에서 화면을 아래로 당겨서 새로고침하는 기능을 지원해, 최신 콘텐츠를 더 쉽게 불러올 수 있도록 했습니다. |
| 2026-06-25 | [r1.54.10](releases/2026-06-25_r1.54.10_web_guest-list-checkin-tabs.md) | 게스트리스트 관리 화면을 입장 전과 입장 완료로 구분한 탭으로 개편해, 행사 현장에서 입장 현황을 더 빠르게 파악할 수 있도록 했습니다. |
| 2026-06-25 | [r1.54.9](releases/2026-06-25_r1.54.9_web_map-source-toggle.md) | 공연 지도에서 아티스트 소스와 AI 수집 소스를 토글로 구분해 볼 수 있게 했습니다. |
| 2026-06-25 | [r1.54.8](releases/2026-06-25_r1.54.8_web_map-artist-profiles.md) | 공연 지도와 목록에 표시되는 AI 수집 아티스트를 실제 아티스트 프로필 기반으로 개편했습니다. 핀이나 행을 누르면 해당 아티스트의 상세 정보와 공연 목록을 함께 볼 수 있습니다. |
| 2026-06-24 | [r1.54.13](releases/2026-06-24_r1.54.13_web_android-app-links-verification.md) | 외부에서 공유한 공연 링크를 Android 앱에서 열면 브라우저를 거치지 않고 앱이 바로 열리도록 앱 링크 검증을 추가했습니다. |
| 2026-06-22 | [r1.54.3](releases/2026-06-22_r1.54.3_web_map-blank-cache-recovery.md) | 일부 기기에서 공연 지도가 빈 화면으로 표시되던 문제를 지도 데이터 캐시 자동 복구로 해소했습니다. |
| 2026-06-22 | [r1.54.2](releases/2026-06-22_r1.54.2_web_event-like-guest-artist.md) | 이벤트 상세에서 좋아요 상태가 유지되도록 수정하고 게스트 아티스트 표시 동작을 개선했습니다. |
| 2026-06-21 | [r1.54.1](releases/2026-06-21_r1.54.1_web_music-links-external-i18n.md) | 아티스트 음악 링크에 외부 열기 버튼을 추가하고 입력 오류 메시지를 다국어로 제공하는 등 음악 링크의 표시와 저장 경험을 개선했습니다. |
| 2026-06-20 | [r1.54.0](releases/2026-06-20_r1.54.0_web_event-cohost.md) | 공연에 공동 주최자를 초대해 함께 관리할 수 있는 기능을 추가했습니다. |
| 2026-06-20 | [r1.53.17](releases/2026-06-20_r1.53.17_web_shared-link-app-deeplink.md) | 공유한 공연 링크를 앱에서 열면 해당 공연이 바로 보이도록 수정했습니다. |
| 2026-06-20 | [r1.53.16](releases/2026-06-20_r1.53.16_web_artist-lineup.md) | 공연을 등록할 때 출연 아티스트(라인업)를 검색해 추가할 수 있게 했습니다. |
| 2026-06-20 | [r1.53.15](releases/2026-06-20_r1.53.15_web_staff-event-highlight.md) | 운영진이 직접 올린 공연이 앱에서 눈에 띄게 강조되도록 했습니다. |
| 2026-06-18 | [r1.53.12](releases/2026-06-18_r1.53.12_web_beta-tester-signup-page.md) | 안드로이드 비공개 베타 테스터를 모집하는 신청 페이지를 추가했습니다. |
| 2026-06-18 | [r1.53.11](releases/2026-06-18_r1.53.11_web_account-deletion-page.md) | 계정과 데이터 삭제 방법을 안내하는 공개 페이지를 추가했습니다. |
| 2026-06-18 | [r1.53.10](releases/2026-06-18_r1.53.10_web_ticket-organizer-name-snapshot.md) | 공연 주최자 계정이 삭제되어도, 구매한 티켓에 구매 당시의 주최자 이름이 그대로 표시되도록 했습니다. |
| 2026-06-16 | [r1.53.8](releases/2026-06-16_r1.53.8_web_profile-photo-edit-touch.md) | 프로필 사진 편집 화면에서 사진을 손가락으로 움직이거나 확대·축소할 수 없고, 완료를 눌러도 저장되지 않던 문제를 해결했습니다. |
| 2026-06-16 | [r1.53.7](releases/2026-06-16_r1.53.7_web_profile-photo-quality.md) | 프로필 사진을 더 높은 화질로 저장하도록 개선해, 아티스트·리스너 프로필 카드의 큰 배경 이미지가 또렷하게 보입니다. |
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
| 2026-06-22 | [r1.54.5](releases/2026-06-22_r1.54.5_backend_rank-promotion-authz-hardening.md) | 등급 승격 권한 검증을 강화해 잘못된 자가 승격을 방지했습니다. |
| 2026-06-22 | [r1.54.4](releases/2026-06-22_r1.54.4_backend_curation-feed-publish-date-sort.md) | 큐레이션 피드를 발행일 기준으로 정렬해 최신 콘텐츠가 먼저 보이도록 개선했습니다. |
| 2026-06-16 | [r1.53.9](releases/2026-06-16_r1.53.9_backend_artist-rank-profile-fields.md) | 아티스트 등업이 승인된 뒤에도 프로필에 장르가 "기타"로 보이거나 자기소개가 비어 있던 문제를 해결해, 등업 신청 시 입력한 정보가 프로필에 그대로 반영되도록 했습니다. |
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
| 2026-06-23 | [r1.54.7](releases/2026-06-23_r1.54.7_data-pipeline_ai-model-update.md) | 공연 정보 분석과 검색에 사용되는 AI 모델을 업데이트해 안정성을 높였습니다. |
| 2026-06-12 | [r1.53.3](releases/2026-06-12_r1.53.3_data-pipeline_today-card-images.md) | Today 화면의 추천 공연 카드에서 일부 이미지가 보이지 않던 문제를 해결해, 공연 이미지가 정상적으로 표시되도록 했습니다. |
| 2026-06-07 | [r1.52.12](releases/2026-06-07_r1.52.12_data-pipeline_map-data-quality.md) | 공연 지도에 잘못 수집되거나 잘못된 위치에 표시되던 항목을 정리하고, 앞으로 더 정확한 공연 정보만 노출되도록 데이터 품질을 개선했습니다. |
| 2026-06-06 | [r1.52.10](releases/2026-06-06_r1.52.10_data-pipeline_ai-event-geocode-enrichment.md) | AI로 수집된 공연이 지도에 올바른 위치로 표시되도록 위치 정보를 보강하고, 매일 진행되는 데이터 정리 과정을 더 빠르고 안정적으로 개선했습니다. |

### Operations

| Date | Version | Summary |
|---|---|---|
| 2026-06-24 | [r1.54.6](releases/2026-06-24_r1.54.6_operations_admin-member-profile-edit.md) | 관리 도구에 회원 통합 프로필 편집 기능을 추가하고, 아티스트 소개와 SNS 정보 저장이 제대로 반영되도록 관리 기능을 개선했습니다. 운영자 전용 기능입니다. |
| 2026-06-17 | [r1.53.14](releases/2026-06-17_r1.53.14_operations_admin-member-pagination.md) | 관리 도구의 회원 목록에서 전체 회원을 페이지로 나눠 보고, 등급별로 빠르게 필터링할 수 있도록 개선했습니다. |
| 2026-06-17 | [r1.53.13](releases/2026-06-17_r1.53.13_operations_admin-member-grade-change.md) | 관리 도구의 회원 관리에서 회원의 등급을 직접 변경할 수 있는 기능을 추가했습니다. |
| 2026-06-12 | [r1.53.4](releases/2026-06-12_r1.53.4_operations_artist-hide-public-surface.md) | 관리 도구에서 아티스트를 숨김 처리하면 공개 화면에 곧바로 반영되도록 개선했습니다. |
| 2026-06-12 | [release-assistant-v0.1](releases/2026-06-12_release-assistant-v0.1_operations_ios-release-assistant-open-source.md) | iOS 앱 출시 준비를 단계별로 도와주는 iOS Release Assistant를 오픈소스 도구로 정리하고, 초보자도 따라갈 수 있도록 문서를 보강했습니다. |
| 2026-06-09 | [r1.53.2](releases/2026-06-09_r1.53.2_operations_report-notification-routing.md) | POMFS 운영 보고와 자동 알림 메일의 기본 수신 경로를 정리해, 중요한 운영 알림이 한 곳으로 모이도록 개선했습니다. |
| 2026-06-09 | [release-history-v4](releases/2026-06-09_release-history-v4_operations_public-release-history-sanitized-refresh.md) | 공개 릴리즈 히스토리를 정제해 내부 개발 로그성 항목을 제거하고, 실제 사용자에게 설명할 수 있는 변경 이력 중심으로 다시 정리했습니다. |
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
- Android
- Web
- Backend
- Data Pipeline
- Operations
- Monthly archive
