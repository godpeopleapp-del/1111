# Template Showcase

순수 HTML/CSS/JS로 만든 템플릿 쇼케이스 예시입니다.

## 구조

- **왼쪽 패널**: 템플릿 목록 (클릭 시 미리보기 전환)
- **오른쪽**: 선택된 템플릿 실시간 미리보기 (iframe)
- **배경**: 완전 투명 (`background: transparent`) — 부모 페이지 배경이 그대로 비침

## 포함 템플릿

| ID | 이름 | 색상 |
|----|------|------|
| `wedding` | 모바일 청첩장 | #EC4899 |
| `qr` | QR 키오스크 | #F59E0B |
| `booking` | AI 예약 페이지 | #A78BFA |
| `landing` | 랜딩 페이지 | #34D399 |

## 사용법

```html
<!-- 단독 실행 -->
open index.html

<!-- iframe으로 임베드 -->
<iframe src="index.html" allowtransparency="true" style="background:transparent;"></iframe>
```

## 템플릿 추가 규격

`TEMPLATES` 배열에 아래 형식으로 추가:

```js
{
  id: "unique-id",       // 고유 식별자
  label: "표시 이름",    // 사이드바에 표시될 이름
  emoji: "🎯",           // 아이콘 이모지
  color: "#HEX",         // 테마 색상 (hex)
  html: `<div>...</div>` // 미리보기에 렌더링될 HTML 문자열
}
```
