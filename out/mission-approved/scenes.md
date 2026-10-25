# scenes — mission-approved

15초 = 450f (30fps, 1920×1080) · 중심: 화면 `src/screens/04-approved.png` + 부품 `src/parts/badge-approved.html`
뼈대 B (Nafa) · 카메라 A (Device Rise). 문구는 `04-approved.png` · 부품 HTML에 있는 글자만 쓴다.

## 1차: 3안 요약 (하나를 고른다)

### 안 A — 화면 중심 "폰이 올라오고, 승인 순간에 밀고 들어간다"
- 콘셉트: B의 5단 흐름을 15초로 줄임. 글줄 "미션을 완성했어요!"가 단어마다 붙고(`motion-pop` · `hold-line`) → 폰이 `camera-rise`로 솟아 글줄을 밀어냄 → `hold-breath` 뒤 화면 안 `badge-approved`가 `motion-pop`으로 커짐 → `camera-push`로 배지 · 제목 묶음에 다가감 → 배지가 `camera-wipe`로 커져 `video-end-bg` 엔드(logo white + 보조 줄 "내 자산에서 보기", `hold-screen`).
- 뼈대: B 00:00–00:24 전체 구성 + B 00:13–00:16 완료 비트 순서. 카메라는 A 솟아오름.
- 화면 · 부품: `src/screens/04-approved.png`(폰 안 ×1), `src/parts/badge-approved.html`(폰 안 ×1), 엔딩 `src/parts/logo.html`(white).
- 반영: R1 R2 R3 R4 R5 R6 R7 R8 R9 R10 R11 R12 R14(엔딩만) — 반영 13/14 (R13 안 씀). 새 후보: N1 · N3 · N4.

### 안 B — 부품 클로즈업 중심 "버튼을 누르면 배지가 된다"
- 콘셉트: 폰 없이 부품을 ×2.8로 단독으로 띄워 시작. `button-submit`(`data-state="submit"` "제출하기")이 `motion-travel`로 들어와 채움 → 같은 자리에서 `badge-approved`로 `motion-swap`, 배지 `motion-pop` + `hold-beat` → `camera-pull-out`으로 빠져나오면 그 배지가 `04-approved` 화면 속 배지가 됨(부품 → 다음 장면, `hold-screen`) → 배지 `camera-wipe` → 어두운 엔딩(`brand-icon` → 보조 줄 "내 자산에서 보기").
- 뼈대: B 00:12–00:16 버튼 채움 → 결과 화면 → 덮고 컷 구간을 영상 전체로 늘림. 카메라 A는 쓰지 않음.
- 화면 · 부품: `src/parts/button-submit.html`(`submit` ×2.8), `src/parts/badge-approved.html`(×2.8 → 폰 안 ×1), `src/screens/04-approved.png`, 엔딩 `src/parts/brand-icon.html`.
- 반영: R1 R2 R3 R8 R10 R11 R14(엔딩만) — 반영 7/14. 새 후보: N1 · N3. (`camera-pull-out` 배율이 reference에 없어서 2차에서 새 후보로 따로 적어야 할 수 있음)

### 안 C — 글자 중심 "배지가 문장의 강조 단어가 된다"
- 콘셉트: `video-bg` 위 글줄이 주인공. "미션을 완성했어요!" 단어마다 붙음 → 다음 줄 자리에 강조 단어 대신 `badge-approved`가 ×2.8로 따로 한 줄 크게 등장(`motion-travel`) → 폰은 짧게 `camera-rise`로 올라와 `04-approved`를 `hold-screen`만큼 보여 줌 → 배지 `camera-wipe` → 검은 면 두 줄 롤: 위 고정 "이번 달 미션", 아래 "자동화 자산 1개" → "실제 적용 사례 1개" → "100% · 4/4 단계 완료"가 `motion-tick`으로 굴러감(`hold-beat`부터 줄어듦) → 엔딩(logo white + "내 자산에서 보기").
- 뼈대: B 00:00–00:02 글줄 도입 + B 00:16–00:22 검은 면 롤 · 엔딩을 키우고, 폰 구간은 줄임. 카메라 A 솟아오름.
- 화면 · 부품: `src/parts/badge-approved.html`(×2.8 단독 → 폰 안 ×1), `src/screens/04-approved.png`, 엔딩 `src/parts/logo.html`(white). 글자는 모두 `04-approved.png` 안 문구.
- 반영: R1 R3 R5 R6 R8 R9 R11 R12 R13 R14 — 반영 10/14 (R2 R4 R7 R10 안 씀). 새 후보: N1 · N2 · N3 · N4.

