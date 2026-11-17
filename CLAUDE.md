# 포트폴리오 PM 노트: 권유정 (Yujeong Kwon)

> 이 파일은 Claude Code가 매 세션 시작할 때 읽는 **PM 노트**입니다. 업데이트: 2026-11-17 (세션 3 종료, 최종)

---

## ▶ 다음 세션 시작점 (여기부터 읽기)

**업데이트: 2026-11-17 (세션 3 종료). 세션 4부터는 `portfolio` 저장소만 붙여서 시작한다.**

### 지금 상태
- **사이트 v0 공개됨:** `https://kwyj9848-stack.github.io/portfolio/` (`index.html` + `style.css`, 순수 HTML/CSS, JS 없음)
- Hero 카드 회전(LP 넘기기) 완료. CSS scroll-driven animation(`animation-timeline: view(inline)`), 미지원 브라우저·동작 줄이기에선 정적.
- 카드 6장 중 실제 이미지: **Fraserview** (`work/fraserview/img/home_d.jpg`), **BCA** (`img/bca-home.jpg`). 나머지 4장(CreoDent, Starlight, LineLoomArt, About)은 색 블록 플레이스홀더.
- **Fraserview 케이스 완료:** `work/fraserview/index.html`. 원본 PT는 `archive/fraserview-pt-original.html`.
- 바디카피 v1 확정, `index.html`에 반영됨. 카피를 바꿀 때는 `index.html`이 기준이다.
- Hero 비주얼 레퍼런스 이미지: `archive/refs/hero-ref-cosmos-crate.jpg` (다크 원본. 우리는 순백+검정)

### 다음에 할 것 (순서)
1. **히어로/랜딩 페이지 전체 틀 잡기 (세션 4 목표).** 이미지는 **전부 목업(플레이스홀더)**으로 둔다. 실제 사진은 나중에 **사용자가 소스를 주면 Claude가 목업을 대체**한다 → 지금은 이미지 채우기를 하지 않는다. 기존 Fraserview·BCA 이미지도 틀 잡는 동안엔 목업으로 바꿔도 된다 (파일은 지우지 않는다).
   - 비주얼 레퍼런스는 **이미 받았다**: `archive/refs/hero-ref-cosmos-crate.jpg` (cosmos.so/e/696464911, LP 넘기기). 이걸 기준으로 순백+검정 고대비로 틀을 잡는다. 추가 레퍼런스를 기다리지 않는다.
   - 볼 것: 레이아웃 그리드, 섹션 간 리듬(여백), 타이포 위계, 카드 줄(LP 넘기기)의 크기·위치, 모바일 첫 화면, 내비게이션
   - 목업은 카드마다 다른 색 블록 + 라벨(예: "CreoDent · cover 3:4")로 비율과 자리가 보이게
2. 폰트·여백 톤 다듬기 (`style.css`의 `:root` 변수만). 사용자가 레퍼런스를 더 주면 그때 반영
3. LinkedIn 주소·레주메 PDF 연결 (`index.html` Contact의 `href="#"` 두 개)
4. CreoDent 상세 페이지 `work/creodent/` (아래 "CreoDent 재료" 참고)
5. 레주메 Brand 버전 글 → 6. Amigo 재구성 지시서
7. (나중) 실제 이미지로 목업 대체: 사용자가 소스를 주면 Claude가 넣는다. Starlight·LineLoomArt는 10/27 덱 아티팩트(`claude.ai/artifact/HWQ69xrravfgNiT4eSxu8R`, `img/star_ig5175.jpg`, `img/ll_sq3.jpg`)에서도 가져올 수 있다

### 사용자에게 받을 것
LinkedIn 주소 / (나중) 이미지 소스 / 브로슈어 종수·플라이어 대략 / 현재 레주메 텍스트 / Amigo 기존 자료

### 일하는 방식 메모 (세션 3에서 사용자가 요청)
- **CLAUDE.md는 세션 끝에 한 번만 업데이트한다. 중간에 일일이 고치지 않는다.**
- **토큰을 아낀다.** 스크린샷·렌더링은 꼭 필요할 때만. 판단·글은 길게, 반복 작업은 짧게.
- 만들기 전에 먼저 묻는다. "만들지 말고 셋업부터"라고 하면 대화로만.
- 출국 11/21. 11/20이 여유일. 밀리면 PDF 전환.
> 대화는 한국어로, 포트폴리오·레주메 결과물은 영어로 만듭니다.

