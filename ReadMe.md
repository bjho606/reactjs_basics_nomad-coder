# A free ReactJs lesson from nomadcoders.co
[Nomad Coders Lesson](https://nomadcoders.co/react-for-beginners)

## The Basics of React (01~03)
- React JS - 어플리케이션이 아주 인터랙티브하도록 만들어주는 library. 엔진과 같다.
- React-dom - library 또는 package. 모든 react element들을 HTML body에 둘 수 있도록 해줌.

<br>

- ReactDOM.render() - render의 의미는 react element를 가지고 HTML로 만들어 배치한다는 것. 즉, 사용자에게 보여준다는 의미
    - ReactDOM.render(A, B) = A 를 B 아래에 배치한다.

- React.createElement("span", {span의 property}, “span의 내용”)
    - property는 class name, id도 가능 style도 가능
    - (참고만 하고 외우지 말기. 이렇게 쓸 일 없음)

<br>

- 바닐라JS는 HTML -> JS 순서
- 리액트는 JS -> HTML 순서

    JS가 element를 생성하고 React JS가 그것을 HTML로 번역하는 것<br>
    React JS는 업데이트 해야 하는 HTML을 업데이트 할 수 있음

<br>

- JSX (JavaScript XML) – javascript에 xml을 추가한 확장한 문법
    - 보통의 HTML과 비슷. 그러나 property를 HTML 태그의 속성처럼 적으면 됨
    - React 프로젝트에서 사용됨
    - Babel은 JSX 문법을 브라우저에서 실행하기 전, javascript 형태의 코드로 변환해준다.

ex)
const Title = (
    console.log("mouse enter")}>
    Hello I'm a span
);

<br>

---
## STATE (04-07)
- VanillaJs vs ReactJs : VanillaJs는 바뀌는 부분이 있으면 HTML 코드에서 관련된 태그 전부를 바꾸지만, ReactJs는 바뀌는 값만 바뀌고 나머지는 바뀌지 않는다.
- state : ReactJs에서 값을 다룰 때 사용. 값을 변화시키고 자동으로 UI까지 rerender시켜준다. 이때 변하는 것은 전체 페이지가 아닌 해당 state값만!
    - [A, B] = React.useState(C)
        - A : 값
        - B : 값을 변경하거나 다루는 함수
        - C : 초기값

<br>

---
## Props (= Properties) (08-10)
- 부모 컴포넌트 -> 자식 컴포넌트로 데이터를 보낼 수 있게 해주는 방법
- 부모 컴포넌트에서 자식 컴포넌트를 호출할 때, property에 any_name으로 호출을 하면, 자식에서 'props'라는 Object 인자로 받아서 처리하게 됨. props에 들어가는 내용은 어떤 것이든(변수, 함수 등) 가능

### Prop Types
- 어떤 타입의 prop을 받고 있는지 체크해줌 -> 특정 타입만 받도록 설정해줄 수 있다.

    `<script src="https://unpkg.com/react@17.0.2/umd/react.development.js"></script>`

    `<script src="https://unpkg.com/prop-types@15.7.2/prop-types.js"></script>`
- Typescript와 같이 입력값의 타입을 미리 설정할 수 있다면 굳이 필요하지 않다.


### Memo
- 일반적으로 어떤 컴포넌트에서 state가 변하면, React에서는 해당 컴포넌트와 그 안에 포함된 모든 컴포넌트들을 re-render한다.
- 이때, "React Memo"를 통해 re-render가 필요하지 않은 컴포넌트들을 다시 그리지 않게 설정할 수 있다.
- 이 작업을 하지 않으면, 모든 컴포넌트를 다 rerender 하게 되므로, 속도가 느려질 수 있다!

<br>

---
---
## Create React App
- Useful when making a react application
- Helps with build setup and many other features

### Pre-Settings
1. install node
2. install npx

[Create React App](https://create-react-app.dev/)

[Create React App Github](https://github.com/facebook/create-react-app)

<br>
TO BE CONTINUED on the next repository...

[Go to next github session](https://github.com/bjho606/reactjs_create-react-app_nomad-coder)