---

## 2차: 장면표

**고른 안: A** (화면 중심, 승인 1)

- 표기: `시작f–끝f`에서 끝f는 다음 비트의 시작f다(끝f 미포함). 비트 길이 = 끝f − 시작f.
- 바탕: 비트 1–7은 `video-bg`, 비트 8–10은 `video-end-bg`. 폰 화면 뒤는 `video-phone-bg`, 가장자리 `video-phone-line`, 그림자 `video-phone-shadow`, 베젤 없이 직각(`docs/video.md` 4장).
- 폰은 `video-phone`(PNG 0.5배) 크기 그대로, 폰 안 부품은 ×1(`docs/video.md` 5장). 폰 안 글자는 최소 크기 규칙에서 빠진다(1장). 폰 밖 글자는 모두 `video-eyebrow` 이상.
- 1차 요약에서 바뀐 점 두 가지. (1) R10 반영: 폰이 빈 화면으로 솟아 안착한 뒤 화면 내용이 `motion-swap`으로 들어온다. (2) 길이를 토큰으로 채우려고 글줄 도입을 두 줄로 하고(R12 줄 교체), wipe 뒤 검은 면 글줄 한 줄을 넣었다(R1 4단 · R14 앞부분, 롤은 없음).

| 비트 | 시작f–끝f | 화면 · 부품(src 경로) | 글자(문구 · video.md 3장 토큰) | 움직임(motion.md 2 · 3장 토큰) | 머무는 시간(motion.md 4장) | 카메라(motion.md 5장) | reference 번호 |
|---|---|---|---|---|---|---|---|
| 1 글줄 1 | 0–36 (36f) | 없음. 빈 `video-bg` 정중앙에 글줄 한 줄 | "이번 달 미션" · `video-display` · `video-text` | 단어 3개("이번" · "달" · "미션")마다 `motion-pop`, 단어 사이 간격 `duration-9` | `hold-beat` | 고정 | R5 R12 R1 |
| 2 글줄 2 | 36–75 (39f) | 없음. 같은 자리 | "미션을 완성했어요!" · `video-display` · `video-text`, "완성했어요!"만 `video-accent` | 첫 단어 "미션을"이 같은 자리에서 앞 줄을 바꿔 씀 `motion-swap` → "완성했어요!" `motion-pop` | `hold-line` | 고정 | R5 R12 R1 |
| 3 폰 솟아오름 | 75–126 (51f) | `src/screens/04-approved.png` 폰 틀만(화면 내용 없음, `video-card` 빈 면) | 글줄 2가 퇴장 | 폰: `camera-rise`. 글줄 2: 같은 자리에서 옅어져 퇴장 `motion-swap`(75–84, 폰이 솟는 동안) | `hold-breath`(안착 뒤 숨) | `camera-rise` | R6 R9 R1 |
| 4 결과 화면 들어옴 | 126–195 (69f) | `src/screens/04-approved.png` 내용 전체(폰 안 ×1). 배지 자리는 아직 비어 있음(새 후보 N5) | 폰 안 PNG 문구만 (새 글자 없음) | 빈 화면 위로 화면 내용 페이드 인 `motion-swap` (`screens` 화면 바꿈) | `hold-screen`(화면 하나 읽기) | 고정 | R10 R3 R2 |
| 5 배지 등장 | 195–207 (12f) | `src/parts/badge-approved.html`(폰 안 ×1, PNG 배지 자리) | "승인 완료" (부품 안 글자, 폰 안 ×1) | 작게 시작해 커지며 등장 `motion-pop`, 처음 크기 새 후보 N3 | `hold-breath`(B 완료 비트의 숨) | 고정 | R11 R2 |
| 6 밀고 들어감 | 207–288 (81f) | `src/screens/04-approved.png` + `src/parts/badge-approved.html`(폰 안 ×1) | 클로즈업에 "승인 완료" · "미션을 완성했어요!" 묶음이 프레임 가운데 위쪽 (폰 안 글자) | 없음 (카메라만) | `hold-line` + `hold-beat` | `camera-push` (기준: 배지 · 제목 "미션을 완성했어요!" 묶음. 아래 세부 정보는 프레임 밖) | R7 R4 R2 |
| 7 배지가 덮음 | 288–294 (6f) | `src/parts/badge-approved.html`(커져서 프레임을 덮음) | 없음 | 없음 (카메라만) | 없음 (덮은 순간 294에서 컷) | `camera-wipe` (덮는 면 색은 새 후보 N6) | R8 R2 R1 |
| 8 검은 면 글줄 | 294–372 (78f) | 없음. `video-end-bg` 정중앙에 글줄 한 줄 | "결과물이 승인되어 내 자산에 등록됐어요." · `video-section` · `video-end-text` | 단어 5개("결과물이" · "승인되어" · "내" · "자산에" · "등록됐어요.")마다 `motion-pop`, 간격 `duration-9` | `hold-line` + `hold-beat` | 고정 | R1 R14 R12 |
| 9 글줄 퇴장 | 372–378 (6f) | 없음 | 비트 8 글줄 퇴장 | 어두워지며 퇴장 `motion-pop`(`curve-in`) | 없음 | 고정 | R14 |
| 10 엔딩 | 378–450 (72f) | `src/parts/logo.html` `data-state="logotype-white"` ×2.8 단독(`video-scale`) | 로고 아래 보조 줄 "내 자산에서 보기" · `video-body` · `video-end-text` | 로고 `motion-pop`(378–384) → 보조 줄 `motion-pop`(384–390) | `hold-screen` | 고정 | R14 R1 |

