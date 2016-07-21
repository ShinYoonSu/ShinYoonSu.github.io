# folder/ file 세팅
1. 영문(한글이나 기타 다른언어로 작성시 웹에서 작동이 안될수 있음!!)
1. 첫글자를 숫자로 사용하는 것 x 무조건 영문
1. 첫글자 소문자로 사용
1. 폴더 및 파일 띄어쓰기 X ( _  - )   ex: work_file.jpg
1. 특수문자 사용 X (_사용만 권장)
1. 추후 사용할 html코드에서도 같은방법으로 사용됨

- **쿠팡기준 이름값 사용시** → 폴더, 파일, 문서내에서의 이름 :단어/ 형용사로 표기 할 것을 권장.
## web 기본 구조(*.html 로 저장, 최초의 인식은 index.html)
```html
<<<<<<< HEAD
<!DOCTYPE html>  												  // html5 형식의 웹표준 선언
	<html lang="ko-KR">  										  // html시작, 한국어의 주사용
	<head>  													  // head 영역
		<meta http-equiv="X-UA-Compatible" content="IE=edge" />   // 설치된 컴퓨터에서의 IE최신버전 사용
		<meta charset="UTF-8">  								  // 사용언어 공용어
		<title>title</title>  									  // 웹페이지의 탭메뉴 표기 제목/웹 페이지 제목
		<style> 												  // css영역(추후 외부 문서로 링크)
			/*  */    											  // css에서의 주석
		</style>  												  // css닫기
	</head>  													  // head영역 닫기
	<body>  													  // html 본문(웹페이지에 나타나는 형태)
	
		<!--  -->   											  // html문서의 주석(css/js에서 사용할 수 없음
		<script>												  // javascript 내용작성(head에서도 사용가능)
			//													  // javascript문서에서의 한줄 주석
			/*  */												  // javascript문서 에서의 여러줄 주석
		</script> 											 	 // javascript 닫기
	</body>  													  // body닫기
	</html>													 	 // html 문서 종료  
=======
<!DOCTYPE html>  												// html5 형식의 웹표준 선언
	<html lang="ko-KR">  										// html시작, 한국어의 주사용
	<head>  														//head 영역
		<meta http-equiv="X-UA-Compatible" content="IE=edge" />  //설치된 컴퓨터에서의 IE최신버전 사용
		<meta charset="UTF-8">  								// 사용언어 공용어
		<title>title</title>  									// 웹페이지의 탭메뉴 표기 제목/웹 페이지 제목
		<style> 													// css영역(추후 외부 문서로 링크)
			/*  */    											// css에서의 주석
		</style>  												// css닫기
	</head>  														//head영역 닫기
	<body>  													//html 본문(웹페이지에 나타나는 형태)
	
		<!--  -->   											// html문서의 주석(css/js에서 사용할 수 없음
		<script>												// javascript 내용작성(head에서도 사용가능)
			//													// javascript문서에서의 한줄 주석
			/*  */												// javascript문서 에서의 여러줄 주석
		</script> 												// javascript 닫기
	</body>  													// body닫기
	</html>														//html 문서 종료  
>>>>>>> cebee98... 코드 일부 수정(보기편하게 변경)
```
___
## body 영역 기본 
1. [제목](#title)
2. [내용 및 강조](#paragraph)
3. [리스트](#list)
4. [링크 및 이미지](#link)
5. [영역 및 이름부여](#scope)
6. [table](#table)
7. [form](#form)
8. [기타](#etc)



### <a name="title">1. 제목</a>
> 제목이란 웹페이지의 필요 항목들에게 정확한 목적을 부여하기 위해 만들어 지는것을 의미하여 h1~h6까지 존재함

- **h1** 가장 중요한 제목의 의미로 사용되며, 웹페이지내에서 하나만 사용할 수 있으며(`html5`에서 다른의미로 가능) 반드시 들어가야하는 상황(주로 ***로고** 에 사용됨)  
- **h2** 두번째로 중요한 제목의 의미 카데고리 분류시 대제목 정도의 의미  
- **h3** 세번째로 중요한 제목의 의미  
- **h4** 네번째로 중요한 제목의 의미  
- **h5** 다섯번째로 중요한 제목의 의미  
- **h6** 여섯번째로 중요한 의미이자 가장 작은 단위의 제목으로 분류  

### <a name="#paragraph">2. 내용 및 강조</a>
> `내용`이란 웹페이지 내에서의 내용을 작성하는 곳으로 쉽게 말해, 본문 or 단락을 의미, 내용상 단락이나 문장을 작성시에 사용  

- **p**  단락의 의미로 사용되고 있으며, 여러번의 띄어쓰기 또는 줄바꿈이 이루어지지 않는 형태의 코드
- **pre** `<p>`와 같은 의미로 사용되나, 여러번의 띄어쓰기, 줄바꿈이 쉽게 이루진다는 장점이 있으나 실무에 사용하기 다소 불편한점이 많아, 자료 확인용이거나 특수한 경우에만 사용되기도 함.
- **br** `<p>` 사용시 줄바꿈을 사용할 경우에 중간에 기입하여 강제 줄바꿈(개행 이라고도 한다)처리 → 어떠한 코드를 삽입하여도 줄바꿈 처리 가능

> `강조`란 웹페이의 문서내용중 일부를 강조의 의미로 사용시 작성되는 곳  

- **strong** 과거 `<b>`로 사용하기 도 했었으나, 정확한 강조의 의미로 사용하기 위한 목적으로 사용(굵은 글씨로 처리)
- **em** 과거 `<i>`로 사용하기 도 했었으나, 정확한 강조의 의미로 사용하기 위한 목적으로 사용(기울기로 처리)
- **del** 과거 `<s>, <strike>`로 사용하기 도 했었으나, 정확한 강조의 의미로 사용하기 위한 목적으로 사용(취소선 처리)
- **ins** 과거 `<u>`로 사용하기 도 했었으나, 정확한 강조의 의미로 사용하기 위한 목적으로 사용(밑줄로 처리)

> `인용문`이란 내용상의 글이 다른이의 말을 인용시에 처리 ex(\"너 자신을 알라\"-소크라테스)의  표현처리시 사용

- **q** 둘러싼 텍스트가 짧은 인라인 인용문, 이 요소는 단락 구분이 필요없는 짧은 인용문을 위해 사용

```html
<p>Everytime Kenny is killed, Stan will announce 
   <q cite="http://en.wikipedia.org/wiki/Kenny_McCormick#Cultural_impact">
     Oh my God, you/they killed Kenny!
   </q>
</p>
```
- **blockquote** 긴 인용문 요소를 사용
	+ **cite** 이 속성의 값은 인용된 정보의 원본 문서나 메세지를 가리키는 URL를 나타냅니다.

```html  
<blockquote cite="http://developer.mozilla.org">
  <p>This is a quotation taken from the Mozilla Developer Center.</p>
</blockquote>
```
- **abbr** 약어를 나타내며 선택적으로 약어에 대한 전체 설명을 제공, 만약 title 속성이 존재한다면 전체 설명만을 포함

```html  
<p>I do <abbr title="Hypertext Markup Language">HTML</abbr></p>
```

### <a name="list">3. 리스트</a>
> `리스트`란 여러개의 나열된 형태 즉, 리스트 항목을 나타낼 때 사용

1. **ul** 정렬되지 않은 리스트  
	- 자식태그로는 반드시 `<li>`를 사용해야함  
2. **ol** 정렬된 리스트
	- 자식태그로는 반드시 `<li>`를 사용해야함  
3. **dl** 제목과 내용을 담는 리스트<br>
	- 자식태그로는 반드시 제목태그로 `<dt>`를 사용해야함
	- 자식태그로는 반드시 내용태그로 `<dd>`를 사용해야함  

### <a name="link">4. 링크 및 이미지</a>
> 절대경로/ 상대경로의 기본 개념을 이해해야 하며, 사용시 정확한 위치로 이동/첨부 및 접근성을 고려한 정확한 처리가 필요하다.

1. **a** 앵커 라고도 하며, 연결해놓은 링크 위치/페이지로 이동하는 기능을 담고 있다.
	- `href=" "` 앵커의 속성중 하나로 정해진 위치를 찾아가는데 필요하다(웹페이지의 경우 프로토콜을 정확하게 입력해야함)
	- `target=" "` 클릭시 표기 및 처리 방식을 설정하는 기능으로 속성값으로는, ' _self ', ' _blank ', ' _parent ', ' _top ' 등이 있다.
2. **img** 이미지를 담는 요소(태그)로 정해진 이미지파일을 담아 보여주는 기능을 가지고 있다.
	- `src=" "` 이미지를 불러오는 소스의 속성으로 정해진 이미지를 불러올 경로값/ 파일이름을 작성한다.
	- `alt=" "` 불러온 이미지의 정확한 설명을 담는 기능으로, 임의의 값을 작성하는 것이아닌 정확한 설명을 필요로 한다.

### <a name="scope">5. 영역 및 이름부여</a>
> 의미를 특별하게 가지지는 않으나, 필요시 일정 공간 및 영역을 의미하는 코드가 필요하다 이때 사용하는 형태가 `<div>`, `<span>` 이다. 

- **div** 블록 형태의 요소이며, 특별한 의미는 가지지 않는다.(html5이후 좀더 정확한 의미 표현을 위해 추가코드가 생겼을 정도로 많은 양을 사용했었다.)
- **span** 인라인 형태의 요소이며, **div** 와 마찬가지로 특별한 의미는 없다.(여러 형태의 작업시 사용함)
- **id=" "** 각 요소에 이름을 부여하는 속성기능, 어느 요소에도 작성할 수 있으며, 페이지 내에서 단 한번만 사용이 가능하다. 이름의 의미 뿐 아니라 연결의 의미도 가진다.
- **class=" "** 각 요소에서 이름을 부여하는 속성기능, 어느 요소에서도 작성이 가능, 여러번 반복 사용할 수 있으며 하나의 요소에 여러개의 이름을 부여할 수 있다.


### <a name="table">6. table</a>
> 표형식을 되어진 요소를 **table** 이라고 한다.<br>
> 과거에는 대부분의 웹페이지들이 **table** 코드로 이루어져 있었으나 현재는 **table**의 정확한 의미의 목적으로만 사용되어지고 있음.
> ex: 날씨, 게시판, 주식차트, 경기표 등

1. **table** 시작을 알리며 table내용 전체를 감쌀때 사용
2. **caption** 표 작성시 제목을 표기하는 내용
3. **tr** 행을 의미하며 각셀값을 넣기 전 가로 행을 우선 작성하게 되어있다.
4. **th** 셀 제목을 의미하며 tr내부에 작성시 셀의 제목위치에 작성하도록 되어있다.
5. **td** 셀 내용을 의미 tr내부에 작성시 사용.
6. **thead** table 영역내부에서 상단 전체 제목영역에 사용됨 tr보다 부모태그 형태로 사용
7. **tbody** table 영역 내부의 중단에 표현할 내용을 담는다. thead 바로 뒤에 나타나는 형태
8. **tfoot** table 영역 내부의 말미에 표현할 내용을 담는다. 실제로 작성은 말미에 작성하지 않아도 thead/ tbody/tfoot순으로 배치가 된다.


### <a name="form">7. form</a>
>

1. **form**
2. **fieldset**
3. **legend**
4. **input**
5. **label**

### <a name="etc">8. etc</a>
>

1. **iframe**
2. **embed**
3. **map**  




___
## css 영역 기본 
1. [선택자](#select)
1. [크기값](#size)
2. [배경](#background)
3. [폰트](#fonts)
4. [float](#float)
5. [margin](#margin)
6. [padding](#padding)
7. [border](#border)
8. [outline](#outline)
9. [position](#position)


### <a name="select">1. 선택자</a>
> body 내부에 존재하는 tag, id, class 형태들을 선택해서 사용할 수 있게 만드는 것

1. **type** tag(요소)를 선택 (h1, p, div)
2. **자손**  `요소 요소` 형태로 사용 태그/id/class 이름간의 띄어쓰기로 구분, 자식을 포함한 그 후손형태의 요소를 선택( ul a {})
```html
<style>
  ul a{}  /* ul태그 후손태그 중 a태그를 선택 */
</style>
<body>
  <div class="box">
    <ul>
      <li><a href="">list_01</a></li>
      <li><a href="">list_02</a></li>
    </ul>
    <ol>
      <li>
        <ul>
          <li> <a href="">list2</a></li>
        </ul>     
    </ol>
  </div>
</body>
```
3. **자식** 자손선택자의 경우는 후손에 관련된건 모두 선택/ 자식만을 선택할 때에는 자식선택자를 사용한 이는 `태그(요소) > 태그(요소)` 사용
(ol li>ul a{})
4. **id** body에서 id값을 가진것은 css에서는 #의 형태로 보여주며, 이를 선택할때에는
```html
<style>
  #test1{} /* id 값이 test1인 요소를 찾아라 */
</style>
<body>
  <p id="test1">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Corrupti itaque natus molestiae quisquam ipsa modi, earum ex quo cupiditate accusamus quos nemo labore suscipit est eos nesciunt voluptatum. Ab, sit.</p>
   <p id="test2" class="class_test">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Corrupti itaque natus molestiae quisquam ipsa modi, earum ex quo cupiditate accusamus quos nemo labore suscipit est eos nesciunt voluptatum. Ab, sit.</p>
</body>
```
5.**class** body에서 class값을 가진것은 css에서는 .의 형태로 보여주며, 이를 선택할때에는 
```css
<style>
  .class_test{}
</style>
```

### <a name="size">2. 크기값</a>
> 크기값을 가지는 형태에게 사이즈를 주는 방법(width, height), 

px(하나의 점/ mm와 상대개념),
pt(인쇄시 9pt/ 웹 12pt), 
%(자신의 부모태그와 기준으로 설정되는 상대), 
em(반응형웹이 나오면서 설정된 단위), 
rem(em단위의 문제점을 해결하기 위해 나온 단위)
<!-- vh, vw, vmin, vmax -->
- 16px  = 12pt = 100% = 1em = 1rem (최초의 설정시)

### <a name="background">3. 배경</a>
> 배경과 관련된 모든것을 설정

1. background-color
1. background-image
1. background-repeat
1. background-position
1. background-attachment
1. background-size

### <a name="fonts">4. 폰트</a>
1. font-size
1. font-family
1. font-weight
1. font-style
1. line-height
1. color
1. text-aligh
1. text-indent

### <a name="float">5. float</a>
> block 태그의 형태를 옆으로 나열/ 바닥에 붙어있지 않고 떠있는 문제
> clear:both 

1. float:left; 
2. float:right;
3. clear:both;

### <a name="margin">6. margin</a>
> 각 태그(요소) 간의 공간(간격)을 만들어 주는것

1. margin:0 auto; - 공간을 위/아래는 없애고, 좌/우는 중간으로 배치(float기능과 같이 사용x)

### <a name="padding">7. padding</a>
> 각 태그(요소) 간의 공간(간격)을 만들어 주는것(자신의 형태가 커진듯한 효과)

### <a name="border">8. border</a>
> 외곽선(크기 o, 부피 o)

### <a name="outline">9. outline</a>
> 외곽선(크기 o, 부피 x)

### <a name="position">10. position</a>

