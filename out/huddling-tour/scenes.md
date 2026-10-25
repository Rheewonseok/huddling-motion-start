# scenes — huddling-tour

30초 = 900f (30fps, 1920×1080) · 화면 5장 `src/screens/01-home` → `05-assets` + BRIEF 부품
뼈대 B (Nafa) · 카메라 A (Device Rise). 문구는 화면 PNG · 부품 HTML에 있는 글자만 쓴다. 움직임 성격은 motion.md 그대로(반동 없음), 역동성은 비트 밀도 · 연속 이음 · 카메라로 낸다.
세 안 공통: 새 장면 간격은 R2 기준(`motion-enter` + `hold-line` 안쪽, N7), 정지는 `hold-line`을 넘지 않음(R3). 오래 머무는 곳은 엔딩 `hold-screen` 한 번뿐. 정해진 값 N1 · N3 · N4 · N5 · N6은 해당 비트가 있으면 그대로 쓴다.

## 1차: 3안 요약 (하나를 고른다)

### 안 A — 화면 사슬 중심 "다섯 화면이 한 번도 끊기지 않는다"
- 콘셉트: 짧은 글줄 "오늘도 하나씩, 내 실력으로"(단어마다 `motion-pop`) → 폰 `camera-rise`로 `01-home` → 검색창으로 `camera-match-zoom`, "자동화" 타이핑(`motion-tick`, PNG 안내 문구는 N5처럼 `video-card` 면으로 가림) → `camera-pull-out`으로 `02-skills`, 스킬 카드 3장 빠른 간격으로 안착 → 칩 "자동화"가 점으로 줄고(`motion-swap`) 점이 선을 그어 `mission-card` 진행 바가 됨(`motion-travel`) → 빠져나오면 `03-mission` → 한 번에 스크롤(`motion-enter`) → 컷, `button-submit` 단독(×2.8)이 옆에서 들어와 채움 → 컷, `04-approved` 내용 페이드 · 배지 `motion-pop` · `camera-push`(기준점 배지 · "미션을 완성했어요!") → 컷, `05-assets` `stat-card` 금액 바뀜 · `asset-card` 상태 `motion-swap` → `asset-card`가 `camera-wipe` → 엔딩(`logo` white + "배움이 쌓여, 나의 자산으로", `hold-screen`).
- 뼈대: B 00:00–00:24 5단 흐름 중 2단(f84→375 화면 사슬)을 영상의 절반 이상으로 늘림. 컷은 B처럼 세 번(버튼 단독 · 결과 화면 · 05 화면)만. 카메라 A는 첫 폰 등장 한 번.
- 화면 · 부품: `src/screens/01-home.png` · `02-skills.png` · `03-mission.png` · `04-approved.png` · `05-assets.png`(폰 안 ×1) · `src/parts/skill-card-1~3.html`(×1) · `src/parts/mission-card.html`(×1, 진행 바) · `src/parts/button-submit.html`(`submit` ×2.8 단독) · `src/parts/badge-approved.html`(×1) · `src/parts/stat-card.html`(×1) · `src/parts/asset-card.html`(×1, `private-image` → `review` → `selling`) · 엔딩 `src/parts/logo.html`(`logotype-white` ×2.8).
- 반영: R1 R2 R3 R4 R5 R6 R7 R8 R9 R10 R11 R12(일부: 카드가 목록 자리로 안착) R13 R14 R15 R16 R17 R19 R20 R22 — **반영 20/22** (R18 강조 단어 · R21 이름 롤 안 씀). R4는 push 뒤 바로 wipe 대신 05 화면을 거쳐 wipe.
- 쓰게 되는 새 후보: N7 · N8 · N9 · N10 · N11 (N2 안 씀). 타이핑 자리 가리기는 N5 방식 응용이라 2차에서 확인.