**길이 내역** (모두 motion.md 토큰의 합. 합계 450f = 15s × 30f)

| 비트 | 길이 | 토큰 합 |
|---|---|---|
| 1 | 36 | 간격 `duration-9` ×2 (18) + `motion-pop` 6 + `hold-beat` 12 |
| 2 | 39 | `motion-swap` 9 + `motion-pop` 6 + `hold-line` 24 |
| 3 | 51 | `camera-rise` 45 + `hold-breath` 6 (글줄 퇴장 `motion-swap` 9는 rise와 겹침) |
| 4 | 69 | `motion-swap` 9 + `hold-screen` 60 |
| 5 | 12 | `motion-pop` 6 + `hold-breath` 6 |
| 6 | 81 | `camera-push` 45 + `hold-line` 24 + `hold-beat` 12 |
| 7 | 6 | `camera-wipe` 6 |
| 8 | 78 | 간격 `duration-9` ×4 (36) + `motion-pop` 6 + `hold-line` 24 + `hold-beat` 12 |
| 9 | 6 | `motion-pop`(`curve-in`) 6 |
| 10 | 72 | `motion-pop` 6 + `motion-pop` 6 + `hold-screen` 60 |
| 합 | **450** | |

구간 비율(R1 대조): 글줄 도입 0–75 (17%, B 12%) · 폰 + 완료 순간 75–294 (49%, B 55%) · 검은 면 글줄 294–378 (19%, B 23%) · 엔딩 378–450 (16%, B 10%).

