# React-Router tutorial

🔨 가장 대표적인 리액트 라우팅 라이브러리인 React-Router를
사용


### *프로젝트 적용방법*

#### 1. 라이브러리 설치

```
npm add react-router-dom 
```

#### 2. 라우터 적용

src/index.js 파일에서 react-router-dom에 내장되어있는 BrowserRouter라는 컴포넌트를 사용해 감싸기

```
import React from 'react';
import ReactDOM from 'react-dom';
import {BrowserRouter} from 'react-router-dom';

ReactDOM.render(
  <BrowserRouter>
    <App />
  </BrowserRouter>,
  document.getElementById('root')
);
```

#### 3. Route 컴포넌트로 특정 주소에 컴포넌트 연결

```
import { Routes, Route } from "react-router-dom"
import About from './about';
import Home from './home';

const App = () => {
  return (
    <Routes>
      <Route path="/" element={<Home/>} />
      <Route path="/about" element={<About/>} />
    </Routes>
  );
}

export default App;
```