### 안 B — 부품 클로즈업 중심 "부품이 다음 부품이 된다"
- 콘셉트: 대부분 폰 없이 `video-bg` 위 부품 ×2.8 단독. 화면은 부품이 `camera-pull-out`으로 빠져나올 때 잠깐씩 "이 부품이 여기 있다"로만 보임. `01-home` `camera-rise` → 스킬 행으로 `camera-match-zoom` → `skill-card-1` 단독, `-2` · `-3`이 빠른 간격으로 쌓임 → pull-out `02-skills` → match-zoom → `mission-card` 단독, 진행 바 채움("50% · 2/4 단계 완료") → 카드 안 버튼(`apply-case`)이 `button-submit` 단독으로 커지고 `motion-swap`으로 `submit` "제출하기" → 채움 → 같은 자리에서 `badge-approved` 단독 `motion-pop` → pull-out `04-approved`, `camera-push` → `stat-card` 단독 금액 바뀜 → `asset-card` 단독 상태 4개 연속 `motion-swap` → pull-out `05-assets` → `asset-card` `camera-wipe` → 엔딩(`brand-icon` + "배움이 쌓여, 나의 자산으로").
- 뼈대: B 00:05–00:06 검색창 단독 → 점 → 그래프 → 상세(match zoom · pull-out 왕복)와 B 00:12–00:16 버튼 단독 → 완료 비트를 영상 전체의 기본 단위로 반복. 글줄 도입 · 롤 없음.
- 화면 · 부품: `src/screens/01-home.png` · `02-skills.png` · `04-approved.png` · `05-assets.png`(폰 안 ×1, 짧게) · `03-mission.png`(match-zoom 출발점으로만) · `src/parts/skill-card-1~3.html` · `mission-card.html` · `button-submit.html`(`apply-case` → `submit`) · `badge-approved.html` · `stat-card.html` · `asset-card.html`(4상태 모두) — 모두 ×2.8 단독 ↔ 폰 안 ×1 · 엔딩 `src/parts/brand-icon.html`.
- 반영: R1(일부) R2 R3 R4 R5 R6 R7 R8 R9 R10 R11 R12 R13 R15 R16 R20 R22 — **반영 17/22** (R14 스크롤 · R17 R18 글줄 · R19 타이핑 · R21 롤 안 씀).
- 쓰게 되는 새 후보: N7 · N8(이 안의 중심, 부품마다 크기 정해야 함) · N9 · N10 · N11. ×2.8 단독 ↔ ×1 폰 안을 오가는 pull-out · match-zoom 배율은 `video-scale` 값이라 새 숫자는 아님.

### 안 C — 글자 · 롤 중심 "화면마다 한 문장, 끝은 이름 롤"
- 콘셉트: `video-bg` 위 글줄이 주인공이고, 폰은 문장 사이에 짧게 디졸브로 바뀌며 증거로만 나옴. 화면 PNG의 제목 문장을 순서대로 씀: "오늘도 하나씩, 내 실력으로"(단어마다 `motion-pop`) → 강조 단어 "실력으로"만 크게(N2), 아래로 `skill-card-1~3`(×1)이 빠른 간격으로 날아와 쌓임 → 폰 솟아오름, 카드들이 `02-skills` 목록 자리로 들어감 → "일에 바로 적용하는 AI" 타이핑(`motion-tick`) → `03-mission` · "반복 업무를 줄이는 AI 자동화" → `04-approved` · "미션을 완성했어요!"(accent "완성했어요!") → `05-assets` `stat-card` 금액 바뀜 → `camera-wipe` → 검은 면 롤: 위 고정 "배움이 쌓여, 나의 자산으로", 아래 줄이 스킬 3개 → 자산 4개 이름으로 점점 빨리 굴러감 → 엔딩(`logo` white + `brand-icon`).
- 뼈대: B 00:00–00:03 글줄 도입 · 강조 단어 · 물체 날아듦과 B 00:16–00:22 이름 롤 · 엔딩을 키우고, 화면 사슬은 디졸브(R14) 위주로 줄임. 카메라는 rise 한 번 외에 고정.
- 화면 · 부품: `src/screens/01-home.png`~`05-assets.png`(폰 안 ×1, 짧게) · `src/parts/skill-card-1~3.html`(×1 날아듦) · `src/parts/stat-card.html`(×1) · `src/parts/asset-card.html`(롤 문구 출처: 4상태 제목) · 엔딩 `src/parts/logo.html`(`logotype-white`) · `src/parts/brand-icon.html`. `mission-card` · `button-submit` · `badge-approved`는 화면 PNG 안 그대로(따로 움직이지 않음).
- 반영: R1 R2 R3 R5 R8 R12 R14 R16 R17 R18 R19 R20 R21 R22 — **반영 14/22** (R4 R7 R11 완료 비트 · push, R6 부품 단독, R9 R10 R13 R15 부품 이음 안 씀).
- 쓰게 되는 새 후보: N2 · N7 · N10 · N11 (N8 · N9 안 씀). 롤 문구 7줄은 B의 16줄보다 짧아 롤 간격(`hold-beat`에서 줄임)은 2차에서 토큰 안에서 맞춤.

---

## 2차: 장면표

**고른 안: A** (화면 사슬 중심, 승인 1)