**반영한 reference**: R1 R2 R3 R4 R5 R6 R7 R8 R9 R10 R11 R12 R14 — **반영 13/14**
- 안 씀: R13 (강조 단어를 따로 크게 두는 배치. 안 A는 글자 중심이 아니어서 뺌. 그래서 N2도 안 씀)
- 일부만: R2는 "알림 위에서 내려옴"(두 번째 `motion-pop`) 단계를 뺐다(화면 · 부품에 알림이 없어서). R9는 폰 등장을 `motion-enter` 대신 R6의 `camera-rise`로 했다(글줄 퇴장 `motion-swap`은 그대로). R14는 롤 없이 검은 면 한 줄 + 엔딩만.

### 새 후보 (쓰기 전에 값을 골라야 함)

| 번호 | 무엇 | 쓰는 비트 | 후보 값 | 근거 |
|---|---|---|---|---|
| N1 | 폰 화면 세로 위치 · 아래 잘림 | 3–5 | (a) 전체 보임: `video-phone` 390×844를 1080 안 세로 가운데 (`docs/video.md` 4장 그대로, 권장) · (b) B처럼 위 여백 약 6%(1080 기준 약 65px)만 두고 화면 아래쪽을 프레임 밖으로 자름 | R3 (B 00:08 f250: 폭 약 36%, 위 여백 약 6%, 아래 잘림). 참고: B 폭 36%는 1920 기준 약 691px이지만 `video.md` 4장이 프레임 크기를 바꾸지 말라고 해서 폭은 390 그대로 둠 |
| N3 | `badge-approved` 처음 크기 | 5 | (a) `scale 0.8 → 1.0` (A 문서 값, motion.md 3장 새 후보와 같은 건) · (b) 더 작게 시작(값을 따로 정함) | R11 (B 00:14 f420→430 체크 아이콘이 작게 시작해 커짐. 수치 없음) |
| N4 | `camera-rise` 거리의 1080 환산 | 3 | (a) `translateY 600px → 0` (720 기준 400px × 1.5) · (b) `translateY 400px → 0` (문서 값 그대로) | R6 (A 문서 값은 1280×720 기준) |
| N5 | PNG 안에 이미 그려진 배지 처리 | 4–5 | (a) 비트 4에서 PNG 배지 자리를 `video-card` 면으로 가려 비워 두고, 비트 5에서 그 자리에 `badge-approved` ×1을 `motion-pop`. 자리는 PNG 실측 @1x 왼쪽 20 · 위 310 · 108×32 · (b) 가리지 않고 PNG 배지 위에 같은 부품을 겹쳐 `motion-pop`만 (처음부터 배지가 보여서 "커지며 등장"이 약해짐) | R10 (빈 화면 → 내용 페이드 인 뒤) · R11 ("완료" 요소 하나만 따로 등장). `04-approved.png`에 배지가 이미 들어 있어서 정해야 함 |
| N6 | `camera-wipe`로 덮는 면의 색 | 7 | (a) 배지 바탕색 그대로(`color-primary-subtle` = `video-tint`) 프레임을 덮고 294에서 `video-end-bg`로 컷 · (b) 커지는 6f 동안 배지 바탕이 `video-end-bg`로 바뀌어 검은 면이 된 뒤 컷 (B와 같은 모양) | R8 (B 00:16 f482→488 알림이 커지며 검은 면이 됨, 컷 f490) |

## 새 후보 결정 (사용자, 2026-10-25 · 승인 1 뒤)
- 추가 구간(글줄 도입 2줄 · 검은 면 글줄): **이대로**
- N1 폰 자리: **(a)** 390×844 전체를 1080 안 세로 가운데
- N3 배지 처음 크기: **(a)** `scale 0.8 → 1.0` (A 문서 값)
- N4 `camera-rise` 거리: **(a)** `translateY 600px` (A 문서 400px × 1080/720)
- N5 PNG 배지: **(a)** 비트 4에서 배지 자리를 `video-card` 면으로 가리고, 비트 5에서 그 자리에 부품 `motion-pop`
- N6 wipe 면 색: **(b)** 커지는 6f 동안 `video-end-bg`로 바뀐 뒤 컷
