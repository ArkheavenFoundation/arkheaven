# AKASHIC RECORD — 발명품 기록 보관소

GitHub Pages에서 돌아가는 SF 보고서풍 기록 사이트입니다.
기록은 이 저장소의 `data/records.json`에, 사진은 `data/images/`에 저장됩니다.

## 1. 저장소 만들기
1. GitHub에서 **New repository** → 이름 예: `akashic` → **Public** 선택 → Create
2. **Add file → Upload files** 로 이 폴더의 파일을 모두 올립니다.
   - `index.html`
   - `data/records.json`
   - `.nojekyll`
   - `README.md`
   (폴더째 끌어다 놓으면 `data/` 구조가 그대로 유지됩니다.)

## 2. 사이트 켜기 (GitHub Pages)
1. 저장소 **Settings → Pages**
2. Source: **Deploy from a branch** / Branch: **main**, 폴더 **/(root)** → Save
3. 1~2분 뒤 `https://<아이디>.github.io/<저장소이름>/` 에서 열립니다.

## 3. 쓰기 권한 토큰 만들기
1. GitHub 오른쪽 위 프로필 → **Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token**
2. Repository access: **Only select repositories** → 이 저장소만 선택
3. Permissions → Repository permissions → **Contents: Read and write**
4. 만들어진 `github_pat_...` 토큰을 복사합니다. (다시 볼 수 없으니 바로 사용)

## 4. 사이트에서 연결
1. 사이트 오른쪽 위 **⚙** 버튼
2. 아이디·저장소 이름은 자동으로 채워집니다. 토큰만 붙여넣고 **연결 확인 & 저장**
3. 상태가 `GITHUB SYNC` 로 바뀌면 끝. 이제 기록을 등재·수정·삭제하면 저장소에 바로 커밋됩니다.

## 알아둘 것
- 토큰은 **내 브라우저에만** 저장됩니다. 다른 기기에서 쓰려면 그 기기에서도 한 번 연결하세요.
- 토큰을 다른 사람에게 보여 주거나 저장소 파일에 적지 마세요. 유출되면 GitHub에서 바로 삭제(Revoke)하면 됩니다.
- 연결하지 않은 방문자는 읽기만 가능합니다.
- 저장 후 다른 사람 화면에 반영되기까지 1~2분 걸립니다 (GitHub Pages 배포 시간).
- ⚙ 메뉴의 **JSON 내보내기 / 가져오기** 로 백업하고 옮길 수 있습니다.
