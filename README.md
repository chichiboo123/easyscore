# 너를 위한 악보 · Easy Score

> 어린이도 쉽게 가사와 멜로디를 그릴 수 있는 시각적 악보 도구  
> A visual lyric-and-melody score editor — no music theory required.

---

> ⚠️ **아이디어 존중 부탁드립니다**  
> 이 프로젝트는 교육 현장에서 직접 경험하고 고안한 아이디어를 바탕으로 만들어졌습니다.  
> 코드는 MIT 라이선스로 공개되어 있지만, 아이디어와 콘셉트의 독창성은 존중받기를 바랍니다.  
> 상업적 활용이나 유사 서비스 제작 시에는 출처를 명시해 주세요.  
>
> ⚠️ **Please respect the original idea**  
> The concept was developed from hands-on classroom experience. The code is MIT-licensed, but please credit the original idea if you build something similar or use it commercially.

---

## ✨ 이런 도구입니다

악보를 읽지 못해도, 누구나 **가사의 위치와 길이만으로 멜로디를 표현**할 수 있어요.  
초등학생 음악 수업, 동요 만들기 활동, 노래 익히기 자료 제작에 사용됩니다.

- **글자 = 음표** : 가사 한 묶음이 하나의 음 블록이에요.
- **위 = 높은 음 / 아래 = 낮은 음** : 글자를 위아래로 드래그해 음정을 표현해요.
- **블록 가로 길이 = 음표 길이** : 양옆 핸들로 길게 늘이면 길게 부르는 음이에요.
- **슬라이드** : 글라이드(미끄러지는 음)는 곡선 위 텍스트로 표현돼요. 슬라이드 끝점 핸들로 방향도 바꿀 수 있어요.

## 🎵 주요 기능

| 기능 | 설명 |
| --- | --- |
| 클릭한 자리에 입력창 | 빈 캔버스를 클릭하면 그 자리 바로 위에 입력창이 떠요. 스페이스/Enter로 다음 칸·마침. |
| 실시간 미리보기 | 입력하는 글자가 캔버스 위에 실시간으로 표시돼요. |
| 글자 블록 이동 | 글자에 마우스를 올리면 ✊ 커서가 뜨고, 드래그로 자유롭게 옮길 수 있어요. |
| 텍스트 편집 | 글자 블록을 더블클릭하거나 상단 도구막대의 ✎ **편집** 버튼으로 텍스트를 수정해요. |
| 다중 선택 (드래그) | 빈 캔버스를 드래그하면 사각형 안의 글자를 한꺼번에 선택해요. Shift+클릭으로 개별 추가/제거, Ctrl/⌘+A로 전체 선택. |
| 일괄 이동·수정 | 여러 글자를 한 번에 옮기고, 크기·색·폰트·슬라이드를 일괄 적용해요. |
| 복사 / 붙여넣기 | Ctrl/⌘+C로 복사, Ctrl/⌘+V로 붙여넣기. 다중 선택 그대로 복제돼요. |
| 실행 취소 / 다시 실행 | Canva 스타일 무제한(80단계) Undo/Redo. Ctrl/⌘+Z, Ctrl/⌘+Shift+Z 또는 헤더 ↶ ↷ 버튼. |
| 원곡 가사 불러오기 | '가사 쓰기' 탭의 새 가사 영역에서 원곡 가사 전체를 그대로 복제해요. 이후 텍스트만 바꿔 쓰면 됩니다. |
| 키보드 이동 | 선택된 글자를 화살표 키로 미세 이동 (Shift+화살표는 큰 폭). |
| Canva 스타일 툴바 | 텍스트 선택 시 상단에 서식 툴바가 고정 표시돼요. |
| 슬라이드 방향 조정 | 슬라이드(글라이드) 블록의 끝점 핸들을 드래그해 방향을 자유롭게 바꿀 수 있어요. |
| 폰트 선택 | Pretendard GOV, Gaegu, Noto Sans KR, 나눔명조, Dongle 등 선택 가능. |
| 줄 높이 조정 | 컨트롤 바에서 캔버스 줄 높이를 좁게/현재 중 선택. |
| 마디 추가/제거 | 컨트롤 바의 마디 ± 버튼으로 곡 길이를 자유롭게 조절. |
| 노래 익히기 / 가사 쓰기 탭 | 원곡 위에서 새 가사를 만드는 작업 모드를 지원. |
| 줄 가이드 | 음 높낮이 가이드 줄(1~5개) 또는 자유 배치 모드 선택. |
| 색·크기·폰트 조정 | 블록별로 폰트 크기, 색깔, 서체를 바꿀 수 있어요. |
| 한·영·일 다국어 | 인터페이스 언어 선택 가능. |
| JSON 저장 / 공유 링크 | 작업을 파일로 저장하거나 링크 하나로 다른 기기에서도 열 수 있어요. |
| PNG 다운로드 / 클립보드 복사 | 완성된 악보를 이미지로 내보낼 수 있어요. |

## 🚀 사용 방법