- 표기: `시작f–끝f`에서 끝f는 다음 비트의 시작f다(끝f 미포함). 비트 길이 = 끝f − 시작f. 괄호 안 f는 비트 안 세부 시점.
- 바탕: 비트 1–17은 `video-bg`, 비트 18–19는 `video-end-bg`. 폰은 N1(390×844 전체를 1080 안 세로 가운데), 화면 뒤 `video-phone-bg`, 가장자리 `video-phone-line`, 그림자 `video-phone-shadow`, 베젤 없이 직각(`docs/video.md` 4장).
- 폰 안 부품은 ×1, 단독 부품은 ×2.8(`video-scale`) + 그림자 `Shadow/md`(`docs/video.md` 5장). 폰 안 글자는 최소 크기 규칙에서 빠진다(1장). 폰 밖 글자는 모두 `video-eyebrow` 이상.
- 카메라 클로즈업 배율은 N8(a) `video-scale` ×2.8 기준으로 적었다(폰 안 ×1 글자가 클로즈업에서 3장 토큰 크기와 같아짐).
- 위치값(PNG @2x 실측 ÷ 2 = @1x, 폰 화면 왼쪽 위 기준)은 표 아래 "위치값"에 모았다.

**1차 요약에서 바뀐 점** (사용자 확인 필요)
1. **R14 넣음**: 스크롤은 뺐다. 화면 5장 모두 390×844 한 장이라 N1(전체 보임)에서는 스크롤할 아래쪽이 없다. 대신 `01-home` → `02-skills`를 폰 자리 그대로 디졸브한다(두 화면의 검색창 · 칩 줄이 같은 자리에 있어서 그 부분은 그대로 남고 둘레만 바뀜). 03의 "한 번에 스크롤"은 지웠다.
2. **길이 채우기**: 요약 그대로는 약 560f라, 정지 상한(`hold-line`)을 지키며 900f를 채우려고 (a) 글줄 도입에 강조 단어 줄(R18, N2), (b) wipe 뒤 검은 면 이름 롤(R21), (c) 01 미션 카드 진행 바 채움, (d) 03 입력칸 타이핑("회의록 정리에 드는 시간을 줄였어요", PNG 예시 문구)을 넣었다.
3. 검색어는 "자동화" → **"AI 자동화"**(01 · 03 PNG · `mission-card` 제목 둘째 줄). 다음 장면이 그 미션 카드 진행 바라 이어짐이 맞고, 프레임 합도 맞는다. 점이 되는 것은 칩 대신 **검색창**(R13 그대로).
4. 버튼은 채운 뒤 `view-assets` "내 자산에서 보기"로 바뀌고 `camera-pull-out`으로 `04-approved`의 같은 버튼이 된다(컷 대신 부품 → 다음 장면). 컷은 B처럼 세 번: 03 → 버튼 단독(394) · 04 → 05(553) · wipe → 검은 면(671).
5. 엔딩 보조 줄은 "오늘도 하나씩, 내 실력으로"(도입 문구로 마무리). "배움이 쌓여, 나의 자산으로"는 롤의 위 고정 줄로 옮겼다.

