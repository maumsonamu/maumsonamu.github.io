# 마음소나무 심리연구상담소 홈페이지 — 수정 안내

홈페이지 주소: **https://maumsonamu.github.io** (저장소 이름에 따라 달라짐)

## 내용 수정하기

1. 이 저장소에서 **`_config.yml`** 클릭 → 오른쪽 위 **연필 아이콘**
2. 한글 텍스트 수정 (콜론 `:` 왼쪽 영문 이름과 들여쓰기는 그대로)
3. **Commit changes…** → **Commit changes**
4. 1~2분 뒤 홈페이지 새로고침

## 처음에 꼭 채워야 할 것 (`_config.yml`에서 "입력하세요" 검색)

| 항목 | 위치 |
|---|---|
| 전화번호, 통화 가능 시간 | `contact:` → `phone:`, `phone_hours:` |
| 이메일 | `contact:` → `email:` |
| 카카오톡 채널 주소 | `contact:` → `kakao_url:` (비우면 숨겨짐) |
| 네이버 예약 / 구글 폼 주소 | `contact:` → `form_url:` (비우면 숨겨짐) |
| 운영 시간, 상담 비용, 결제 방법 | `info:` 목록 |
| 상담사 자격 | `director:` → `credentials:` |

## 예약을 열 때

`_config.yml` 에서 `booking_open: false` → `booking_open: true` 로 바꾸고, `contact:` 의 전화·이메일·카카오톡·예약 양식 주소를 채우면 첫 화면 버튼과 "예약 · 문의" 섹션이 예약 모드로 바뀝니다.

## 하단 회사 정보

`company:` 에서 수정합니다 (상호, 대표, 사업자등록번호, 주소, 대표 전화·이메일, 안내 문구).

## 자주 하는 수정

| 하고 싶은 것 | 위치 |
|---|---|
| 휴무·공지 올리기 | `news:` 맨 위에 `- date:` / `text:` 추가 |
| 상담 영역 추가·수정 | `services:` (`title`, `desc`, `tags`) |
| 자주 묻는 질문 추가 | `faq:` 에 `- q:` / `a:` 덩어리 추가 |
| 비용·시간 변경 | `info:` 의 `value:` |
| 연구 소개 수정 | `research:` (`title`, `subtitle`, `desc`, `note`) |
| 첫 화면 문구 | `center:` → `tagline:`, `lead:` |
| 상담사 사진 | 저장소에 `images/` 폴더 만들어 사진 업로드 후 `director:` → `photo: images/파일명.jpg` |
| 긴급 연락처 | `emergency:` (바꾸지 않는 것을 권장) |

## 주의

- 값에 콜론(`:`)이 들어가면 따옴표로 감싸세요. 예: `value: "평일 10:00–18:00"`
- 수정 후 반영이 안 되면 저장소 **Actions** 탭에 빨간 X가 있는지 확인 (들여쓰기·따옴표 오류). 오류가 있어도 이전 버전이 계속 보입니다.
- 내담자 정보, 상담 기록은 절대 이 저장소에 올리지 마세요. 공개 저장소입니다.

## 파일 설명

| 파일 | 역할 |
|---|---|
| `_config.yml` | **홈페이지 내용** (여기만 고치면 됨) |
| `index.html` | 디자인 틀 |
| `robots.txt`, `sitemap.xml` | 검색엔진용 |
| `README.md` | 이 안내문 |
