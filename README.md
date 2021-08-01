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

    >element의 내부를 보고 싶으면 console.dir()
    >addEvenetListener 구문
    > > ```
    > > target.addEventListener(type, listsner);
    > > 예제)
    > > function handleResize(){
    > >   console.log("I have been resized")
    > > }
    > > window.addEvenetListener("resize", handleResize);

    > > console title = document.querySelector("div.hello:first-child h1");
    > > function handleTitleClick(){
    > > title.style.color="blue";
    > > }
    > > title.addEventListener("click",handleTitleClick);
    > > //title.onclick = handleTitleClick;이런식의 표현도 가능하다.
    > > function handleWindowResize(){
    > > document.body.style.backgroundColor = "tomato";
    > > }
    > > window.addEventListener("resize", handleWindowResize);
    > > ```
    > > handleResize를 할 때, 뒤에 ()를 붙이지 않는다. ()를 붙이면 함수가 바로 호출되어 버린다.

- If else -Function practice
    > 비교를 할 때는 ===을 쓴다.
    > 
    > rgb 형식 사용시에 반점 뒤에는 반드시 띄어쓰기 한칸을 해야 한다. ex)rgb(52, 73, 94)
    > 
    > 그리고 JS에서는 rgb형식을 쓰자! (OTHER COLOR 같이 저렇게 쓰면 비교 구문에서동작이 안된다.)
    > 이벤트의 종류가 궁금하다면, MDN을 방문하자! 꼭!(formerly Mozilla Developer Network)

    > const와 let의 차이: let은 변할 수 있는 값.
    > ```
    > const currentColor = title.style.color
    > const OTHER_COLOR = "#7f9c8d"
    > if(currentColor === BASE_COLOR){
    >   tytle.style.color = OTHER_COLOR;
    > }else{
    >   title.style.color = BASE_COLOR;
    >  }
    >  
    > ```
- CSS in Javascript(3.8)
    > toggle 함수: html의 className을 변경하는 버그를 막기 위해, classList에 token(className)의 여부로 추가/삭제를 해주는 함수.
    > ```
    > const h1 = document.querySelector("div.hello:first-child h1");
    > function handleTitleClick(){
    > h1.classList.toggle("clicked");
    > }
    > h1.addEvenetListener("click", handleTitleClick);
    > ```