| 비트 | 시작f–끝f | 화면 · 부품(src 경로) | 글자(문구 · video.md 3장 토큰) | 움직임(motion.md 2 · 3장 토큰) | 머무는 시간(motion.md 4장) | 카메라(motion.md 5장) | reference 번호 |
|---|---|---|---|---|---|---|---|
| 1 글줄 | 0–27 (27f) | 없음. 빈 `video-bg`, 프레임 가운데 위쪽 한 줄 | "오늘도 하나씩," · 크기 N2(아래) · `video-text` | 단어 2개("오늘도"(0–6) · "하나씩,"(9–15))마다 `motion-pop`, 간격 `duration-9` | `hold-beat` (15–27) | 고정 | R17 R1 R3 |
| 2 강조 단어 줄 | 27–60 (33f) | 없음. 같은 자리 | "내 실력으로" · `video-display` · `video-text`, "실력으로"만 `video-accent` | 앞 줄을 같은 자리에서 한 번에 바꿔 씀 `motion-swap`(27–36) | `hold-line` (36–60) | 고정 | R18 R17 |
| 3 폰 솟아오름 | 60–111 (51f) | `src/screens/01-home.png`(폰 안 ×1) + `src/parts/mission-card.html`(×1, PNG 미션 카드 자리에 겹침, 진행 바 `--progress` 0에서 시작) | 비트 2 글줄 퇴장. 폰 안 PNG 문구 | 글줄 2: 같은 자리에서 옅어져 퇴장 `motion-swap`(60–69, 폰이 솟는 동안) | `hold-breath` (105–111) | `camera-rise`(60–105, N4 600px) | R8 R5 R1 |
| 4 진행 바 채움 | 111–153 (42f) | `src/parts/mission-card.html` 진행 바 `#mission-card-progress-fill`(폰 안 ×1) | 폰 안 문구만. "50% · 2/4 단계 완료"는 부품 글자 그대로(바뀌지 않음) | 진행 바 0 → 0.5(부품 기본값) `motion-travel`(111–129) | `hold-line` (129–153) | 고정 | R8 R3 |
| 5 화면 디졸브 | 153–162 (9f) | `01-home.png` → `src/screens/02-skills.png`(폰 자리 그대로). 02의 스킬 3행 자리는 `video-card` 면으로 가려 비워 둠(N5 방식) | 폰 안 PNG 문구만. 검색창 · 칩 줄은 두 화면이 같은 자리라 그대로 남음 | `screens` 화면 바꿈 `motion-swap`(겹친 `mission-card`도 01과 함께 옅어짐) | 없음 | 고정 | R14(디졸브만) R5 R1 |
| 6 스킬 카드 안착 | 162–210 (48f) | `src/parts/skill-card-1.html` · `-2` · `-3`(폰 안 ×1, 02 PNG 스킬 행 자리) | 부품 안 글자: "회의록을 실행 목록으로" · "자료를 비교표로 정리하기" · "반복 메일, 자동으로 답장하기" 등 | 한 장씩 `motion-enter`(162 · 168 · 174 시작), 간격 N10(a) `duration-6`, 들어오는 모양 N12 | `hold-line` (186–210) | 고정 | R12 R2 |
| 7 검색창 클로즈업 · 타이핑 | 210–252 (42f) | `02-skills.png` 검색창 (폰 안 ×1, 카메라 ×2.8. 폰 가장자리 · 둘레 내용은 보임). PNG 안내 문구 자리를 면으로 가림(면 색 N13) | "AI 자동화" · 폰 안 `Text/body`(클로즈업에서 `video-body` 크기) · `video-text`. 커서 없음 | 글자 5개("A" 220 · "I" 224 · "자" 228 · "동" 232 · "화" 236)마다 `motion-tick`, 간격 `duration-4`(띄어쓰기는 "자"와 함께) | `hold-breath`(214–220, 빈 검색창) · `hold-beat`(240–252) | `camera-match-zoom`(210–214, 검색창으로) | R9 R19 R6(일부) R3 |
| 8 검색창 → 점 → 선 | 252–279 (27f) | 검색창이 `src/parts/mission-card.html`의 `#mission-card-progress-fill`이 됨(카메라 ×2.8 그대로) | 없음 (02의 나머지 내용은 옅어져 폰 면 `video-card`만 남음) | 검색창이 옅어지며 알약 → 점으로 줄고 진행 바 왼쪽 끝 자리로 감 `motion-swap`(252–261, 02 둘레 내용 퇴장도 같이) → 점에서 진행 바가 0 → 0.5로 그어짐 `motion-travel`(261–279) | 없음 | 고정 | R13 R1 |
| 9 03 화면으로 빠짐 | 279–312 (33f) | `src/screens/03-mission.png`(폰 안 ×1). 그어진 선이 03 미션 카드 진행 바 자리에 놓임 | 폰 안 PNG 문구만 | 선 둘레로 03 화면 내용 페이드 인 `motion-swap`(279–288) | `hold-line` (288–312) | `camera-pull-out`(279–285, ×2.8 → ×1) | R10 R1 R5 |
| 10 입력칸 클로즈업 · 타이핑 | 312–394 (82f) | `03-mission.png` "어떻게 활용했나요?" 입력칸 (폰 안 ×1, 카메라 ×2.8). 안내 문구 두 줄 자리를 면으로 가림(면 색 N13). "어떻게 활용했나요?"는 그대로 | "회의록 정리에 드는 시간을 줄였어요" (PNG 예시 줄에서 "예:" · 마침표 뺌) · 폰 안 `Text/body`(클로즈업에서 `video-body` 크기) · `video-text`. 커서 없음 | 글자 15개마다 `motion-tick`(322–382), 간격 `duration-4`, 띄어쓰기는 다음 글자와 함께 | `hold-breath`(316–322, 빈 입력칸) · `hold-beat`(382–394) | `camera-match-zoom`(312–316, 입력칸으로) | R19 R20(입력 부분) R9 R3 |
| 11 버튼 단독 | 394–457 (63f) | 컷. `src/parts/button-submit.html` `data-state="submit"` → `view-assets`, ×2.8 단독 · `video-bg` | "제출하기" → "내 자산에서 보기" · 부품 안 `Text/label`(×2.8 = `video-label`) | 오른쪽 프레임 밖에서 미끄러져 들어와 가운데 안착 `motion-travel`(394–412) → 왼쪽부터 채움 `motion-travel`·`curve-linear`(418–436, 채움 색 N14) → 문구 `motion-swap`(436–445) | `hold-breath`(412–418) · `hold-beat`(445–457) | 고정 | R15 R6 R2 |
| 12 04 화면으로 빠짐 | 457–472 (15f) | `button-submit`(`view-assets`)이 `src/screens/04-approved.png`의 같은 버튼 자리(폰 안 ×1)가 됨. 폰 면은 처음엔 `video-card`만 → 04 내용 페이드. 배지 자리는 `video-card` 면으로 가림(N5) | 폰 안 PNG 문구만 | 빈 폰 화면 위로 04 내용 페이드 인 `motion-swap`(463–472) | 없음 | `camera-pull-out`(457–463, ×2.8 → ×1) | R4 R10 R15(결과 페이드) |
| 13 배지 등장 | 472–484 (12f) | `src/parts/badge-approved.html`(폰 안 ×1, PNG 배지 자리) | "승인 완료" (부품 안 글자) | 작게 시작해 커지며 등장 `motion-pop`(N3 `scale 0.8 → 1.0`) | `hold-breath` (478–484) | 고정 | R4 R2 |
| 14 밀고 들어감 | 484–553 (69f) | `04-approved.png` + `badge-approved.html`(폰 안 ×1) | 클로즈업에 "승인 완료" · "미션을 완성했어요!" · "결과물이 승인되어 내 자산에 등록됐어요." 묶음이 프레임 위쪽 (폰 안 글자) | 없음 (카메라만) | `hold-line` (529–553) | `camera-push`(484–529, 배율 · 기준점 N9: 기준점은 배지 · 제목 묶음) | R7 R11 R4 |
| 15 05 화면 · 금액 | 553–595 (42f) | 컷. `src/screens/05-assets.png`(폰 안 ×1) + `src/parts/stat-card.html`(×1, PNG 수익 카드 자리에 겹침) | "이번 달 수익 ₩29,700" · "전체 4개 / 검수 중 1개 / 판매 중 1개" (부품 안 글자). 바뀌는 것은 `#stat-card-amount`뿐 | 금액 자리마다 `motion-tick`, 전체 N11(a) `duration-18`(553–571)로 `data-final` 29,700에 정착 | `hold-line` (571–595) | 고정 | R20 R5 R1 |
| 16 자산 카드 단독 · 상태 | 595–665 (70f) | `05-assets.png` 첫 자산 카드 → `src/parts/asset-card.html` ×2.8 단독 · `video-bg`(줌 4f 안에서 바뀜). `data-state` `private-image` → `review` → `selling` | "회의록 자동 정리 템플릿 · 비공개 · 나만 볼 수 있어요" → "리서치 비교표 템플릿 · 멤버 공개 · 판매 검수 중" → "업무 자동화 체크리스트 · 멤버 공개 · 판매 중 · ₩9,900" · 부품 안 `Text/list-title` · `Text/caption`(×2.8 = `video-list` · `video-caption`) | 상태 바뀜 `motion-swap` 두 번(611–620 · 632–641) | `hold-beat`(599–611) · `hold-beat`(620–632) · `hold-line`(641–665) | `camera-match-zoom`(595–599, 첫 자산 카드로) | R9 R6 R2 R3 |
| 17 카드가 덮음 | 665–671 (6f) | `asset-card.html`(`selling`, 커져서 프레임을 덮음) | 없음 | 없음 (카메라만) | 없음 (덮은 순간 671에서 컷) | `camera-wipe`(N6: 커지는 동안 `video-end-bg`로 바뀜) | R16 R4 R1 |
| 18 이름 롤 | 671–816 (145f) | 없음. `video-end-bg` 가운데 두 줄(줄 사이 `space-section` × `video-scale`) | 위 고정: "배움이 쌓여, 나의 자산으로" · `video-heading` · `video-end-text`. 아래 롤 9개: "회의록을 실행 목록으로" → "자료를 비교표로 정리하기" → "반복 메일, 자동으로 답장하기" → "반복 업무를 줄이는 AI 자동화" → "자동화_적용사례_v1.pdf" → "회의록 자동 정리 템플릿" → "리서치 비교표 템플릿" → "주간 보고서 작성 도우미" → "업무 자동화 체크리스트" · `video-section` · `video-end-text` | 위 줄 `motion-pop`(671–677) → 아래 첫 이름 `motion-pop`(683–689) → 세로로 한 칸씩 8번 `motion-tick`(701 · 716 · 730 · 743 · 755 · 766 · 777 · 788 시작) | `hold-breath`(677–683) · 롤 사이 머무름 12에서 7까지 줄임(N15) · 마지막 `hold-line`(792–816) | 고정 | R21 R1 R3 |
| 19 엔딩 | 816–900 (84f) | `src/parts/logo.html` `data-state="logotype-white"` ×2.8 단독 · `video-end-bg` | 로고 아래 보조 줄 "오늘도 하나씩, 내 실력으로" · `video-heading` · `video-end-text` (로고와 줄 사이 `space-section` × `video-scale`) | 롤 두 줄 어두워지며 퇴장 `motion-pop`·`curve-in`(816–822) → 로고 `motion-pop`(828–834) → 보조 줄 `motion-pop`(834–840) | `hold-breath`(822–828) · `hold-screen`(840–900) | 고정 | R22 R1 R3 |

