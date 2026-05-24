# 너를 위한 악보 · Easy Score

> 어린이도 쉽게 가사와 멜로디를 그릴 수 있는 시각적 악보 도구
> A visual lyric-and-melody score for kids — no music theory required.

[👉 바로 사용해 보기](https://chichiboo123.github.io/easyscore/) <!-- update if the page is hosted elsewhere -->

---

## ✨ 이런 도구입니다

악보를 읽지 못해도, 누구나 **가사의 위치와 길이만으로 멜로디를 표현**할 수 있어요.
초등학생 음악 수업, 동요 만들기 활동, 노래 익히기 자료 제작에 사용됩니다.

- **글자 = 음표** : 가사 한 묶음이 하나의 음 블록이에요.
- **위 = 높은 음 / 아래 = 낮은 음** : 글자를 위아래로 드래그해 음정을 표현해요.
- **블록 가로 길이 = 음표 길이** : 양옆 핸들로 길게 늘이면 길게 부르는 음이에요.
- **슬라이드** : 글라이드(미끄러지는 음)는 곡선 위 텍스트로 표현돼요.

## 🎵 주요 기능

| 기능 | 설명 |
| --- | --- |
| 클릭으로 가사 쓰기 | 빈 캔버스를 더블클릭하면 입력창이 열려요. |
| **띄어쓰기 = 블록 분리** | `반짝 반짝 작은 별` 한 번에 입력하면 4개 블록이 만들어져요. |
| 마디 추가/제거 | 컨트롤 바의 마디 ± 버튼으로 곡 길이를 자유롭게 늘릴 수 있어요. |
| 좌우 스크롤 | 긴 곡은 캔버스를 가로로 스크롤해서 표시해요. |
| 노래 익히기 / 가사 쓰기 탭 | 원곡 위에서 새 가사를 만드는 작업 모드를 지원해요. |
| 줄 가이드 | 음 높낮이 가이드 줄(1~5개) 또는 자유 배치 모드를 선택할 수 있어요. |
| 색·크기 조정 | 블록별로 폰트 크기와 색깔을 바꿀 수 있어요. |
| 한·영·일 다국어 | 인터페이스 언어를 선택할 수 있어요. |
| JSON 저장 / 공유 링크 | 작업을 파일로 저장하거나 링크 하나로 다른 기기에서 열 수 있어요. |
| PNG 다운로드 / 클립보드 복사 | 완성된 악보를 이미지로 내보낼 수 있어요. |

## 🚀 사용 방법

1. **헤더의 ❓ 아이콘**을 눌러 사용 방법을 확인하세요. 모달 우측의 **예시 보기** 버튼을 누르면 샘플 악보(반짝반짝 작은 별)를 바로 불러옵니다.
2. 캔버스를 **더블클릭**해서 가사를 입력합니다. 띄어쓰기를 넣으면 자동으로 글자 묶음이 나뉘어요.
3. 글자 블록을 **드래그**해서 음의 높낮이를 정합니다.
4. 블록 양옆 핸들을 잡고 **늘이면** 길게 부르는 음이 돼요.
5. 마디가 부족하면 컨트롤 바의 **마디 + 버튼**을 눌러 늘리세요.
6. 다 그렸으면 **💾 저장**(JSON) 또는 **🔗 공유**(이미지/링크)로 내보내세요.

## 🛠 기술 스택

- **순수 HTML / CSS / Vanilla JS** — 빌드 단계 없이 정적 파일 하나로 동작합니다.
- **SVG** — 모든 악보 요소(블록·가이드 줄·곡선)는 인라인 SVG로 렌더링됩니다.
- **html2canvas** — PNG 내보내기에 사용 (CDN 로드).
- **폰트** : Pretendard GOV(본문) · Black Han Sans(한글 타이틀) · Gaegu/Fraunces/Zen Maru Gothic(캔버스 글자) · Material Symbols Rounded(아이콘).

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

## 🌐 접근성·키보드

- `Enter` : 입력 확정
- `Esc` : 입력 취소 / 선택 해제
- `Delete` / `Backspace` : 선택된 블록 삭제
- 한국어·일본어 IME 조합 중 `Enter`는 글자 확정에만 사용되며 블록 입력은 끊기지 않습니다.

## 🙏 만든 사람

[교육뮤지컬 꿈꾸는 치수쌤](https://litt.ly/chichiboo)

---

## English summary

**Easy Score** is a kid-friendly visual score editor. Lyrics become draggable
blocks whose vertical position represents pitch and whose horizontal length
represents note duration. Typing a sentence with spaces automatically splits
it into separate blocks, and the canvas grows by adding measures with the
± button.

- No music notation knowledge needed
- Pure HTML / CSS / Vanilla JS, no build step
- Single-file deploy (`index.html`)
- JSON save / shareable URL / PNG export
- Korean · English · Japanese UI
