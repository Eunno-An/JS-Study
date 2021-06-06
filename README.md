# JS-Study

### _노마드 코더 바닐라 JS로 크롬 앱 만들기_


## Practicing 
- [replit 실습](https://replit.com/@EunnoAn/BothGoodnaturedCache#index.html)
- JS 기본 함수 정의
- 오브젝트 안에서의 함수 선언 방법, 리턴
- JS로 DOM 변경하기
    > document.querySelector():querySelector는 특정 name이나 id를 제한하지 않고 css 선택자를 이용해 찾을 수 있다. 
    > 
    > 객체를 id로 찾고 싶다면 "#title"
    > 
    > 클래스로 찾고 싶다면 ".title"
    > 
    > getElementById(): gets only by ID
    > 
    > getElementByClassName(): gets MANY elements by classname
    > 
    > querySelector(): gets ONE element by any selector you want.
    > 
- 이벤트와 이벤트 핸들러
    >JS는 html과 css를 바꾸는 기능을 하지만, 이벤트에 반응하기 위해 만들어짐.
    >
    >event란? 웹사이트에서 발생하는 것들: click, submit, input, change, load, before, closing, printing..
    >
    >addEvenetListener 구문
    > > ```
    > > target.addEventListener(type, listsner);
    > > 예제)
    > > function handleResize(){
    > >   console.log("I have been resized")
    > > }
    > > window.addEvenetListener("resize", handleResize);
    > > ```
    > > handleResize를 할 때, 뒤에 ()를 붙이지 않는다. ()를 붙이면 함수가 바로 호출되어 버린다.

- If else -Function practice
    > 비교를 할 때는 ===을 쓴다.
    > 
    > rgb 형식 사용시에 반점 뒤에는 반드시 띄어쓰기 한칸을 해야 한다. ex)rgb(52, 73, 94)
    > 
    > 그리고 JS에서는 rgb형식을 쓰자! (OTHER COLOR 같이 저렇게 쓰면 비교 구문에서동작이 안된다.)
    > 이벤트의 종류가 궁금하다면, MDN을 방문하자! 꼭!(formerly Mozilla Developer Network)
    >
    > ```
    > const currentColor = title.style.color
    > const OTHER_COLOR = "#7f9c8d"
    > if(currentColor === BASE_COLOR){
    >   tytle.style.color = OTHER_COLOR;
    > }else{
    >   title.style.color = BASE_COLOR;
    >  }
    > ```