### 길이 내역 (모두 motion.md 토큰의 합. 합계 900f = 30s × 30f)

| 비트 | 길이 | 토큰 합 |
|---|---|---|
| 1 | 27 | 간격 `duration-9` (9) + `motion-pop` 6 + `hold-beat` 12 |
| 2 | 33 | `motion-swap` 9 + `hold-line` 24 |
| 3 | 51 | `camera-rise` 45 + `hold-breath` 6 (글줄 퇴장 `motion-swap` 9는 rise와 겹침) |
| 4 | 42 | `motion-travel` 18 + `hold-line` 24 |
| 5 | 9 | `motion-swap` 9 |
| 6 | 48 | 간격 `duration-6` ×2 (12, N10 a) + `motion-enter` 12 + `hold-line` 24 |
| 7 | 42 | `camera-match-zoom` 4 + `hold-breath` 6 + 간격 `duration-4` ×4 (16) + `motion-tick` 4 + `hold-beat` 12 |
| 8 | 27 | `motion-swap` 9 + `motion-travel` 18 |
| 9 | 33 | `motion-swap` 9 (`camera-pull-out` 6은 그 안에 겹침) + `hold-line` 24 |
| 10 | 82 | `camera-match-zoom` 4 + `hold-breath` 6 + 간격 `duration-4` ×14 (56) + `motion-tick` 4 + `hold-beat` 12 |
| 11 | 63 | `motion-travel` 18 + `hold-breath` 6 + `motion-travel`(`curve-linear`) 18 + `motion-swap` 9 + `hold-beat` 12 |
| 12 | 15 | `camera-pull-out` 6 + `motion-swap` 9 |
| 13 | 12 | `motion-pop` 6 + `hold-breath` 6 |
| 14 | 69 | `camera-push` 45 + `hold-line` 24 |
| 15 | 42 | `duration-18` (18, N11 a) + `hold-line` 24 |
| 16 | 70 | `camera-match-zoom` 4 + `hold-beat` 12 + `motion-swap` 9 + `hold-beat` 12 + `motion-swap` 9 + `hold-line` 24 |
| 17 | 6 | `camera-wipe` 6 |
| 18 | 145 | `motion-pop` 6 + `hold-breath` 6 + `motion-pop` 6 + `motion-tick` ×8 (32) + 롤 머무름 12 · 11 · 10 · 9 · 8 · 7 · 7 · 7 (71, motion.md 4장 규칙 · N15 a) + `hold-line` 24 |
| 19 | 84 | `motion-pop`(`curve-in`) 6 + `hold-breath` 6 + `motion-pop` 6 + `motion-pop` 6 + `hold-screen` 60 |
| 합 | **900** | |

