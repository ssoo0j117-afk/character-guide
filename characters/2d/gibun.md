# 기분파 (Gibun · 감정형) — 2D 캐릭터 프롬프트

> 캐릭터 시그니처 락(Lock) 표 기반. 아래 "고정값"은 절대 변경하지 말고, "가변 요소"만 상황에 따라 조정하세요.

---

## 0. 공통 구조 규칙 (4종 캐릭터 전체 동일 적용)

| 항목 | 규칙 |
|---|---|
| 실루엣 | 목 없이 머리+몸통이 하나의 둥근 덩어리로 이어짐 (egg / teardrop 형태) |
| 몸통 블록 비율 | 전체 캐릭터 높이의 약 80~92%가 "머리-몸통 블록", 나머지가 다리 |
| 페이스 패치 크기 | 블록 폭의 약 75%, 블록 높이의 약 50~60%를 차지하는 밝은 톤 타원 |
| 페이스 패치 위치 | 블록 상단에서 대략 10~30% 지점부터 시작 (기분파는 4종 중 가장 위쪽) |
| 공통 고정 색상 | 이목구비 라인 `#36322E` (다크 브라운블랙), 입 안쪽 `#EB6153` |
| 팔다리 | 몸통보다 진한 톤의 얇은 타원형, 좌우 대칭 부착 |

## 1. 기분파 고유 설정

| 항목 | 값 |
|---|---|
| 톤 | 옐로우 / 오렌지 |
| 후드(외곽) 컬러 | `#FFD52B` |
| 페이스 패치 컬러 | `#FFF2BE` |
| 포인트 컬러 | 오렌지 `#F38200`, 땡땡이 무늬 `#FCA500` |
| **시그니처 디테일** | 이마 중앙 곱슬 스월 헤어 / 양쪽 날개 모양 귀 장식 (내부 땡땡이 무늬 포함) |

## 2. 가변 요소

- **표정**: 자유롭게 변경 가능 (감정형답게 표정 변화가 풍부하고 생동감 있는 느낌 권장)
- **포즈**: 자유
- **귀 위치**: 포즈에 따라 쫑긋 서거나 축 처질 수 있음 (단, 귀의 형태·색상 자체는 고정)

---

## 3. 2D 이미지 생성 프롬프트 (영문 — 그대로 복사해서 사용)

```
Cute chibi mascot character, flat 2D vector illustration style, matte toy-like finish.

SHAPE: No visible neck — the head and torso merge into a single smooth, rounded egg/teardrop-shaped blob. This head-body block makes up about 80-92% of the character's total height; two short simple oval legs form the remaining bottom portion.

BODY COLOR: Bright yellow hood/outer shell, hex #FFD52B.

FACE PATCH: A pale cream-yellow oval face patch, hex #FFF2BE, covering roughly 75% of the body block's width and 50-60% of its height, positioned starting near the very top of the block (this character has the highest face-patch position among the four).

HAIR (signature detail): A small curly swirl tuft of hair in the center of the forehead, orange tone.

EARS (signature detail): Two wing-shaped ear decorations on either side of the head, with a polka-dot pattern inside using hex #FCA500 dots.

ACCENT COLOR: Orange #F38200 used for ear/wing edges and other accent details; polka dots #FCA500.

FACE: Simple, expressive facial features drawn in dark brownish-black line art, hex #36322E — lively eyes, small nose, an energetic and emotionally expressive mouth. When the mouth is open, the inside shows warm coral-red #EB6153.

LIMBS: Thin oval-shaped arms and legs in orange #F38200, symmetrically attached to the body.

MOOD: Emotional, moody, vivid, expressive personality ("Gibun" = emotion/mood type). Playful, energetic, a little dramatic in expression.

STYLE: Clean flat vector shapes, minimal soft cel-shading, no harsh gradients, no outlines other than the dark facial line art. Matte PVC-figure-like texture cues are optional for this 2D pass.

BACKGROUND: Pure white, hex #FFFFFF, seamless, no shadows or props.

COMPOSITION: Single character, centered, front-facing, full body visible, high resolution, clean silhouette suitable for sticker/mascot use.
```

## 4. 네거티브 프롬프트 (권장)

```
visible neck, long neck, realistic human anatomy, extra limbs, asymmetrical ears, missing forehead swirl, wrong color palette, sharp hard shadows, noisy gradient, text, watermark, signature, multiple characters, cropped, blurry, low detail, background clutter, busy background
```
