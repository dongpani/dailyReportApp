# dailyReportApp
vue.js 데일리 레포트 만들기

## CLI 도구 설치
1. 윈도우 cmder 설치 <br>
2. <a>https://cmder.net/</a> 접속 후 pull 버전 패키지 다운로드
3. 압축을 해제하고 원하는 경로로 이동 (C:\devTools\cmder\)
4. 윈도우 cmd 관리자 권한으로 실행
5. .\cmder.exe /REGISTER ALL
6. 아무 폴더에서 context 메뉴에서 활성 체크

## CLI 로 설치
1. 터미널 실행 후 명령어 입력(cmder)
2. npm install -g @vue/cli
3. vue --version 
4. 버전 확인

## vue 프로젝트 생성
1. 프로젝트 폴더로 이동.
2. vue create 프로젝트명
3. menual 선택
4. babel, router, vuex, css pre-processors, linter/formatter 선택 후 엔터 (5개)
5. Y
6. Sass 선택
7. EsLint with error preventioin only 선택
8. Lint on save  선택
9. In dedicated config files : 지금까지의 설정을 별도의 파일에 저장
10. 그냥 엔터

## 로컬 서버 실행
1. 로컬 서버 실행 : npm run serve
2. 브라우저 자동 실행 : package.json : vue-cli-service serve --open