구간 비율(R1 대조): 글줄 도입 0–60 (7%, B 12%) · 화면 사슬 60–394 (37%, B 40%) · 부품 클로즈업 · 완료 394–671 (31%, B 15%) · 검은 면 롤 671–816 (16%, B 22%) · 엔딩 816–900 (9%, B 10%).

**역동성 점검** (N7 대조)
- 정지(아무것도 안 움직임) 최대 `hold-line` 24f. 넘는 곳은 엔딩 `hold-screen` 한 번(840–900).
- 새 요소 · 화면 · 카메라 시작 시점: 0 · 9 · 27 · 60 · 111 · 153 · 162 · 168 · 174 · 210 · 220 · 252 · 261 · 279 · 312 · 322 · 394 · 418 · 436 · 457 · 463 · 472 · 484 · 553 · 595 · 611 · 632 · 665 · 671 · 683 · 816 · 828 · 834. 간격 대부분 6~42f.
- 42f를 넘는 곳은 세 군데이고 모두 안에서 움직임이 이어진다(B 74 · 69f와 같은 경우): 60→111 51f(`camera-rise` 45f 동안 계속 움직임) · 322→394 72f(타이핑 4f마다 바뀜) · 484→553 69f(`camera-push` 45f + `hold-line`). 롤(683→816)도 4f 바뀜이 7~12f마다 이어진다.

