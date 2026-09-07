# 분석파 (Bunseok · 분석형) — 2D 캐릭터 프롬프트

> 캐릭터 시그니처 락(Lock) 표 기반. 아래 "고정값"은 절대 변경하지 말고, "가변 요소"만 상황에 따라 조정하세요.

---

## 0. 공통 구조 규칙 (4종 캐릭터 전체 동일 적용)

| 항목 | 규칙 |
|---|---|
| 실루엣 | 목 없이 머리+몸통이 하나의 둥근 덩어리로 이어짐 (egg / teardrop 형태) |
| 몸통 블록 비율 | 전체 캐릭터 높이의 약 80~92%가 "머리-몸통 블록", 나머지가 다리 |
| 페이스 패치 크기 | 블록 폭의 약 75%, 블록 높이의 약 50~60%를 차지하는 밝은 톤 타원 |
| 페이스 패치 위치 | 블록 상단에서 대략 10~30% 지점부터 시작 |
| 공통 고정 색상 | 이목구비 라인 `#36322E` (다크 브라운블랙), 입 안쪽 `#EB6153` |
| 팔다리 | 몸통보다 진한 톤의 얇은 타원형, 좌우 대칭 부착 |

## 1. 분석파 고유 설정

| 항목 | 값 |
|---|---|
| 톤 | 틸 / 그린 |
| 후드(외곽) 컬러 | `#40ADA3` |
| 페이스 패치 컬러 | `#A0D7D0` |
| 포인트 컬러 | 안경테 다크네이비 `#0F4155` |
| **시그니처 디테일** | 큼직한 동그란 안경 / 정수리 볼(공) 안테나(살짝 굽은 형태) / 양볼 주근깨 / 입을 벌렸을 때 살짝 보이는 흰 이빨 1개 |

## 2. 가변 요소

- **표정**: 자유롭게 변경 가능. **단, 안경은 항상 유지** (분석형의 핵심 아이덴티티)
- **포즈**: 자유
- **귀 위치**: 해당 없음 (분석파는 귀 대신 안테나가 시그니처 요소이며, 안테나 형태·색상은 고정)

---

## 3. 2D 이미지 생성 프롬프트 (영문 — 그대로 복사해서 사용)

```
Cute chibi mascot character, flat 2D vector illustration style, matte toy-like finish.

SHAPE: No visible neck — the head and torso merge into a single smooth, rounded egg/teardrop-shaped blob. This head-body block makes up about 80-92% of the character's total height; two short simple oval legs form the remaining bottom portion.

BODY COLOR: Teal/green hood/outer shell, hex #40ADA3.

FACE PATCH: A soft light teal oval face patch, hex #A0D7D0, covering roughly 75% of the body block's width and 50-60% of its height, positioned starting a little below the top of the block (10-30% down).

ANTENNA (signature detail): A single ball-tipped antenna on top of the head, slightly curved/bent shape, same body tones.

GLASSES (signature detail, MUST always be present): Large round glasses with a dark navy frame, hex #0F4155, centered on the face — this is a mandatory, always-on feature and must never be removed regardless of expression.

FRECKLES (signature detail): A small scatter of freckles on both cheeks.

TEETH (signature detail): When the mouth is open, one single small white tooth is visible peeking from the smile.

FACE: Simple, thoughtful facial features drawn in dark brownish-black line art, hex #36322E — behind the round glasses, calm analytical eyes, small nose, a smart subtle smile. Mouth interior when open shows warm coral-red #EB6153, with the single white tooth detail.

LIMBS: Thin oval-shaped arms and legs in a deeper teal tone than the main body, symmetrically attached.

MOOD: Analytical, calm, smart, observant personality ("Bunseok" = analysis type). Curious and precise, slightly nerdy-cute appeal.

STYLE: Clean flat vector shapes, minimal soft cel-shading, no harsh gradients, no outlines other than the dark facial line art. Matte PVC-figure-like texture cues are optional for this 2D pass.

BACKGROUND: Pure white, hex #FFFFFF, seamless, no shadows or props.

COMPOSITION: Single character, centered, front-facing, full body visible, high resolution, clean silhouette suitable for sticker/mascot use.
```

## 4. 네거티브 프롬프트 (권장)

```
visible neck, long neck, realistic human anatomy, extra limbs, missing glasses, glasses removed, missing antenna, wrong color palette, sharp hard shadows, noisy gradient, text, watermark, signature, multiple characters, cropped, blurry, low detail, background clutter, busy background
```
