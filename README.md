# DROM Lab 홈페이지 (drom.knu.ac.kr)

경북대학교 스마트생물산업기계공학과 **노외기계설계 및 신뢰성평가 연구실(DROM Lab)** 홈페이지.
정적 HTML/CSS로 제작되어 GitHub Pages로 그대로 배포됩니다. (버전 02 · 2026-07-23)

## 페이지 구성
| 파일 | 내용 |
|------|------|
| `index.html` | 메인 (한국어) — 사이트 첫 화면 |
| `ko_1_main.html` | 메인 (한국어) — index.html과 동일 사본 |
| `ko_2_professor.html` | 교수 소개 (한국어) |
| `ko_5_students.html` | 재학생 소개 (한국어) — 대학원생·학부연구생 |
| `ko_6_alumni.html` | 졸업생 소개 (한국어) |
| `ko_3_lab.html` | 연구실 소개 (한국어) |
| `ko_4_research.html` | 연구 분야 (한국어) |
| `en_1_main.html` | 메인 (English) |
| `en_2_professor.html` | Professor (English) |
| `en_5_students.html` | Students (English) |
| `en_6_alumni.html` | Alumni (English) |
| `en_3_lab.html` | About the Lab (English) |
| `en_4_research.html` | Research (English) |
| `images/` | 교수·학생·졸업생 사진 (professor.jpg, student_*.jpg, grad_*.jpg) |
| `drom_logo.svg` | 로고 |
| `CNAME` | 커스텀 도메인 설정 (drom.knu.ac.kr) |
| `404.html` | 없는 페이지 안내 |

## 메뉴 구조
메인 "둘러보기": **연구원 소개 / 연구실 소개 / 연구 분야**.
"연구원 소개"는 교수 소개 페이지로 연결되고, 교수/재학생/졸업생 페이지 상단의
서브 탭(교수 소개 · 재학생 · 졸업생)으로 서로 이동합니다.

## 배포 방법 (요약)
1. 이 폴더의 모든 파일·폴더(images 포함)를 GitHub 저장소에 업로드.
2. Settings → Pages → Source: `main` / `/(root)`.
3. Custom domain: `drom.knu.ac.kr` (CNAME 파일 포함됨). 학교 DNS에서 `<사용자명>.github.io` 로 연결 요청.
4. Enforce HTTPS 체크.

## 수정 방법
- 색상: 각 HTML 상단 `<style>` 안 `.dl-root{ --navy / --blue / --teal ... }` 변수.
- 학생 추가: `images/` 에 사진(예: `student_이름.jpg`)을 올리고, `ko_5_students.html`(및 `en_5_students.html`)
  의 `dl-mgrid` 안에 카드 한 덩어리(`<div class="dl-mcard">…</div>`)를 복사해 이름·이메일·사진 경로만 바꾸면 됩니다.
- 텍스트: 해당 HTML 본문을 직접 편집.

## 데이터 출처
학생·졸업생·교수 사진과 명단은 기존 KNU 홈페이지(home.knu.ac.kr/HOME/drom)에서 이전.
사진은 웹용으로 축소되어 `images/`에 포함되어 있습니다.