### 위치값 (PNG @2x 실측 ÷ 2, 폰 화면 왼쪽 위 기준 @1x)
| 무엇 | 화면 | 자리 |
|---|---|---|
| `mission-card` 겹침 | 01-home | 왼쪽 20 · 위 294 · 350×253 (PNG 카드 40–740 · 588–1093) |
| 스킬 행 가림 면(`video-card`) | 02-skills | 왼쪽 0 · 위 410 · 390×264 |
| `skill-card-1~3` 자리 | 02-skills | 왼쪽 0 · 위 410 / 498 / 586 · 350×88 (PNG 썸네일 위 860 / 1036 / 1212, 왼쪽 40 → 카드 안쪽 여백 20을 뺀 자리) |
| 검색창 (클로즈업 중심) | 02-skills | 왼쪽 20 · 위 164 · 350×44 (PNG 40–740 · 328–415) |
| 검색창 안내 문구 가림 | 02-skills | 왼쪽 32 · 위 177 · 140×18 (PNG 글자 64–344 · 355–390) |
| 진행 바 채움(점 자리 = 왼쪽 끝) | 03-mission | 왼쪽 37 · 위 282 · 0.5일 때 폭 159 (PNG 74–392 · 563–568) |
| 입력칸 (클로즈업 중심) | 03-mission | 왼쪽 20 · 위 605 · 350×107 (PNG 40–740 · 1210–1425) |
| 입력칸 안내 두 줄 가림 | 03-mission | 왼쪽 36 · 위 650 · 240×43 (PNG 글자 72–552 · 1300–1385) |
| 타이핑 글자 자리 | 03-mission | 안내 첫 줄 자리(왼쪽 36 · 위 650) |
| `button-submit` 도착 자리 | 04-approved | 왼쪽 20 · 위 668 · 350×44 (PNG 40–740 · 1336–1424) |
| `badge-approved` 자리 · 가림 면 (N5) | 04-approved | 왼쪽 20 · 위 310 · 108×32 (PNG 40–256 · 620–684) |
| `stat-card` 겹침 | 05-assets | 왼쪽 20 · 위 168 · 350×101 (PNG 40–740 · 336–538) |
| 첫 자산 카드 (클로즈업 중심) | 05-assets | 왼쪽 20 · 위 481 · 350×74 (PNG 40–740 · 962–1110) |

**반영한 reference**: R1 R2 R3 R4 R5 R6 R7 R8 R9 R10 R11 R12 R13 R14 R15 R16 R17 R18 R19 R20 R21 R22 — **반영 22/22**
- 일부만: R6(검색창 · 입력칸 클로즈업은 PNG 영역이라 폰 가장자리 · 둘레가 보임. 완전 단독은 버튼 · 자산 카드) · R12(앞 장면 물체가 아니라 카드가 목록 자리로 안착) · R14(스크롤 없음, 같은 자리 디졸브만. 이유는 위 "바뀐 점 1") · R18(강조 단어만, 물체 날아듦 없음) · R4("알림 위에서 내려옴" 단계 없음, push 뒤 05를 거쳐 wipe) · R20(가격 오르내림 대신 금액 정착 · 입력칸 타이핑).

### 새 후보 (쓰기 전에 값을 골라야 함)

