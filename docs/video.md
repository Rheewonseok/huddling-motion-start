# video.md

영상 룩 기준. 캔버스 **16:9 · 1920×1080 · 30fps**.
규칙: 색 · 폰트는 [design.md](design.md)에서만 가져온다. 움직임은 [motion.md](motion.md)를 따른다. 장면 순서 · 흐름 · 구성은 여기에 쓰지 않는다. 레퍼런스와 비트 시트가 정한다.
정한 것 (2026-10-25): 배경 **밝은** · 헤드라인 **단정하게** · 엔드 카드 **어두운**.

---

## 1. 텍스트 최소 크기

| 변수 | 값 | 근거 |
|---|---|---|
| `video-scale` | **×2.8** | 피그마 글자 크기를 영상용으로 키우는 배율 (모션용 텍스트) |
| `video-text-min` | **30.8px** | 가장 작은 스타일 `Text/eyebrow` 11px × 2.8 |

- 영상 위에 직접 올리는 글자는 30.8px보다 작게 쓰지 않는다.
- 폰 프레임 **안의** 글자(화면 PNG · 1배 parts)는 이 규칙에서 빠진다. 꼭 읽혀야 하면 카메라로 다가가거나(motion.md 5장), parts를 ×2.8로 따로 띄운다.

---

## 2. 배경

| 변수 | hex | design.md 토큰 | 쓰는 곳 |
|---|---|---|---|
| `video-bg` | `#f7f7f8` | `color-surface` | 본편 기본 바탕 (밝은) |
| `video-card` | `#ffffff` | `color-bg` | 폰 화면 · parts가 올라가는 면 |
| `video-tint` | `#edf1ff` | `color-primary-subtle` | 강조 장면 바탕 (필요할 때만) |
| `video-char-bg` | `#e3f2fd` | `color-character-bg` | 캐릭터만 단독으로 나오는 장면 바탕 |
| `video-end-bg` | `#18191b` | `color-text` | 엔드 카드 바탕 (어두운) |

