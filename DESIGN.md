# Minimal 3D Educational Image Design Guide

이 문서는 Git, SSR, CSR 같은 개발 개념을 설명하는 이미지를 일관된 스타일로 생성하기 위한 디자인 가이드입니다.

## 목표

- 복잡한 기술 개념을 한눈에 이해되는 은유로 표현한다.
- 발표 슬라이드나 교육 자료에 바로 넣을 수 있는 차분하고 심플한 이미지를 만든다.
- 이미지마다 스타일은 통일하되, 개념별 은유와 구도는 다르게 잡는다.

## 기본 스타일

다음 키워드를 기본 스타일로 사용합니다.

```text
minimalist 3D isometric illustration
clean modern educational slide style
soft neutral background
lots of whitespace
restrained color palette
warm coral, muted teal, soft blue, off-white accents
smooth rounded edges
soft shadows
minimal 3D objects
16:9 wide image
```

한국어로 설명하면:

- 미니멀한 3D 아이소메트릭 일러스트
- 교육용 슬라이드에 어울리는 깨끗한 구성
- 넓은 여백
- 부드러운 중립 배경
- 코랄, 틸, 소프트 블루, 오프화이트 중심의 제한된 색상
- 둥근 모서리와 부드러운 그림자
- 장식보다 개념 전달을 우선하는 단순한 사물

## 피해야 할 것

프롬프트 끝에 다음과 같은 금지 조건을 넣으면 스타일이 안정됩니다.

```text
no characters
no clutter
no realistic supermarket aisles
no toy workshop details
no browser imagery unless needed
no GitHub remote/cloud imagery unless needed
no extra text
```

특히 Git 이미지를 만들 때는 SSR/CSR 브라우저 이미지가 섞이지 않도록 하고, SSR/CSR 이미지를 만들 때는 Git 커밋 큐브나 원격 저장소 구름이 섞이지 않도록 명시합니다.

## 프롬프트 구조

좋은 프롬프트는 보통 아래 구조를 따릅니다.

```text
Create a minimalist 3D isometric illustration symbolizing "[concept]".

Style:
[shared style keywords]

Concept:
[one-sentence metaphor]

Composition:
[left/center/right or top/bottom layout]

Motion:
[what moves from where to where]

Labels:
[allowed labels only]

Avoid:
[things to exclude]
```

핵심은 단순히 "git add 이미지를 그려줘"라고 하지 않고, 다음 다섯 가지를 같이 주는 것입니다.

- `Style`: 어떤 그림체인지
- `Concept`: 무엇을 어떤 은유로 표현하는지
- `Composition`: 화면에서 무엇이 어디에 있는지
- `Motion`: 흐름의 방향이 무엇인지
- `Avoid`: 헷갈리는 요소를 무엇을 빼야 하는지

## 공통 색감

정확한 색상값을 지정해야 할 때는 아래 팔레트를 참고합니다.

```text
Background: #F7F5F0
Warm coral: #D87963
Muted teal: #6FA7A1
Soft blue: #8DB7D9
Off-white: #FFFDF7
Text dark: #2B2B2B
Soft shadow: rgba(43, 43, 43, 0.14)
```

이미지 생성 프롬프트에는 보통 색상 이름만 넣어도 충분합니다. UI나 슬라이드 템플릿을 직접 만들 때는 색상값을 사용합니다.

## Git 이미지 패턴

### git add

은유: 작업 파일을 장바구니에 담아 스테이징 영역으로 옮긴다.

