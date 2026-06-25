# Assiworks Design System

Assiworks 브랜드의 디자인 토큰 · 유닛 색 · 컴포넌트 · 아이콘 셋. AIFactory 디자인시스템과 동일한 모듈형 CSS 컨벤션을 따릅니다.

## Files

| File | Purpose |
|------|---------|
| `tokens.css` | 핵심 토큰: 브랜드(`#702EFF`), gray(zinc) 팔레트, 유닛/엔진 색, 상태 색, 타이포 스케일, radius, shadow |
| `components.css` | 기본 컴포넌트: reset, `.btn`, `.chip`(engine/type), `.badge`, `.status`/`.status-dot`, `.card`, `.input`, `.seg`(segmented), `.nav-item`, `.toggle` |
| `reference.html` | 토큰·컴포넌트·아이콘을 보여주는 리빙 레퍼런스 |
| `assets/logo-assiworks.svg` | 브랜드 로고 |
| `assets/icons/` | 유닛 아이콘 셋 — `*_Default`(회색) / `*_Selected`(브랜드) 2종, 일부 `*_inFlow` |
| `assets/unit-blocks/` | 플로우 노드용 unit 블록 아이콘(in/out/tool/operator/loop/flow) |

## Usage

```html
<link rel="stylesheet" href="tokens.css">
<link rel="stylesheet" href="components.css">
```

## Font

**Pretendard Variable** + 시스템 폴백.

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/orioncactus/pretendard/dist/web/variable/pretendardvariable.css">
```

## Tokens 요약

- **Brand**: `--brand #702EFF`, hover `--brand-hover #5A25CC`
- **Unit/Engine 색** (타입 식별용): RAG `--rag #14B8A6`(청록) · Tool `--tool #2563EB`(파랑) · Loop `--loop #FF622E`(주황) · Operator `#702EFF` · Cheliped `#0EA5E9` · Input `#008236` · Output `#8058DB`
- **Status**: ready/running(brand)/done(emerald)/error(red)/warn(amber)/paused(sky)
- **아이콘**: Default fill `#F1F1F2`·stroke `#9F9FA9` / Selected fill `#D4C0FF`·stroke `#702EFF`

## 원칙

- **메뉴(분류) ≠ 색**: 유닛 분류는 위계로 표현하고, 색은 플로우 에디터·칩에서 타입 식별 보조로만 사용.
- 아이콘은 Default/Selected 2-state 한 쌍으로 운용.
