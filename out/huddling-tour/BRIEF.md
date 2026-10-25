# BRIEF — huddling-tour

작성: 2026-10-25 · 사용자 요청: "좀 역동적으로 30초짜리" · 세 질문은 기본값

| 질문 | 답 |
|---|---|
| 1. 무엇을 | 화면 5장 전체: `src/screens/01-home` → `02-skills` → `03-mission` → `04-approved` → `05-assets` · 부품 `skill-card-1~3` · `mission-card` · `button-submit` · `badge-approved` · `stat-card` · `asset-card` (+ 엔딩 `logo` · `brand-icon`) |
| 2. 몇 초 | 30초 (= 900f, 30fps) |
| 3. 레퍼런스 | `references/`의 영상 2개 (`references/sources.md`) |

## 느낌
- **역동적으로**: 움직임의 성격은 docs/motion.md 그대로(경쾌함, 반동 없음)이고, 역동성은 비트 밀도 · 연속 전환 · 카메라 이동으로 낸다. 새 숫자는 만들지 않는다.
- 지난 영상(mission-approved)에서 쓰지 않았거나 약했던 B의 요소를 살린다: 이름 롤(R14 롤 부분), 강조 단어(R13), 타이핑, 부품이 다음 장면이 되는 연속 전환, 클로즈업 구도(R4).

## 레퍼런스 역할
| 레퍼런스 | 파일 | 역할 |
|---|---|---|
| B · Nafa (@SaadPastaDev) | `references/skillry-saadpastadev-347341.mp4` | **뼈대** (구성 · 구도 · 전환 · 글자 배치) |
| A · Remotion Device Rise | `references/remotion-device-rise.mp4` | **카메라** (폰 등장) |

## 이미 정해진 값 (mission-approved에서 사용자 결정, 이번에도 씀)
`out/mission-approved/scenes.md` 맨 아래 "새 후보 결정": 폰 세로 가운데(N1) · 배지 `scale 0.8 → 1.0`(N3) · `camera-rise` 600px(N4) · PNG 배지 가리기(N5) · wipe 면 `video-end-bg`(N6).
