# 건축사 작도 대시보드

2027년 3월 5일 건축사 시험까지의 작도 체크리스트입니다.

- 체크리스트에서 끝낸 작도를 누르면, 공부 기록(날짜별 칸)과 월별·전체 완성도 그래프가 바로 바뀝니다.
- 체크 기록은 이 저장소의 `progress.json`에 저장되어 휴대폰과 PC에서 똑같이 보입니다.
- 일정을 바꾸려면 `schedule.json`을 고치면 됩니다.

## 처음 한 번 설정

### 1. GitHub Pages 켜기
저장소 → Settings → Pages → Branch를 `main`, 폴더를 `/ (root)`로 두고 Save.
1~2분 뒤 `https://<아이디>.github.io/<저장소이름>/` 에서 열립니다.

### 2. 동기화용 토큰 만들기
1. GitHub → 오른쪽 위 프로필 → Settings → Developer settings → Personal access tokens → **Fine-grained tokens** → Generate new token
2. Expiration: 시험 이후 날짜로 지정 (예: 2027-03-31)
3. Repository access: **Only select repositories** → 이 저장소만 선택
4. Permissions → Repository permissions → **Contents: Read and write**
5. Generate 후 나온 `github_pat_…` 값을 복사

### 3. 페이지에 토큰 넣기
대시보드 오른쪽 위 버튼(「동기화 꺼짐 · 설정」)을 눌러 토큰을 붙여넣고 저장합니다.
폰과 PC에서 각각 한 번씩 넣으면 됩니다. 토큰은 그 기기의 브라우저에만 저장됩니다.

## 파일

| 파일 | 내용 |
| --- | --- |
| `index.html` | 대시보드 페이지 |
| `schedule.json` | 작도 일정 (날짜, 회차, 교시, 월) |
| `progress.json` | 체크 기록. 페이지가 자동으로 고칩니다 |
