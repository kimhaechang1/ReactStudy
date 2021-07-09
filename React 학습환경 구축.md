# React 환경을 만들어 보자

npm, node.js 설치
보통 nodejs 설치 하면 자동으로 npm도 설치 됨

2. 기본 파일 형성
프로젝트 폴더 생성(소문자 영어로 작성할 것)
명령프롬프트 실행 후 
cd 프로젝트 폴더경로
npm init -y : package.json 초기 파일 생성

프로젝트 폴더 안에 
index.html 생성 후
js폴더 및 jsx 폴더 생성
jsx폴더에 .jsx 파일만, js폴더에 .js 파일만...

```HTML
in index.html...
<!DOCTYPE html>
<html>
    <head>
        <script src = "node_modules/react/dist/react.js"></script>
        <script src = "node_modules/react-dom/dist/react-dom.js"></script>
    </head>
    <body>
        <div id = "content"></div>
        <script src = "js/JAVASCRIPT_FILE_NAME.js"></script>
    </body>
</html>
```

3. http-server 설치 (Apache로 대체 할 예정)
스스로 만든 웹 테스트용
명령 프롬프트 실행 후

```
npm install http-server
```

실행은 프로젝트 단위로 실행
명령프롬프트 실행 후
cd 프로젝트 폴더경로

```
http-server ./
```

4. React 설치

프로젝트단위로 설치 
명령프롬프트 실행 후
cd 프로젝트 폴더 경로

```
npm install react@15 react-dom@15
```
package.json 에 버전 확인

5. babel 설치
.jsx -> .js로 변환 
프로젝트 단위로 설치 

명령 프롬프트 실행 후
cd 프로젝트 폴더 경로
```
npm install @babel/cli
npm install @babel/core
npm install babel-preset-react@6.5.0
```
변환 실행 명령
명령 프롬프트 실행 후 
cd 프로젝트 폴더 경로
```
npx babel jsx/JSX_FILE_NAME.jsx -o js/JAVASCRIPT_FILE_NAME.js
```
```
주의 
package.json에서
"babel": {
    "presets": [ "@babel/preset-react" ]
  },
이 부분 꼭 넣어줘야 npx babel 실행됨 (이미 되어 있다면 무시)
```
