# Express Fundamentals 

Express는 Node.js 웹 프레임워크입니다. 

## Node.js

* 서버 쪽 자바스크립트
* 크로스 플랫폼
* 자바스크립트/타입스크립트 그 자체
* 오픈소스 

## Node.js와 NPM 설치

* https://nodejs.org
  * LTS 버전 설치(강의 기준) 

## 버전 확인

* node -v
  * node --version
* npm -v
  * npm --version 


> * nvm - Node Version Manager
> * nvm-windows 
> * nvm install node 


## IDE: Visual Studio Code

* https://code.visualstudio.com 

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

* npm init
* npm install express

```Terminal
npm init
p(엔터)
v(엔터)
d(엔터)
t(엔터)
g(엔터)
k(엔터)
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


## /index.js

```JS
import express from "express";

const app = express(); 

const PORT = 3000;

app.lesten(PORT, () => {
  console.log(`Server start on port ${PORT}`);
})
```

```Terminal
npm start
```

## /app.js

```JS
const express = require('express');

const app = express(); 

app.get('/', (req, res) => {
   res.send("Hello Express.js");  
});

app.listen(3000, () => {
    console.log("listening 3000 port"); 
});
```

```Terminal
node app.js 

start http://localhost:3000 
```



