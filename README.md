# gonglab website

Static single-file site (`index.html`), hosted on GitHub Pages.

## 배포 (GitHub Pages)

1. GitHub에서 새 저장소 생성 (예: `gonglab-site`, Public)
2. 이 폴더의 파일 전체 업로드 (`index.html`, `.nojekyll`, `README.md`)
3. Settings → Pages → Source: **Deploy from a branch** → Branch: `main` / `/ (root)` → Save
4. 1~2분 후 `https://<아이디>.github.io/gonglab-site/` 에서 확인

## 내 도메인 연결

1. Settings → Pages → **Custom domain** 에 도메인 입력 (예: `gonglab.com`) → Save
   - 저장소에 `CNAME` 파일이 자동 생성됩니다.
2. 도메인 구매처 DNS 설정:
   - 루트 도메인(`gonglab.com`) — **A 레코드** 4개
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
   - `www` — **CNAME** → `<아이디>.github.io`
3. DNS 반영 후(수 분~수 시간) Pages 설정에서 **Enforce HTTPS** 체크

## 수정

디자인을 수정한 뒤 새로 생성된 `index.html`로 교체하여 커밋하면 자동 재배포됩니다.
