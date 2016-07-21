## HTML & CSS Style Guide
__________________________

### I. 일반 작성 원칙

1. 들여쓰기  
 각 문단마다 2칸 들여쓰기를 한다. tab을 사용하지 말고, tab과 space를 혼용하여 사용하지 말 것

2. 대소문자  
	모든 코드는 소문자로 작성되어야 한다. HTML 요소의 이름, 속성, 속성값, CSS선택자,요소 및 요소값 모두에 이 규칙이 적용된다.

     ```html
        <!--Not recommended-->
        	<A HREF="/">Home</A>
        
        <!--Recommended-->
        <img src="bird.png" alt="bird">
    ```
3. 불필요한 공백 없애기  
	불필요한 공백은 무의미한 것이고, 문제를 일으킬 수 있다.



### II.HTML Style Guide

1. Document type  
HTML5로 작성하는 것을 권장한다.

2. Semantics  
각각의 요소들을 그 요소들의 목적에 맞춰 사용하도록 한다.  
예를 들면, heading요소는 heading에, p요소는 문단에 그리고 a요소를 링크를 거는 역할에 맞춰 사용하도록 한다. 접근성, 재사용, 그리고 코드 효율성을 위해 HTML 요소들을 그 목적에 맞춰 사용하도록 한다.

3. Multimedia  
이미지, 비디오, 애니메이션 오브젝트 같은 multimedia요소를 사용할 때는 접근성 관점을 고려하여야 한다.  
예를 들어, 이미지의 경우 alt속성을 이용하여 그 의미를 나타낸다면, 앞을 보지 못하는 장애인의 경우 그 이미지가 무엇을 의미하는지 알 수 있으며, 비장애인의 경우에도 그 이미지나 비디오의 컨텐츠가 무엇인지 정확히 파악할 수 있다.

4. type 속성  
type속성을 CSS나 JavaScriptstyle를 사용하는 경우라면 sheets나 script에 사용하지 않도록 한다.  
HTML5는 text/css와 text/javascript를 기본값으로 정의하고 있기 떄문에 type속성은 필요하지 않다.

5. 각각의 요소를 다른 줄에 작성  
block,list,table 같은 요소들을 각기 다른 줄에 작성하도록 한다. 또한, 그 요소들이 자식 요소일 경우 들여쓰기하도록 한다.

6. 따옴표  
class같이 따옴표가 필요한 속성의 경우, ' '(홑따옴표)보다는 " "(쌍따옴표)사용이 권장된다.
    
    ```html
    <!-- Not recommended -->
    <a class='button-set'>Click me</a>
    
    <!--Recommended-->
    <a class="button-set">Click me</a>
    ```

7. HTML Attribute(속성) 순서

    순서|속성
    ---|---
    1|rel
    2|type
    3|href,src
    4|width,height
    5|target
    6|id
    7|name
    8|class
    9|style
    10|title,alt
    11|기타 attribute
  
### III.CSS style Guide

1. ID와 Class 이름 정의  

    * ID와 Class의 이름을 정의할 때, 그 목적이 명확히 나타날 수 있도록 네이밍한다. ID나 Class의 이름이 길어지더라도 명시적으로 정의하는 것을 권장한다.

    * 또한, 선택자를 작성할 때, 불필요한 부모 요소의 사용을 사용하지 않도록 한다.
<<<<<<< HEAD
            
=======
			
>>>>>>> 5425c68460c6eed172bcf6f397833c83746b962c
     ```css
    /* Not recommended */
	ul#example{}
	div.error{}

	/* Recommended */
	#example{}
	.error{}
    ```

<<<<<<< HEAD
    * ID와 Class의 이름을 정의할 때 띄어쓰기를 사용한다면 그 공백을 하이픈(-)을 사용하여 네이밍 한다.  
    문제가 생겼을 때 찾기 수월하고 이해가 더 간편하도록 하이픈을 사용하며, 하이픈 이외 단어나 공백 혹은 기호로 사용하지 않도록 한다.