```text
Create a minimalist 3D isometric illustration symbolizing "git add" for a clean modern educational slide.
Use a soft neutral background, lots of whitespace, restrained palette with warm coral, muted teal, soft blue, and off-white accents, smooth rounded edges, soft shadows, minimal 3D objects.
Concept metaphor: adding changed files to the staging area is like putting products into a shopping cart.
Composition: on the left, several simple file cards sitting in a clean area labeled "Working Directory". In the center/right, a minimal shopping cart or basket labeled "Staging Area". A few file cards are floating or sliding into the cart, with a thin clean arrow showing movement from Working Directory into Staging Area. Add a small badge that says "git add".
Keep it minimal and polished, no characters, no clutter, no realistic supermarket aisles, no GitHub remote/cloud imagery, no browser imagery.
16:9 wide image. No extra text besides "git add", "Working Directory", and "Staging Area".
```

### git add + git commit

은유: 파일을 카트에 담고, 그 내용을 하나의 커밋 상자로 포장한다.

```text
Create a minimalist 3D isometric illustration explaining "git add" followed by "git commit" in one simple flow.
Use a clean modern educational slide style with soft neutral background, lots of whitespace, restrained palette with warm coral, muted teal, soft blue, and off-white accents, smooth rounded edges, soft shadows, minimal 3D objects.
Composition with three clear steps left to right:
1. Left side labeled "Working Directory" with a few simple file cards.
2. Center labeled "Staging Area" with a minimal shopping cart or basket; several file cards are visibly moving into the cart along a thin arrow labeled "git add".
3. Right side labeled "Commit" with the staged files transformed into one compact sealed snapshot box with a small check mark; a thin arrow from the cart to the box labeled "git commit".
Above the Commit box, add a small clean symbolic Git history graph: 4 or 5 circular commit nodes connected by thin branching and merging lines.
Keep it simple and uncluttered, no characters, no supermarket aisles, no remote/cloud/GitHub imagery, no push/pull imagery, no browser imagery.
16:9 wide image. No extra text besides "Working Directory", "Staging Area", "Commit", "git add", and "git commit".
```

### git push

은유: 로컬 저장소에서 원격 저장소로 커밋을 보낸다.

```text
Create a minimalist 3D isometric illustration symbolizing "git push", matching a clean modern educational slide style.
Concept: local repository sends commits up to GitHub remote.
Minimal shapes, soft neutral background, lots of whitespace, restrained color palette with warm coral, muted teal, soft blue, and off-white accents, smooth rounded edges, soft shadows.
Composition: left/bottom side has a simple local repository block or tray labeled "Local Repository" containing a few small commit cubes with git branch symbols. Right/top side has a simple cloud/server block labeled "GitHub Remote". A thin clean arrow or subtle glowing line carries two commit cubes from Local Repository toward GitHub Remote. Add a small central label "git push".
Make direction unmistakable: local to remote.
Very minimal, no clutter, no characters, no code page/browser imagery.
16:9 wide image. No extra text besides "git push", "Local Repository", and "GitHub Remote".
```

### git pull

은유: 원격 저장소에서 내려온 변경사항이 로컬 트레이에 정리되어 들어온다.

```text
Create a minimalist 3D isometric illustration symbolizing "git pull", visually distinct from a companion git push image while keeping the same clean modern educational slide style.
Concept: pulling updates from GitHub Remote into the local repository, like a neat download tray receiving remote changes.
Minimal shapes, soft neutral background, lots of whitespace, restrained palette with warm coral, muted teal, soft blue, and off-white accents, smooth rounded edges, soft shadows.
Composition: place a compact cloud/server icon labeled "GitHub Remote" near the upper center, and below it a larger open local folder/tray labeled "Local Repository". From the cloud, a vertical soft blue download beam or thin downward path lowers several small commit cards/cubes with git branch symbols into the open local tray. Inside the tray, show the incoming commits snapping into an ordered stack beside existing local blocks, suggesting updates being received and integrated. Add a small badge that says "git pull".
Make this feel paired with git push through color and minimal 3D style, but use a different metaphor and layout: download beam, receiving tray, organized stack.
No clutter, no characters, no browser imagery.
16:9 wide image. No extra text besides "git pull", "Local Repository", and "GitHub Remote".
```