### 세션 3에서 다른 에이전트(ChatGPT) 의견을 검토한 결론
- 가져온 것: About의 4문장 구조(observe / understand context / translate visually / bring to life), "Beyond the screen" 표.
- 거절한 것: "Multidisciplinary Designer" 타이틀, 세 서브브랜드 BI를 히어로에 쓰기(BI는 회사 것), 7섹션 구조, Roomeo 1순위, Figma 하이파이 먼저. 이유는 §1 "컨셉 메시지" 참고.

---

## CreoDent 재료 (세션 3에서 확인한 사실)

- **기간:** 인하우스 2024.08–2025.08 (뉴욕), 프리랜서 2026–현재 (INOSS 브로슈어 등)
- **세 서브브랜드:** Orion / Inosys(INOSS) / Creo. 분위기와 BI가 다 다르다. BI는 회사 것이고 사용자는 적용물을 만들었다. "하루에 세 브랜드를 오가며 이전 브랜드의 습관을 지우고 새로 시작했다"가 사용자의 실제 경험.
- **BI 브로슈어:** 브랜드 초기 설립·확장용. **Orion, INOSS는 직접 작업**, Creo는 커버 시안만.
- **숫자:** 영상 8편(사내행사 2, SNS 5, 행사 스케치 1, 촬영·편집 모두), 전시 **4회**(GNYDM + LMT East 2024, LMT Chicago 2025, LMT West 2025), 잡지 광고 14(LMT 10, Dentaltown 4), 이메일 블라스트(비정기, 횟수 모름 → "ad-hoc email campaigns"), 플라이어 있음. COTD 시리즈는 엎어짐(쓰지 않음).
- **eShop 상품 이미지:** 직접 촬영 → 보정 → 편집 전부. eCommerce 직무에 강한 카드.
- **내부 툴 2개 (Product 태그의 근거):**
  1. **사내 물품 주문 웹사이트:** 지점(허드슨밸리, 뉴욕)마다 유니폼·종이컵·패키지 박스·티슈 등을 매번 Slack으로 담당자에게 요청하던 것을 온라인 쇼핑처럼 주문하게 만든 내부 사이트. HR을 돕기 위해.
  2. **웰컴 인터랙션 스크린:** 로비에서 거래처·손님이 회사의 부서, 하는 일, 메인 가치를 보는 인터랙티브 화면. 전시회에서도 사용. 기기는 LG StanbyME.
  → 둘 다 화면 디자인이 별로라 **스크린샷 대신 "문제 → 만든 것 → 쓰인 곳" 흐름도**로 보여준다.
- **파일 위치 (사용자 Mac):** iCloud `Desktop/Desktop - 권유정의 MacBook Pro/Creodent`. 한글 경로는 NFD라 복사해 붙이면 안 열린다. `find "$HOME/Library/Mobile Documents/com~apple~CloudDocs" -maxdepth 3 -type d -iname "*creodent*"`로 찾는다. 주요 폴더: SNS/Video, Advertisement/Magazine, Show/(전시 4개), eShop/, Brochure/, Seminar/, Goods/, Interior/Monitor, For Confirmation(시안→컨펌 과정 증거). 파일 수는 소스 포함이라 제작물 수가 아니다.
- **상세 페이지 블록 순서:** ① SNS·영상·이메일 ② 전시 ③ eShop ④ 세미나 자료 ⑤ 브랜드 환경 + 내부 툴 ⑥ 인쇄(잡지·BI 브로슈어·플라이어). 첫 화면에 "Three brands, one desk".

---

## 0. Claude에게: 일하는 방식

