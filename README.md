# DROM Lab 홈페이지 (drom.knu.ac.kr)

경북대학교 스마트생물산업기계공학과 **노외기계설계 및 신뢰성평가 연구실(DROM Lab)** 홈페이지.
정적 HTML/CSS로 제작되어 GitHub Pages로 그대로 배포됩니다.

## 페이지 구성
| 파일 | 내용 |
|------|------|
| `index.html` | 메인 (한국어) — 사이트 첫 화면 |
| `ko_1_main.html` | `index.html`로 이동시키는 리디렉션 |
| `ko_2_professor.html` | 교수 소개 (한국어) |
| `ko_3_lab.html` | 연구실 소개 (한국어) |
| `ko_4_research.html` | 연구 분야 (한국어) |
| `en_1_main.html` | 메인 (English) |
| `en_2_professor.html` | Professor (English) |
| `en_3_lab.html` | About the Lab (English) |
| `en_4_research.html` | Research (English) |
| `drom_logo.svg` | 로고 |
| `CNAME` | 커스텀 도메인 설정 (drom.knu.ac.kr) |
| `404.html` | 없는 페이지 안내 |

## 배포 방법 (요약)
1. 이 폴더의 모든 파일을 GitHub 저장소에 업로드.
2. 저장소 **Settings → Pages** 에서 Source를 `main` 브랜치 / `/ (root)` 로 지정.
3. **Custom domain** 에 `drom.knu.ac.kr` 입력 (`CNAME` 파일이 이미 포함됨).
4. 학교 전산 담당에게 DNS에서 `drom.knu.ac.kr` 을 `<GitHub사용자명>.github.io` 로 연결(CNAME 레코드) 요청.
5. 연결 후 GitHub Pages의 **Enforce HTTPS** 체크.

## 수정 방법
- 색상: 각 HTML 상단 `<style>` 안의 `.dl-root{ --navy / --blue / --teal ... }` 변수 수정.
- 교수 사진: `ko_2_professor.html` / `en_2_professor.html` 의 `.dl-photo` div 내부를
  `<img src="사진파일.jpg" style="width:100%;height:100%;object-fit:cover">` 로 교체하고 사진 파일을 함께 업로드.
- 텍스트: 해당 HTML의 본문을 직접 편집.
