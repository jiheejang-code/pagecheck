# PageCheck GitHub Pages 배포 안내

## 1. 온라인 화면 게시
1. GitHub에 로그인하고 새 저장소를 만듭니다. 이름은 pagecheck, 공개 범위는 Public으로 선택합니다.
2. 이 ZIP을 압축 해제합니다. 저장소의 Add file → Upload files에서 이 폴더의 **내용물**을 올립니다. index.html이 저장소 최상위에 있어야 합니다.
3. Commit changes로 저장합니다.
4. Settings → Pages → Build and deployment에서 Source를 Deploy from a branch로 선택합니다.
5. Branch는 main, 폴더는 /(root)로 선택하고 Save를 누릅니다.
6. 배포가 끝나면 Pages 설정에 나타나는 Visit site 주소를 엽니다. 보통 https://사용자이름.github.io/pagecheck/ 형태입니다.

## 2. 이 PC에서 실제 검사 연결
1. 온라인 화면의 로컬 엔진 다운로드로 받은 pagecheck-local.zip을 압축 해제합니다.
2. 설치.bat를 처음 한 번 실행합니다. Node.js 20 이상과 Chrome 또는 Edge가 필요합니다.
3. 온라인연결.bat를 실행하고 1단계의 Visit site 주소를 붙여넣습니다. 기존 엔진 실행 창이 있다면 먼저 종료하세요.
4. 온라인 화면의 엔진 연결에서 http://127.0.0.1:47831 과 실행 창에 표시된 연결 키를 입력합니다.
5. 브라우저가 로컬 네트워크 접근 허용을 요청하면 허용합니다. 연결이 제한되는 환경에서는 http://127.0.0.1:47831 로 검수할 수 있습니다.
6. 회사의 테스트 URL을 등록하고 빠른 점검부터 실행합니다. 실행 창을 닫으면 검사 엔진도 종료됩니다.

온라인연결.bat는 입력한 github.io 출처만 해당 실행 중 허용합니다. GitHub 프로젝트 경로는 서로 같지 않아도 동일 출처를 공유하므로 신뢰할 수 있는 계정에 게시하세요. 연결 키는 공개 저장소에 올리지 않습니다.

## 공개되는 범위
이 폴더의 화면 코드, 자체 예시 결과·이미지, 로컬 실행 패키지가 공개됩니다. 회사 URL·검수 기록·로그인 세션은 포함하지 않습니다. 실제 기록과 증거 화면은 로컬 엔진의 data 폴더에 보관됩니다. 결과를 내보낸 파일은 따로 공개 저장소에 올리지 마세요.

GitHub Pages는 정적 화면을 게시합니다. 실제 브라우저 검사 서버는 PC에서 실행합니다. 팀 공동 기록 저장과 회사 로그인 기능은 별도 구축 범위입니다.

## 공식 도움말
- https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
