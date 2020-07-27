# inflearn-React-with-Typescript
:point_right: **인프런 강좌를 통해 리액트(React), 타입스크립트(Typescript) 배우기**
------------
[인프런 - 타입스크립트코리아 : React with TypeScript 세미나](https://www.inflearn.com/course/react-with-typescript/dashboard)
> 본 Repository는 인프런에서 제공하고 있는 무료 강좌를 통해 학습한 내용을 정리하고 있음을 밝힙니다.

### 1. React란? 
- React의 기본 작업단위는 Component다.
    - Component Tree는 DOM Tree와 동일 하다고 볼 수 있다.
    - [왜 Virtual DOM 인가?](https://velopert.com/3236)
    - [React and the Virtual DOM](https://www.youtube.com/watch?v=BYbgopx44vo)
- JSX(JavaScript XML) 문법을 사용한다.
    - JSX.Element로 그려질 Component를 표현
    - React.Component를 상속받아서 render를 호출하면 react가 그려줌!
- React Basic Project: es6
    - webpack2, webpack-dev-server
    - loader
        - babel-loader
            - babel-core, babel-preset-env, bael-plugin-transform-react-jsx
    - react, react-dom
- React Basic Project: TypeScript
    - webpack2, webpack-dev-server
    - loader
        - ts-loader / typescript
        - tslint-loader
            - tslint, tslint-react
        - source-map-loader
    -react
        - react, @types/react, react-dom, @types/react-dom
    - :heavy_exclamation_mark: ts-loader는 typescript를 컴파일해야 하는데 이를 위해서는 typescript를 설치해야함
    - :heavy_exclamation_mark: tslint-loader - eslint와 같은 역할
- Create-React-App(CLI)
    - 부가적인 설정을 알아서 해주는 기특한 녀석
    - 개발용 / 프로덕션 빌드 / 테스트 / eject / progressive webapp
    - ~~너는 Component나 잘 짜라.~~
    - eject는 돌이킬수 없는것...
```
create-react-app [프로젝트명] --typescript
```
- webpack의 진입로는 index.tsx
- src directory에서 작업을 시작하자!

#### 1.1 src 디렉토리 요소들의 역할
- index.tsx
    - 메인 엔트리 파일이자, 가장 위에서 ReactDom.render를 수행
    - pwa를 위한 서비스 워커 등록
- index.css
    - 글로벌 스타일 작성
- App.tsx
    - App 컴포넌트, 클래스 이름과 파일이름을 맞추는 것이 관례다!
- App.css
    - App 컴포넌트에서 쓰이는 스타일
- App.test.tsx
    - App 컴포넌트에 대한 테스트 작성 파일
- serviceWorkder.ts
    - pwa를 위한 것


