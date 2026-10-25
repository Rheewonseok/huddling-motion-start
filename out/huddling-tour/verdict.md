# verdict — huddling-tour

## 1회차 · 대상 3안 요약 (scenes.md)
- 안 A: 통과 · 숫자 0 · UI 0 · 반영 19/22 (86%)
- 안 B: 통과 · 숫자 0 · UI 0 · 반영 14/22 (64%)
- 안 C: 통과 · 숫자 0 · UI 0 · 반영 14/22 (64%)

## 2회차 · 대상 장면표(안 A) (scenes.md 2차, 비트 19개, 900f)
- 통과 · 숫자 0 · UI 0 · 반영 19/22 (86%) (반영 안 셈: R12 앞 장면 물체 없이 카드만 안착 · R14 스크롤 없음, 디졸브는 motion.md 기본 화면 바꿈 · R18 물체 날아듦 없음, 단어 하나가 아닌 줄 강조)

## 3회차 · 대상 스냅보드 (snapboard.png + index.html, 비트 19개, 900f)
- 불합격 · 숫자 1 (비트 15 금액 바뀜 간격 1f, motion-tick duration-4 아님) · UI 0 · 반영 19/22 (86%) (반영 안 셈: R12 · R14 · R18, 2회차와 같음. 결함 기록: 비트 7 검색창 가림 면 오른쪽 끝에 PNG 안내 문구 "요" 가장자리 1px 비침, 화면 PNG 글자라 UI로 세지 않음)

## 4회차 · 대상 스냅보드(수정 1) (snapboard.png + index.html, 비트 19개, 900f)
- 통과 · 숫자 0 · UI 0 · 반영 19/22 (86%) (비트 15 금액 확인: 컴포지션 프레임 f552–572를 1f 간격으로 뽑음(`_frames/v4-amount-sheet.png`). 0 → 6,600 → 13,200 → 19,800 → 29,700 이 f553 · 557 · 561 · 565 · 569에서만 바뀌고 사이 프레임은 같은 값 = motion-tick duration-4 간격, 전체는 N11 (a) duration-18 안. 반영 안 셈: R12 · R14 · R18, 3회차와 같음. 결함 기록(셈 밖): 비트 7 검색창 가림 면 "요" 1px 비침, 3회차와 같음)

## 5회차 · 대상 영상 (huddling-tour.mp4, 1920×1080 · 30fps · 900f)
- 통과 · 숫자 0 · UI 0 · 반영 19/22 (86%) (확인: index.html 수정 00:16:04 < 4회차 기록 00:18:08 < mp4 렌더 00:19:12, 4회차 이후 안 바뀜. ffprobe 1920×1080 · 30/1 · 900f · 30.000s = video.md · 장면표. 영상에서 비트 1~19 안착 프레임과 전환 24곳을 뽑음(`_frames/v5/`). 비트 15 금액 f552–572(`_frames/v5/amount-crop.png`): ₩0(f553) → 6,600(f557) → 13,200(f561) → 19,800(f565) → 29,700(f569), 바뀜 간격 4f, 4회차와 같음. 비트 11 버튼 채움 색은 success-green(#247a51, N14). 보이는 UI는 PNG 5장과 parts(button-submit submit/view-assets · badge-approved · stat-card · asset-card 3상태 · skill-card 1~3 · mission-card 진행 바 · logo logotype-white)뿐. 반영 안 셈: R12 · R14 · R18, 4회차와 같음)