- 세션을 시작하면 **"이번 주 목표 / 지난 진행 / 다음 할 일"**을 3줄로 먼저 정리한다.
- 결정이 필요하면 **선택지 2~3개와 추천안**을 보여주고 고르게 한다. 바로 적용하지 않는다.
- 기존 작업물은 보존하고, 큰 변경은 별도 버전으로 제안한다.
- 범위가 커지면(scope creep) 경고하고, 마감 기준으로 자를 부분을 제안한다.
- 디자인 설명은 실무자 수준으로, **코드·AI 설명은 쉬운 말로, Figma에 비유해서** 한다.
- 사용자는 **공부가 목적**이다. 코드를 짜면 무엇을 했는지 짧게 설명하고, 사용자가 **직접 고쳐볼 한 가지**를 제안한다.
- 파일을 정리할 때는 **절대 원본을 이동하거나 삭제하지 않는다. 복사만 한다.**
- 이 저장소는 포트폴리오 전용이다. 팀 프로젝트(BCA)는 `kwyj9848-stack/CICCC_FNL_PJ` 저장소에 있고, 그쪽 `CLAUDE.md`는 건드리지 않는다. BCA 자료가 필요할 때만 `add_repo`로 붙여서 **읽기만** 한다 (`bca-home.html`을 Playwright로 1440×1920, 7초 대기 후 촬영하면 히어로 제목까지 나온다).

---

## 1. 확정된 결정

| 항목 | 결정 |
|---|---|
| 경로 | **A: 밴쿠버 글로벌 브랜드(룰루레몬, 아크테릭스 등)의 Digital / eCommerce / Brand Designer로 입사 → 사내에서 Product로 이동.** 계약직(contract)과 크리에이티브 채용 에이전시도 같이 노린다 |
| 2단계 목표 | 1~2월에 케이스를 추가한 뒤 Product/UX 포지션(Microsoft 등)까지 넓힌다 |
| 사이트 | **Claude Code로 직접 제작** (이유: 공부). 기술은 **순수 HTML + CSS** (기본값). 호스팅은 **GitHub Pages** |
| 작업 환경 | Mac의 Claude 데스크톱 앱 → Claude Code, 또는 claude.ai/code 클라우드 세션. 둘 다 이 저장소를 쓴다 |
| 작업 폴더 | **홈 폴더의 `portfolio`** = 이 저장소. iCloud 폴더 안에서는 작업하지 않는다 |
| 출국 전 범위 | **A안: 한 페이지 사이트 v0** (소개 한 줄 + CreoDent 케이스 압축본 + BCA "진행 중" 카드 + 레주메 링크 + 연락처). 나머지는 한국에서 붙인다 |
| 첫 화면 문구 | 정보형 한 줄로 간다. 최종 문구는 현직자 포폴을 분석한 뒤 정한다. 임시 문구: *"Designer working across brand, marketing, and product. Based in Vancouver."* |
| 포트폴리오 흐름 | **Brand가 약속하고 → Marketing이 사람을 데려오고 → Product가 약속을 지킨다.** 케이스마다 `Brand` `Marketing` `Product` 태그를 단다 |
| 포폴 구조 (11/16 확정) | 한 페이지: **Hero(이름+정보형 한 줄+카드 줄) → Work(번호 리스트+태그) → About("How these connect") → Experience(성과 문장+숫자) → Contact.** About이 Work **뒤**에 오는 이유: 작품으로 먼저 신뢰를 만들고, 흐름 설명은 그 뒤에. Hero에 "How these connect →" 링크로 보완 |
| Hero 비주얼 (11/17 확정) | **LP 넘기기(레코드 크레이트)**: 커버들이 가로 줄로 서 있고 가운데만 정면. 레퍼런스는 cosmos.so/e/696464911 (다크) → **순백 #FFFFFF + 검정, 고대비**로. 색은 카드에서만. 카드 6장: CreoDent, Fraserview, BCA, Starlight, LineLoomArt, About(본인 사진). 구현은 CSS만, 모바일은 스와이프, 미지원 브라우저는 정적 |
| 컨셉 메시지 | **"Same method, different rooms."** 자아·직업을 나열하지 않는다. "Multidisciplinary"라는 단어는 쓰지 않는다. 적응력은 말로 주장하지 않고 작업물의 대비(세 서브브랜드 등)로 증명한다 |
| 케이스 4건 (11/16 확정) | 01 CreoDent (Brand·Marketing·Product) / 02 Fraserview (Product, 완료) / 03 BCA (Product, 진행 중) / 04 Amigo (Product, 혼자, 12월). Roomeo는 팀 과제라 Playground로. v0는 3줄만 공개, Amigo는 코드에 주석으로 대기 |
| CreoDent 케이스 틀 | "내가 다 바꿨다"가 **아니라** "한 브랜드를 여러 채널에서 빠르게 일관되게 + 클라이언트가 다시 찾는 사람". 제목 *A year in-house. Then they called me back.* 세 서브브랜드(Orion·Inosys·Creo, BI는 회사 것) 적용 경험은 Work 01 첫 화면에서 "Three brands, one desk"로. 비자 이야기는 쓰지 않는다 |
| 네일 | Experience에는 **넣지 않는다**(디자인 경력 아님). About "Beyond the screen" 한 줄만 (11/17) |
| 팀 프로젝트 | **BCA (Brazilian Community Association of BC) 웹사이트 리디자인** (CICCC 파이널). 역할: low-fi → mid-fi, 팀 전체 무드·디자인 시스템 통일(`DESIGN.md`), 이중언어·접근성. 7년차 개발자와 협업, Claude로 구현한 부분 포함 (11/16 확정) |
| 네일 경험 | 케이스 스터디가 **아니다**. **About**에서 "1:1 사용자 관찰, raw UX" 근거로 쓴다 (11/16 확정) |
| 앱 출시 | 별도 앱은 만들지 않는다. 12~1월에 **네일 서비스 AI 프로토타입(작동 링크)** 으로 대체 검토 (11/16 결정) |

