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
| 클릭으로 가사 쓰기 | 빈 캔버스를 클릭하면 입력창이 열려요. 스페이스바로 블록 완성 후 다음 칸으로 이동해요. |
| 실시간 미리보기 | 입력하는 글자가 캔버스 위에 실시간으로 표시돼요. |
| Canva 스타일 툴바 | 텍스트 선택 시 상단에 서식 툴바가 고정 표시돼요. |
| 슬라이드 방향 조정 | 슬라이드(글라이드) 블록의 끝점 핸들을 드래그해 방향을 자유롭게 바꿀 수 있어요. |
| 폰트 선택 | Pretendard GOV, Gaegu, Noto Sans KR, 나눔명조, Dongle 등 선택 가능해요. |
| 줄 높이 조정 | 컨트롤 바에서 캔버스 줄 높이를 좁게/현재 중 선택할 수 있어요. |
| 마디 추가/제거 | 컨트롤 바의 마디 ± 버튼으로 곡 길이를 자유롭게 늘릴 수 있어요. |
| 노래 익히기 / 가사 쓰기 탭 | 원곡 위에서 새 가사를 만드는 작업 모드를 지원해요. |
| 줄 가이드 | 음 높낮이 가이드 줄(1~5개) 또는 자유 배치 모드를 선택할 수 있어요. |
| 색·크기·폰트 조정 | 블록별로 폰트 크기, 색깔, 서체를 바꿀 수 있어요. |
| 한·영·일 다국어 | 인터페이스 언어를 선택할 수 있어요. |
| JSON 저장 / 공유 링크 | 작업을 파일로 저장하거나 링크 하나로 다른 기기에서 열 수 있어요. |
| PNG 다운로드 / 클립보드 복사 | 완성된 악보를 이미지로 내보낼 수 있어요. |

## 🚀 사용 방법

1. **헤더의 ❓ 아이콘**을 눌러 사용 방법을 확인하세요. 모달 우측의 **예시 보기** 버튼을 누르면 샘플 악보(반짝반짝 작은 별)를 바로 불러옵니다.
2. 캔버스를 **클릭**해서 가사를 입력합니다. **스페이스바**를 누르면 블록이 완성되고 다음 위치로 이동해요.
3. 글자 블록을 **드래그**해서 음의 높낮이를 정합니다.
4. 블록 양옆 핸들을 잡고 **늘이면** 길게 부르는 음이 돼요.
5. 블록을 선택하면 상단에 **서식 툴바**가 나타나요. 폰트·크기·색상·슬라이드를 조정할 수 있어요.
6. 마디가 부족하면 컨트롤 바의 **마디 + 버튼**을 눌러 늘리세요.
7. 다 그렸으면 **💾 저장**(JSON) 또는 **🔗 공유**(이미지/링크)로 내보내세요.

## ⌨️ 키보드 단축키

| 키 | 동작 |
| --- | --- |
| **클릭** | 빈 캔버스에 텍스트 입력 시작 |
| **스페이스바** | 현재 블록 완성 후 다음 칸으로 이동 |
| **Tab** | 스페이스바와 동일 (다음 칸 이동) |
| **Enter** | 입력 마침 |
| **Esc** | 입력 취소 / 선택 해제 |
| **더블클릭** | 기존 블록 편집 |
| **Delete / Backspace** | 선택된 블록 삭제 |
| **F2** | 선택된 블록 편집 |

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
- **Click** the canvas to start typing; **Space** confirms a block and moves to the next position
- Real-time text preview appears on the canvas while typing
- Canva-style toolbar at the top of the canvas for formatting (font, size, color, slide)
- Drag a block up/down for pitch; drag side handles to stretch for held notes
- Drag the slide endpoint handle to change glide direction

**Tech:**
- Pure HTML / CSS / Vanilla JS, no build step
- Single-file deploy (`index.html`)
- JSON save / shareable URL / PNG export
- Korean · English · Japanese UI