=======
	* ID와 Class의 이름을 정의할 때 띄어쓰기를 사용한다면 그 공백을 하이픈(-)을 사용하여 네이밍 한다.  
	문제가 생겼을 때 찾기 수월하고 이해가 더 간편하도록 하이픈을 사용하며, 하이픈 이외 단어나 공백 혹은 기호로 사용하지 않도록 한다.
>>>>>>> 5425c68460c6eed172bcf6f397833c83746b962c

2. 속기 작성  
	CSS는 속기형 작성을 지원한다. 속기 작성은 코드 효율성과 이해면에서 효과적이지만 명기적으로 표기하는 것을 권장한다.

3. 0 and Units  
	0 뒤에는 px, percent 등등의 Units을 사용하지 않도록 한다.
    ```css
    	margin: 0;
    	padding: 0;
    ```

4. Leading 0s  
<<<<<<< HEAD
    소수점을 표현하는데 있어 -1과 1 사이의 값이나 길이 앞에 0을 쓰지 않는다.
=======
	소수점을 표현하는데 있어 -1과 1 사이의 값이나 길이 앞에 0을 쓰지 않는다.
>>>>>>> 5425c68460c6eed172bcf6f397833c83746b962c
    ```css
    	 	font-size: .8em;
    ```

5. 따옴표  
<<<<<<< HEAD
    HTML과 다르게 " "(쌍따옴표)보다는 ' '(홑따옴표)의 사용을 권장한다.  또한, url값에는 따옴표를 사용하지 않도록 한다.
```css
         /* Not recommended */
            @import url("//www.naver.com/css/media.css");
=======
	HTML과 다르게 " "(쌍따옴표)보다는 ' '(홑따옴표)의 사용을 권장한다.  또한, url값에는 따옴표를 사용하지 않도록 한다.
```css
	     /* Not recommended */
			@import url("//www.naver.com/css/media.css");
>>>>>>> 5425c68460c6eed172bcf6f397833c83746b962c

			html {
			font-family: "open sans", arial, sans-serif;
			}

		/* recommended */
			@import url(//www.naver.com/css/media.css);

			html{
				font-family: 'open sans', arial, sans-serif;
			}
```

<<<<<<< HEAD
#####CSS 선언

- 선언 끝  
    각각의 선언문들은 세미콜론(;)으로 끝을 내야 한다.
        
    ```css
            /* Not recommended */
            .test{
            display:block;
            height: 100px
            }
    
            /* Recommended */
            .test{
            display:block;
            height: 100px;
            }
    ```

- CSS 속성 선언 순서  
    기억하기 쉽고 유지보수하기 쉽도록 코드를 알파벳 순서로 나열하도록 한다.  
    그러나, multiple vendor-specific prefixes(ex)-moz-border-radius etc...)의 경우에는 차례대로 나열하도록 한다.
=======
6. 선언 끝  
	각각의 선언문들은 세미콜론(;)으로 끝을 내야 한다.
		
    ```css
            /* Not recommended */
    		.test{
    		display:block;
    		height: 100px
    		}
    
    		/* Recommended */
    		.test{
    		display:block;
    		height: 100px;
    		}
    ```

7. CSS 속성 선언 순서  
	기억하기 쉽고 유지보수하기 쉽도록 코드를 알파벳 순서로 나열하도록 한다.  
	그러나, multiple vendor-specific prefixes(ex)-moz-border-radius etc...)의 경우에는 차례대로 나열하도록 한다.
>>>>>>> 5425c68460c6eed172bcf6f397833c83746b962c

    순서|속성|의미
    ---|---|---
    1| display|표
    2|overflow|넘침
    3|float|흐름
    4|position|위치
    5|z-index|정렬
    6|width & height|크기
    7|margin & padding|간격
    8|border|보더
    9|font|폰트
    10|background|배경
    11|etc(기타)|color,text-decoration,text-indent,clear...