## SSR / CSR 이미지 패턴

### SSR

은유: 서버가 완성된 HTML을 먼저 만들고, 빈 브라우저로 보낸다.

```text
Create a minimalist 3D isometric illustration symbolizing SSR, Server-Side Rendering, matching a clean modern educational slide style.
Concept: the server prepares a complete rendered HTML page first, then sends it to an empty browser.
Soft neutral background, lots of whitespace, restrained color palette with warm coral, muted teal, soft blue, and off-white accents, smooth rounded edges, soft shadows.
Composition: left side has a simple server block labeled "Server" with a finished web page card labeled "Ready HTML" emerging from it. The Ready HTML card already contains simple geometric UI blocks: header bar, text lines, image rectangle, and button blocks. The card is moving along a thin clean arrow toward the right. Right side has a large browser frame labeled "Browser" with its interior still blank white or very pale, waiting to receive the page. Add a small central label "SSR".
Make the flow unmistakable: complete HTML is built on the server side and is currently entering the empty browser.
No JavaScript assembly inside the browser, no Git imagery.
16:9 wide image. No extra text besides "SSR", "Server", "Browser", and "Ready HTML".
```

### CSR

은유: 서버는 빈 HTML과 JS 번들만 보내고, 브라우저가 직접 화면을 조립한다.

```text
Create a minimalist 3D isometric illustration symbolizing CSR, Client-Side Rendering, based on this idea: the server sends only Empty HTML and a JS Bundle, and the browser builds the page itself.
Clean modern educational slide style, minimal shapes, soft neutral background, restrained color palette with warm coral, muted teal, soft blue, and off-white accents.
Composition: left side has a simple small server block labeled "Server". From it, two clean floating cards move toward the right: one labeled "Empty HTML" as a mostly blank page outline, and one labeled "JS Bundle" as a compact stack of code blocks. Right side has a large browser frame labeled "Browser". Inside the browser, simple geometric UI blocks are being assembled: a header bar, text lines, image rectangle, and button blocks snapping into place. Add a small central label "CSR". Use subtle arrows or thin glowing lines showing flow from server to browser.
Very minimal, lots of whitespace, smooth rounded edges, soft shadows, no clutter, no characters, no Git imagery.
16:9 wide image. No extra text besides "CSR", "Server", "Browser", "Empty HTML", and "JS Bundle".
```

## 좋은 결과를 얻는 팁

- 한 이미지에는 하나의 핵심 은유만 둡니다.
- 여러 개념을 넣어야 하면 2단계 또는 3단계 흐름으로 제한합니다.
- 텍스트는 3-5개 이하로 제한합니다.
- "visually distinct from..."을 넣으면 비슷한 이미지의 단순 반전을 피하는 데 도움이 됩니다.
- "No extra text besides..."를 넣으면 모델이 불필요한 단어를 추가하는 것을 줄일 수 있습니다.
- 같은 시리즈를 만들 때는 스타일 문장은 고정하고, Concept와 Composition만 바꿉니다.
- 결과가 너무 비슷하면 은유 자체를 바꿉니다. 예: `git pull`은 단순 반대 화살표 대신 다운로드 트레이.

## 새 이미지 요청 템플릿

아래 템플릿의 대괄호 부분만 바꿔 사용합니다.

```text
Create a minimalist 3D isometric illustration symbolizing "[CONCEPT]" for a clean modern educational slide.
Use a soft neutral background, lots of whitespace, restrained palette with warm coral, muted teal, soft blue, and off-white accents, smooth rounded edges, soft shadows, minimal 3D objects.
Concept metaphor: [METAPHOR].
Composition: [LAYOUT AND OBJECTS].
Motion: [FLOW DIRECTION].
Add a small badge that says "[LABEL]".
Keep it minimal and polished, no characters, no clutter, no unrelated imagery.
16:9 wide image. No extra text besides [ALLOWED TEXT LABELS].
```