---

## 2. 케이스 스터디 계획 (총 4건, 단계별 공개)

| 단계 | 케이스 | 레이어 | 범위 |
|---|---|---|---|
| **v0 (출국 전, ~11/20)** | **CreoDent** 상세 페이지 | Brand + Marketing + Product | 블록 순서: ① SNS·영상·이메일 ② 전시 4회 ③ eShop 상품 촬영·보정 ④ 세미나 자료 ⑥ 브랜드 환경(내부 툴 2개는 흐름도로) ⑤ 인쇄(잡지 14, BI 브로슈어 Orion·INOSS). 숫자: 영상 8편, 전시 4회(GNYDM + LMT 3), 잡지 광고 14, 이메일 비정기 |
| ✅ v0 | **Fraserview** | Product | 완료 (`work/fraserview/`) |
| v0 | **BCA** | Product | Work 줄 + 카드 (스크린샷 1장). 완성본은 한국에서 |
| v1 (한국 체류) | BCA 완성본 + **Amigo** 재구성 | Product | 북미 케이스 흐름: Overview → Problem → Research → Insights → Process → Solution → Outcome → Reflection |
| v2 (12~1월) | (선택) 네일 서비스 AI 프로토타입 — About에만 쓰기로 한 결정과 충돌하니 귀국 후 재결정 | — | — |
| 항상 | About + 레주메 (Visual/Brand 버전), Playground (이미지 몇 장) | — | v0부터 |

- 학교 과제: Fraserview(바이크샵 리디자인, Tak과 2인), Roomeo(룸메이트 매칭, 팀), Amigo(이민자·유학생 일반약 검색, 혼자). Roomeo는 Playground.
- **10/27 "Yujeong Kwon Portfolio" 아티팩트**(19장 인쇄형 덱, claude.ai/artifact/HWQ69xrravfgNiT4eSxu8R)에 CreoDent·Starlight·LineLoomArt·SMC·Ugly So Lovely 이미지가 이미 있다. 이미지 소스로 쓴다.
- 사이트 구조는 처음부터 케이스 4칸으로 만들고, 빈 칸은 "Coming soon"으로 둔다.

**안전장치:** 사이트가 늦어지면 CreoDent 케이스를 **PDF로 먼저 만들어 지원을 시작한다.**

---

## 3. 채용공고에서 뽑은 기준 (lululemon / Arc'teryx)

- **lululemon Graphic Designer (digital-first):** 웹, CRM 이메일, 유료 SNS, 캠페인을 아우르는 멀티채널 작업. After Effects / Premiere 우대 → **1순위 타깃 포지션 유형**
- **lululemon Senior Digital Designer:** Figma·Adobe, 개발자와 협업
- **lululemon UX Designer, Design Systems:** 처음부터 끝까지의 프로세스, 재사용 컴포넌트
- **Arc'teryx UX/UI:** 리서치, 정보 구조(IA), 프로토타이핑, 시각 커뮤니케이션
- 시사점: **영상 편집 경험을 보여준다 / 개발자 협업을 보여준다 / 디자인 시스템을 보여준다.** BCA 케이스가 뒤의 두 개를 직접 증명한다