- 바탕은 단색만 쓴다. 그러데이션 · 패턴 · 질감은 design.md에 값이 없으니 쓰지 않는다.
- 흰 화면이 흰 바탕에 묻히지 않도록 본편 바탕은 `video-bg`(#f7f7f8)이고, 그 위에 `video-card`(#ffffff)가 올라간다.

---

## 3. 글자

폰트는 `Pretendard` 하나뿐이다. 로컬 파일 `src/assets/fonts/Pretendard-{Regular,SemiBold,Bold}.otf`를 쓴다(design.md 3장 A). 첫 프레임을 캡처하기 전에 `document.fonts.ready`를 기다린다. 자간은 0%다.
크기와 행간은 피그마 값 × 2.8이다. 소수점 값도 그대로 쓴다(반올림하면 design.md에 없는 숫자가 된다).

| 변수 | 원본 스타일 | 굵기 | 크기(px) | 행간(px) | 쓰는 곳 |
|---|---|---|---|---|---|
| `video-display` | `Text/display` 28/34 | 700 | 78.4 | 95.2 | **헤드라인** (단정하게: 이보다 크게 쓰지 않음) |
| `video-title` | `Text/title` 24/32 | 600 | 67.2 | 89.6 | 두 번째 큰 문장 |
| `video-compact` | `Text/compact-title` 22/28 | 700 | 61.6 | 78.4 | 짧고 굵은 한 줄 |
| `video-section` | `Text/section` 20/28 | 700 | 56 | 78.4 | 엔드 카드 문장 · 숫자 강조 |
| `video-heading` | `Text/heading` 18/28 | 600 | 50.4 | 78.4 | 보조 문장 |
| `video-body` | `Text/body` 15/24 | 400 | 42 | 67.2 | 설명 한 줄 |
| `video-list` | `Text/list-title` 15/22 | 600 | 42 | 61.6 | 목록 항목 · 이름 |
| `video-label` | `Text/label` 14/20 | 600 | 39.2 | 56 | 라벨 · 버튼 문구 |
| `video-caption` | `Text/caption` 12/16 | 400 | 33.6 | 44.8 | 출처 · 작은 안내 |
| `video-eyebrow` | `Text/eyebrow` 11/16 | 600 | 30.8 | 44.8 | 문장 위 작은 머리말 (= 최소 크기) |

| 변수 | hex | design.md 토큰 | 쓰는 곳 |
|---|---|---|---|
| `video-text` | `#18191b` | `color-text` | 밝은 바탕 위 기본 글자 |
| `video-muted` | `#75777c` | `color-text-muted` | 보조 글자 |
| `video-accent` | `#3759de` | `color-primary` | 강조 단어 하나 |
| `video-success` | `#247a51` | `color-success` | 완료 · 상승 숫자 |
| `video-error` | `#b42318` | `color-error` | 오류 · 하락 숫자 |
| `video-end-text` | `#ffffff` | `color-bg` | 엔드 카드(어두운) 위 글자 |

- 굵기는 400 · 600 · 700만 쓴다.
- 한 문장에서 `video-accent`는 한 군데만 쓴다.

---

## 4. 폰 프레임

화면 PNG는 `src/screens/*.png`이고 크기는 780×1688(= 390×844 @2x)이다.

| 변수 | 값 | 근거 |
|---|---|---|
| `video-phone` | 화면 **390×844** (PNG를 0.5배로) | design.md 6장 화면 크기 @1x. 1080 높이 안에 들어간다 |
| `video-phone-bg` | `#ffffff` (`color-bg`) | 화면 뒤 바탕 |
| `video-phone-line` | 1px `#e9eaed` (`color-border`) | 화면 가장자리 선. 1px은 parts의 선 두께와 같다 |
| `video-phone-shadow` | `Shadow/lg` 0 · 8 · 24 · 0 `#0000001F` | design.md 4장 그림자 |

- 폰 프레임 안의 parts는 1배(피그마 크기 그대로)로 쓴다. 화면 PNG와 축척이 같다.
- 확대는 카메라로만 한다(motion.md `camera-push` 약 1.4배). 프레임 자체의 크기는 바꾸지 않는다.
- **새 후보**: 프레임 모서리 반경 · 베젤 두께 · 상단 노치. design.md에 값이 없어서 쓰기 전에 정해야 한다. 정하기 전까지는 베젤 없이 화면만, 직각으로 쓴다.

---

## 5. parts

`src/parts/*.html`은 피그마 크기(1배)로 되어 있다. 부품 파일은 고치지 않고 감싸서 쓴다.

| 쓰는 방식 | 배율 | 방법 |
|---|---|---|
| 폰 프레임 안 | ×1 | 그대로 둔다 (4장) |
| 영상 위에 단독으로 | ×2.8 (`video-scale`) | 감싸는 요소에 `zoom: 2.8`. 안쪽 글자도 3장 크기와 같아진다 |

×2.8로 띄울 때의 크기 (피그마 크기 × 2.8)

| 파일 | 피그마 | ×2.8 |
|---|---|---|
| `asset-card.html` | 350×74 | 980×207.2 |
| `badge-approved.html` | 108×32 | 302.4×89.6 |
| `brand-icon.html` | 98×98 | 274.4×274.4 |
| `button-submit.html` | 350×44 | 980×123.2 |
| `logo.html` logotype · symbol | 149×19 · 100×100 | 417.2×53.2 · 280×280 |
| `mission-card.html` | 350×253 | 980×708.4 |
| `skill-card-1~3.html` | 350×88 | 980×246.4 |
| `stat-card.html` | 350×101 | 980×282.8 |

- 상태가 있는 부품(`asset-card` · `button-submit`)은 `data-state`만 바꾼다. 숫자는 `stat-card`의 `#stat-card-amount` 글자만 바꾼다.
- 단독으로 띄운 parts에는 그림자 `Shadow/md` 0 · 4 · 12 · 0 `#00000014`를 준다. 이 값은 zoom 밖에 둔다.
- 엔드 카드(어두운 바탕)에서는 `logo` white 버전(`logo-*-white.svg`)이나 `brand-icon`을 쓴다. 밝은 바탕에서는 black 버전을 쓴다.
- 캐릭터 PNG(`buddy-front-1 · 2`, `perdi-flag`)는 원본 그대로 쓴다. 색을 바꾸거나 잘라 내지 않는다.