1. **헤더의 ❓ 아이콘**을 눌러 사용 방법을 확인하세요. 모달 우측의 **예시 보기** 버튼을 누르면 샘플 악보(반짝반짝 작은 별)를 바로 불러옵니다.
2. 캔버스의 원하는 위치를 **클릭**하면 그 자리 위에 입력창이 뜹니다. 글자를 쓰고 **스페이스바**(다음 칸) 또는 **Enter**(마침)로 확정하세요.
3. 만들어진 글자 블록을 **드래그**해서 음의 높낮이를 정하세요. 양옆 핸들을 잡고 늘이면 길게 부르는 음이 됩니다.
4. 글자 블록을 클릭하면 위에 **서식 툴바**가 나타나요. 폰트·크기·색상·슬라이드·편집·삭제를 조절할 수 있어요. **편집(✎)** 또는 **더블클릭**으로 텍스트를 수정합니다.
5. 빈 공간을 **드래그**하면 사각형 안의 글자를 한꺼번에 선택할 수 있어요. 선택된 글자는 같이 옮기거나 일괄 수정할 수 있고, **Ctrl/⌘+C → Ctrl/⌘+V**로 복제할 수 있어요.
6. 실수했을 때는 **Ctrl/⌘+Z**로 되돌리고 **Ctrl/⌘+Shift+Z**로 다시 실행하세요. 헤더의 **↶ ↷** 버튼도 같은 기능입니다.
7. **가사 쓰기** 탭에서는 **'원곡 가사 불러오기'** 버튼으로 원곡 가사를 새 가사 영역에 그대로 복제할 수 있어요. 그다음 텍스트만 바꿔 쓰면 가사 바꿔 부르기 활동에 바로 쓸 수 있습니다.
8. 마디가 부족하면 컨트롤 바의 **마디 + 버튼**을 눌러 늘리세요.
9. 다 그렸으면 **💾 저장**(JSON) 또는 **🔗 공유**(이미지/링크)로 내보내세요.

## ⌨️ 키보드 단축키

| 키 | 동작 |
| --- | --- |
| **클릭** | 빈 캔버스에 텍스트 입력 시작 (클릭한 위치에 입력창) |
| **스페이스바** | 현재 블록 완성 후 다음 칸으로 이동 |
| **Tab** | 스페이스바와 동일 |
| **Enter** | 입력 마침 |
| **Esc** | 입력 취소 / 선택 해제 |
| **더블클릭** | 기존 블록 편집 |
| **F2** | 선택된 블록 편집 |
| **Delete / Backspace** | 선택된 블록 삭제 |
| **드래그(빈 공간)** | 사각형 다중 선택 |
| **Shift+클릭** | 선택에 추가/제거 |
| **Ctrl/⌘+A** | 현재 탭의 모든 블록 선택 |
| **Ctrl/⌘+C** | 선택된 블록 복사 |
| **Ctrl/⌘+X** | 선택된 블록 잘라내기 |
| **Ctrl/⌘+V** | 붙여넣기 (현재 탭 패널에) |
| **Ctrl/⌘+Z** | 실행 취소 (Undo) |
| **Ctrl/⌘+Shift+Z**, **Ctrl/⌘+Y** | 다시 실행 (Redo) |
| **방향키** | 선택된 블록 미세 이동 (Shift+방향키: 큰 폭 이동) |

## 🛠 기술 스택

- **순수 HTML / CSS / Vanilla JS** — 빌드 단계 없이 정적 파일 하나로 동작합니다.
- **SVG** — 모든 악보 요소(블록·가이드 줄·곡선)는 인라인 SVG로 렌더링됩니다.
- **html2canvas** — PNG 내보내기에 사용 (CDN 로드).
- **폰트** : Pretendard GOV · Black Han Sans · Gaegu · Fraunces · Zen Maru Gothic · Noto Sans KR · 나눔명조 · Dongle · Material Symbols Rounded

## 💻 로컬 실행

별도의 설치 없이 `index.html` 하나만 열면 됩니다.

```bash
git clone https://github.com/chichiboo123/easyscore.git
cd easyscore
# 아무 정적 파일 서버나 OK — 클립보드 API를 위해 http(s) 권장
python3 -m http.server 8000
# → http://localhost:8000 접속
```

## 📦 파일 구조

```
.
├── index.html   # 앱 전체 (HTML + CSS + JS 인라인)
└── README.md
```

## 🙏 만든 사람

[교육뮤지컬 꿈꾸는 치수쌤](https://litt.ly/chichiboo)

---

## English summary

**Easy Score** is a kid-friendly visual score editor built for music classrooms.  
Lyrics become draggable blocks whose vertical position represents pitch and whose horizontal length represents note duration.

**Key interactions:**
- **Click** a spot on the canvas → input bar appears right there; **Space** moves to the next position, **Enter** finishes
- Drag a text block up/down for pitch; drag side handles to stretch for held notes
- Drag the slide endpoint handle to change glide direction
- Double-click a block (or use the ✎ Edit button on the top toolbar) to change its text
- **Drag on empty canvas** to select multiple blocks; Shift+click to toggle, Ctrl/⌘+A to select all
- **Ctrl/⌘+C / V** to copy & paste selected blocks (paste targets the current tab's panel)
- **Ctrl/⌘+Z** to undo and **Ctrl/⌘+Shift+Z** to redo — up to 80 steps, Canva-style
- In the **Write** tab, the **"Copy original lyrics"** button duplicates the original score into the new-lyrics panel, so you only need to change the text

**Tech:**
- Pure HTML / CSS / Vanilla JS, no build step
- Single-file deploy (`index.html`)
- JSON save / shareable URL / PNG export
- Korean · English · Japanese UI
