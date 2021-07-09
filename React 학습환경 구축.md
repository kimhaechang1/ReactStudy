# React 환경을 만들어 보자

## npm, node.js 설치
보통 nodejs 설치 하면 자동으로 npm도 설치 됨

## 기본 파일 형성
프로젝트 폴더 생성(소문자 영어로 작성할 것)

명령프롬프트 실행

cd 명령어로 프로젝트 폴더 경로로 이동한 후
```
npm init -y : package.json 초기 파일 생성
```

프로젝트 폴더 안에 

index.html 생성
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
js폴더 및 jsx 폴더 생성

jsx폴더에 .jsx 파일만, js폴더에 .js 파일만...


## http-server 설치 (Apache로 대체 할 예정)
스스로 만든 웹 테스트 목적


명령프롬프트 실행

cd 명령어로 프로젝트 폴더 경로로 이동한 후
```
npm install http-server
```

http-server 실행은 프로젝트 단위로 실행


명령프롬프트 실행

cd 명령어로 프로젝트 폴더 경로로 이동한 후
```
http-server ./
```

## React 설치
프로젝트단위로 설치 


명령프롬프트 실행

cd 명령어로 프로젝트 폴더 경로로 이동한 후
```
npm install react@15 react-dom@15
```
package.json 에 버전 확인

## babel 설치
.jsx -> .js로 변환목적
프로젝트 단위로 설치 


명령프롬프트 실행

cd 명령어로 프로젝트 폴더 경로로 이동한 후
```
npm install @babel/cli
npm install @babel/core
npm install babel-preset-react@6.5.0
```

babel 실행 명령


명령프롬프트 실행

cd 명령어로 프로젝트 폴더 경로로 이동한 후
```
npx babel jsx/JSX_FILE_NAME.jsx -o js/JAVASCRIPT_FILE_NAME.js
```

**주의**
```
package.json에서
"babel": {
    "presets": [ "@babel/preset-react" ]
  },
  ```
**이 부분 꼭 넣어줘야 npx babel 실행됨 (이미 되어 있다면 무시)**

