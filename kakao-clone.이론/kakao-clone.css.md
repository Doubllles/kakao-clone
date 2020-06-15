css  syntax

css는 2가지 파트가 있다

	1. selector : ex) h1{ 작성한 property를 넣는다 }
 	2. Property :  property-name:value(무조건 소문자,공백없이사용,마지막 세미콜론)



css를 html에 연결시키는 방법

​	1.inline방법: head안에 <style></style>을 사용해서 적어넣음,모든 html에 복사해야하는 단점이있음

​	2.external방법:<link href = "style.css" ref= "stylesheet"> 링크만 붙여넣으면됨



박스모델

element들이 박스이다.



패딩:안쪽으로 패딩값이생긴다(간격을 만들어낸다), 총길이 늘어남, 보더에서 안쪽으로의 간격

마진: 보더에서 바깥쪽으로의 간격,

보더:border-width 값만큼 늘어난다.



display:block은 폭,높이가 존재하지만 그 옆에 어떤. element도 놓을 수 없다.



display:inline은 박스의 모든 property 설정값을 지운다.

Ex) span에서 내가 작성한 컨텐츠의 폭,높이 만큼의 스타일만 적용됨

인라인이라 함은 텍스트다,텍스트는 높이도 폭도 없다. 켄텐츠의 길이만 존재할뿐 이다



display:inline-block 은 박스의 폭, 높이가 존재하고 그리고 서로서로 옆에 놓을 수 있다.

인라인과 같은 설정값을 원하면서 동시에 박스 형태를 유지하고 싶을때 사용



포지션

 style{ //브라우저가 갖고있는 디폴트 값을 상쇄시키기 위함

​	height:100%,

​	Margin:0,

​	padding:0;

}



플렉스

Inline-block을 사용하게 되면 자동으로 옆으로 붙는게 아니라, 브라우저의 칸에 꽉차게되면 아래로 떨어진다.

부모 컨테이너를 플렉스로 선언하면, 그 안에 종속된 칠드런 박스들을 움직일 수 있다. 

​	그렇기 때문에, 각각 박스에게 일일히 명령할 필요가 없다.

```
  html, body {
​            height: 100%;
​        }


​        .*father* {
​            display: flex;
​            justify-content: center;
​            align-items: center;
​            height: 100%;
						flex-direction:column; //주축을 가로에서 세로로 바꾸게된다. 이때 align-items은 가로가된다.
​        }
```



'입력을 누르는 버튼' 을 선택하고 싶다고하면, class를 주 수도 있다.

Id,class를 사용하지 않고 pseudo-selector(가상 셀렉터:element가 아닌 것을 뜻함)를 사용할 수도 있음.



트랜지션:*transition, 하나의 state에서 다른 tate로 넘어갈 때 나타나는 효과*

트랜지션은 어떤 state가 바뀔때 적용이된다.

state들은 hover, active, focus,visited가 있다.

트랜지션은 hover, active, focus 에서 효과적으로 적용이됨. 



트랜스포메이션:element의 모양새를 바꾸는 것