---

## 4. 공부 계획

**방법: 만들면서 배우기 루프 (매 작업마다)**
1. 작은 목표 하나 정하기 → 2. Claude Code에게 시키기 → 3. "쉬운 말로, Figma에 비유해서 설명해줘" → 4. **한 가지는 내 손으로 직접 고치기** → 5. 3줄 학습 일지 쓰기 (`study-log.md`)

**핵심 개념:** HTML(레이어 구조) / CSS(Fill·Auto Layout·Text Style) / CSS 변수(Figma Variables) / Git·GitHub(Version History) / 배포(Publish 링크)

**시간:** 하루 4시간. 대략 공부+제작 2시간, 콘텐츠(자료·글) 2시간.

**참고 자료 (막힐 때만):** MDN Learn Web Development / web.dev Learn CSS / Claude Code 공식 문서

---

## 5. 일정

| 기간 | 할 일 |
|---|---|
| **지금 ~ 출국 전** | ① ✅ Claude 앱 설치 ② CreoDent 파일 고르기 (블록당 2~3장) ③ ✅ GitHub 저장소 + Pages ④ CreoDent 케이스 글과 페이지 ⑤ About + 레주메 ⑥ 사이트 공개 + 첫 지원 5~10건 + 에이전시 등록 |
| 한국 방문 (11월 말~12월 중순) | 가벼운 공부, BCA 완성본, 학교 과제 1건, 커피챗 메시지 보내기 |
| 12~1월 | 학교 과제 1건 더, (선택) 네일 AI 프로토타입. 커피챗 주 2~3건 |
| 1~2월 | v2 공개, Product 포지션까지 지원 확대, 면접 |
| 늦어도 3월 | 입사, 480시간 시작 |

출국일 **11/21 확정**. 귀국 날짜는 확인 필요.

### 출국 전 상세 일정 (A안, 하루 4시간)

| 날짜 | 공부·제작 | 콘텐츠 |
|---|---|---|
| 11/16 | ✅ Claude 앱, `portfolio` 폴더, ✅ GitHub 저장소 + 빈 페이지 | ✅ 흐름 확정, ✅ Fraserview 포폴 버전 |
| 11/17 | ✅ 페이지 뼈대 + 카드 회전 + BCA 카드 | ✅ 바디카피 v1, CreoDent 숫자 정리 |
| 11/18 | **히어로/랜딩 전체 틀 (목업)** | CreoDent 상세 페이지 글 |
| 11/19 | 색·폰트·여백 (CSS 변수), 모바일 확인 | 레주메 Brand 버전 |
| 11/20 | 최종 점검 → **공개** | 첫 지원 3~5건 또는 에이전시 등록. 짐 싸기 |

밀리면 11/20이 여유 시간이다. 그래도 안 되면 **PDF로 전환**한다.

---

## 6. 다음 할 일 (체크리스트)