| 번호 | 무엇 | 쓰는 비트 | 후보 값 | 근거 |
|---|---|---|---|---|
| N2 | 강조 단어 줄 크기 배율 (앞 글줄 대비) | 1–2 | (a) 앞 줄 `video-heading` 50.4 → 강조 `video-display` 78.4 (약 1.56배) · (b) 앞 줄 `video-body` 42 → `video-display` 78.4 (약 1.87배, B에 더 가까움). 둘 다 `video-display`를 넘지 않음(단정하게) | R18 (B f48→50 약 2배) |
| N7 | 새 장면 간격 기준 | 전체 | (a) 새 요소 · 화면 · 카메라 시작 간격 42f 이하, 안에서 움직임이 이어지면 예외 허용 + 정지 상한 `hold-line` (이 표가 맞춘 기준) · (b) 36f(= `motion-enter` + `hold-line`) 엄격 상한 — 고르면 비트 3 · 10 · 14를 쪼개야 함 | R2 (가운데값 약 32f, 대부분 20~42f, 예외 74 · 69f) · R3 (정지 최대 약 24f) |
| N8 | 클로즈업 · 단독 부품 크기 | 7 · 10 · 11 · 16 | (a) ×2.8 `video-scale` (부품 980px = 프레임 폭 51%, `docs/video.md` 5장 그대로, 표 기준) · (b) B처럼 프레임 폭 약 60%(검색창) ~ 거의 전체(버튼) — `video.md` 5장 배율을 바꿔야 함 | R6 (B f160 검색창 약 60% · f390 버튼 거의 전체) · R9 |
| N9 | `camera-push` 배율 · 기준점 | 14 | (a) 1.4배(motion.md 그대로) · (b) 1.8배(B f448→481 폰 폭 36→65%). 기준점은 둘 다 배지 · "미션을 완성했어요!" 묶음(위쪽) | R7 · R11 |
| N10 | 빠른 stagger 간격 | 6 | (a) `duration-6` (표 기준) · (b) `duration-4`. motion.md 기본 `duration-9`로 두면 비트 6이 +6f라 다른 비트에서 6f를 빼야 함 | R12 · R18 (B f52→74 4~6f 간격) |
| N11 | `stat-card` 금액 바뀜 전체 길이 · 시작값 | 15 | (a) `duration-18`, 0에서 `data-final` 29,700까지 자리마다 `motion-tick` (표 기준) · (b) 24f(6f 간격 × 4번, B 실측). (b)면 비트 15 = 24 + `hold-beat` 12 + `hold-breath` 6으로 길이 그대로. 중간 숫자는 화면에 없는 값이라 시작값도 함께 정해야 함 | R20 (B 가격 26f · 금액 20f) |
| N12 (새) | 스킬 카드가 목록 자리에 들어오는 모양 (motion.md 3장 "부품용 등장 거리 없음") | 6 | (a) 움직임 거리 없이 투명도만 · (b) N3 값 재사용 `scale 0.8 → 1.0`으로 커지며 자리에 안착 | R12 (B f100→112 물체가 줄어들며 행 아이콘 자리에 안착, 거리 이동보다 크기 변화) |
| N13 (새) | 검색창 · 입력칸 안내 문구를 가리는 면 색 | 7 · 10 | (a) `video-card`(N5 그대로 흰 면) — 두 칸 바탕이 회색이라 흰 면이 보일 수 있음 · (b) `video-bg`(= `color-surface` #f7f7f8, 칸 바탕과 같은 값으로 보임. 구현 때 PNG 픽셀로 확인) | R19 (B f160 빈 검색창에서 타이핑 시작) · N5 |
| N14 (새) | `button-submit` 왼쪽부터 채우는 면 색 (motion.md 3장에 색 없음) | 11 | (a) `video-text`(= `color-text` #18191b, 뒤 wipe 검은 면과 같은 계열) · (b) `video-success`(= `color-success`, 다음 장면 "승인 완료" 글자색과 같음) | R15 (B f394→410 채움) |
| N15 (새) | 이름 롤 머무름 줄이는 계단 (합 71f 고정) | 18 | (a) 12 · 11 · 10 · 9 · 8 · 7 · 7 · 7 (motion.md 4장 "12에서 7까지 줄임" 1f씩, 표 기준) · (b) 12 · 12 · 10 · 8 · 8 · 7 · 7 · 7 (B처럼 같은 값이 몇 번 이어지는 계단) | R21 (B 롤 간격 10 · 10 · 10 · 8 · 8 · 8 … 6f로 점점 빨라짐) |

## 새 후보 결정 (사용자, 2026-10-25 · 승인 1 뒤)
- 추가 구간(강조 단어 줄 · 진행 바 채움 · 03 입력칸 타이핑 · 검은 면 이름 롤): **이대로**
- N9 `camera-push` 배율: **(b) 1.8배**, 기준점은 배지 · 제목 묶음
- N14 버튼 채움 색: **(b) `video-success`**
- N13 가림 면 색: **(b) `video-bg`** (구현 때 입력칸 바탕과 픽셀 확인)
- N2 **(a)** `video-heading` → `video-display` · N7 **(a)** 42f 이하(안에서 움직임이 이어지면 예외) + 정지 상한 `hold-line` · N8 **(a)** ×2.8 `video-scale` · N10 **(a)** `duration-6` · N11 **(a)** `duration-18`, 0 → 29,700 · N12 **(a)** 투명도만 · N15 **(a)** 12·11·10·9·8·7·7·7
- mission-approved에서 정해진 N1 · N3 · N4 · N5 · N6은 그대로
- N13 비트 7: PNG 빈 영역으로 덮음(사용자, 2026-10-26)
