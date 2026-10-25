# 레퍼런스 출처 (2026-10-25 받음)

## A. remotion-device-rise.mp4 — Remotion Prompts "Apple-Style Device Rise Animation"
- https://www.remotion.dev/prompts/apple-style-device-rise-animation (@gaucho_booleano, Claude Code · Opus 4.5)
- 1280×720 · 30fps · 4s
- 프롬프트에 적힌 움직임 값 (문서 값):
  - 기기 등장: translateY 400px → 0, rotateX ~35° → ~8°, scale 0.8 → 1.0, 1.5s, Easing.out(Easing.cubic)
  - transformOrigin center bottom, 순서 translateX → translateY → rotateX → scale
  - 기기 안착 뒤 알림 카드가 위에서 아래로 미끄러져 들어옴, 0.3s 간격 stagger
  - 모든 애니메이션 interpolate() + Easing.out(Easing.cubic)

## B. skillry-saadpastadev-347341.mp4 — @SaadPastaDev (Nafa 마케팅)
- https://skillry.dev/ai-videos/opus-5-5/saadpastadev-347341
- 원 게시물 https://x.com/SaadPastaDev/status/2107741413769347341
- 1280×720 · 30fps · 24.55s · Remotion (SVG · GSAP · CSS)
- 공개된 프롬프트는 일부뿐 (움직임 수치 없음) → 값은 프레임 분석으로 뽑음
