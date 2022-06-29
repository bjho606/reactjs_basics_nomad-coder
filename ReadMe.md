# A free ReactJs lesson from nomadcoders.co

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

- JSX – 자바스크립트를 확장한 문법
    - 보통의 HTML과 비슷. 그러나 property를 HTML 태그의 속성처럼 적으면 됨

ex)
const Title = (
    console.log("mouse enter")}>
    Hello I'm a span
);

## STATE (04-)
- VanillaJs vs ReactJs : VanillaJs는 바뀌는 부분이 있으면 HTML 코드에서 관련된 태그 전부를 바꾸지만, ReactJs는 바뀌는 값만 바뀌고 나머지는 바뀌지 않는다.
