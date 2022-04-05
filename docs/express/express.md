# Express 

Express는 Node.js 웹 프레임워크입니다. 


## Node.js와 NPM 설치

https://nodejs.org


## 버전 확인

* node -v
* npm -v

## Express Application Generator

https://expressjs.com/en/starter/generator.html

* npx express generator

## Hello World

```Terminal
md express
cd express
express - h 
express --git --hbs expressapp 
cd expressapp
npm install 
DEBUG=expressapp:* npm start 
start http://localhost:3000 
```

## public 폴더

정적 파일들이 들어오는 곳


## routes 폴더

라우팅 설정

## views 폴더

핸들바를 사용하는 뷰 페이지 영역



## ExpressNote

```Terminal
npm init
(엔터)
(엔터)
(엔터)
(엔터)
(엔터)
(엔터)
author: RedPlus

cd express-note
code . 
npm install express nodemon 
npm install --save-dev @babel/core @babel/cli @babel/preset-env @babel/node 
touch .babelrc 
```

## .babelrc 파일

```Text
{
  'presets': [
    "@babel/preset-env"
  ]
}
```

## package.json 

package.json
```JSON
{
  ...
  "type": "module", 
  ...
  "scripts": {
    "start": "nodemon --experimental-json-modules --exec babel-node index.js"
  }
}
```