- [x] Mac에 Claude 데스크톱 앱 설치 → `portfolio` 폴더 생성
- [x] GitHub 저장소 만들기 (`kwyj9848-stack/portfolio`) + 빈 `index.html`
- [x] GitHub Pages 켜기
- [x] 포트폴리오 흐름 잡기 → 구조·컨셉·바디카피 v1 확정 (index.html에 반영됨)
- [x] 학교 과제 → Fraserview, Amigo 채택
- [x] BCA 스크린샷 → 카드 (`img/bca-home.jpg`)
- [ ] 히어로/랜딩 전체 틀 (이미지는 목업)
- [ ] (나중) 사용자 소스로 목업 대체
- [ ] LinkedIn 주소, 레주메 PDF 연결
- [x] 비주얼 레퍼런스 (cosmos 레코드 크레이트, `archive/refs/`)
- [ ] CreoDent 상세 페이지
- [ ] CreoDent 파일: iCloud `Desktop - 권유정의 MacBook Pro/Creodent` 폴더 (한글 경로는 NFD라 복사해 붙이면 안 열림; `find -iname "*creodent*"`로 찾기). 블록당 2~3장만 고르면 됨. 과거 검색 기준(2024.08–2025.08, **바탕화면 두 곳 모두** (로컬 Desktop + iCloud의 "Desktop - 권…" 폴더), 회사 Drive·Dropbox, 이메일, 회사 인스타·웹사이트 스크린샷
- [ ] 기억나는 숫자 적기 (제작 수량, 기간, 반응·결과)
- [ ] CreoDent에 포트폴리오 사용 가능한지 짧게 확인
- [ ] (보조) 링크드인에서 lululemon·Arc'teryx 현직 Digital/eCommerce/Brand Designer 중 포폴 링크가 있는 5명 찾기 → 비교 분석

---

## 7. 미결 사항

- [ ] 한국 귀국 날짜
- [ ] 자격증(외국어교육관리사 1급, 2026.06)을 레주메에 어떻게 쓸지 (A 빼고 스토리로만 / B 맨 아래 한 줄)
- [ ] 브로슈어 종수, 플라이어 대략, eShop 제품 종수
- [ ] Amigo 기존 자료 (링크 또는 스크린샷)
- [ ] 현재 레주메 텍스트
- [ ] 한국 방문 기간 공부 강도
- [ ] 장기 체류(영주권 등) 경로 → 공인 이민 컨설턴트에게 따로 확인

---

## 8. 사용자 프로필 요약

- **위치·신분:** 밴쿠버 다운타운. CICCC UX/UI 학업 파트는 11월 말 종료. 코업 퍼밋이 끝나면 워킹홀리데이(오픈 워크퍼밋)로 전환 예정
- **디플로마:** 학업 종료 후 6개월 안에 디자이너 직무로 480시간 근무하면 받음. **보너스로 취급**하고, 이것 때문에 더 좋은 기회를 포기하지 않는다
- **목표:** 1년 안에 이름 있는 회사의 디자이너 → 2년 안에 Product Designer → 5년 안에 북미 대기업 Senior/Lead. 첫 직장은 연봉보다 이름값. 꿈의 장면: 내가 참여한 제품을 영어로 키노트처럼 발표하기
- **포지셔닝 (북극성):** Brand-minded Product Designer who imagines boldly and ships with AI. 공통분모: 상상한 것을 사람이 보고 만지고 느끼는 경험으로 만드는 사람
- 한 분야만 하는 디자이너가 아니다: 브랜딩, 마케팅, 시각·그래픽·편집, UX/UI, 프리랜스, 네일 아트, 과거 미술 강사·영어 스터디 강사. **경력이 시간순이 아니라 동시에 진행된다** → 약점이 아닌 강점으로 보여줄 구조가 필요

**경력 (레주메 재료)**
- CreoDent, New York: Marketing 2D Graphic Designer, **2024.08–2025.08** (11/16 확정; 이전 기록 2023–24는 오류). 브로슈어, 잡지·SNS 광고, SNS 템플릿, 브랜딩, 카드뉴스, 배송 카드, 사진·영상 촬영 및 편집, 전시회 출장(LMT, Greater New York Dental Meeting). 정규직 전환 제안을 받았으나 비자 문제로 종료
- CreoDent: Freelance Designer, **2024–현재** (프로젝트 단위)
- 한국 회사 디자인팀: SNS Content Designer Intern, **2023.01–2023.06**
- 한국 미술학원 SNS 마케팅 (릴스, 블로그, 인스타그램): 원격, 진행 중
- N.BAR Vancouver: Nail Technician, 2026.06–현재
- 미술 강사: 3개월 (과거)
- 영어 스터디 강사: 한국에서 **성인 대상** (과거)
- **외국어교육관리사 1급**, 컬쳐컴플렉스 평생교육원, **2026.06**
- Etsy: Canva 웨딩 웹사이트 템플릿 셀러 (리스팅 3개)
- 수상: 졸업전시 105명 중 4위, Mediheal 최우수상, KSDS 우수 졸업작품, 디자인클라우드 100선

**지금 하지 않을 것:** Etsy 신규 리스팅 확장, 빅테크 신입 Product 포지션 집중 (나중에), 별도 앱 출시
