# Study log

매 작업 후 3줄: 오늘 배운 것 / 내 손으로 고친 것 / 다음에 해볼 것

## 2026-11-16
- GitHub 저장소를 만들고 첫 페이지(index.html)를 올렸다. Git = Figma의 Version History, GitHub Pages = Publish 링크.
- 직접 고쳐볼 것: index.html의 문장을 바꿔보고 commit → push.

## 2026-11-17
- 한 페이지 v0를 코드로 만들었다. `style.css`의 `:root` = Figma Variables, `.h-xl` 같은 클래스 = Text Style, `section`/`.wrap` = Auto Layout 프레임.
- Hero 카드 회전은 자바스크립트 없이 CSS "scroll-driven animation"으로: 카드가 가로 줄에서 어디 있는지(스크롤 위치)가 회전 각도를 움직인다. 지원 안 되는 브라우저는 정적 줄로 떨어진다.
- 직접 고쳐볼 것: `--bg: #ffffff;`를 `#f4f4f0`으로 바꿔 순백과 오프화이트 비교 → commit → push.
