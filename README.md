# 황영주[202030336]

## [04월06일]

## [03월30일]
>중첩 조건문
:조건문 안에 조건문을 중첩해 사용하는것<br/>
if(불 표현식){<br/>
    if(불 표현식){<br/>
        문장;<br/>
    } else{<br/>
        문장<br/>
    }<br/>
} else{<br/>
    if(불 표현식){<br/>
        문장;<br/>
    } else{<br/>
        문장;<br/>
    }<br/>
}<br/>

>switch 조건문
switch(비교할 값) {<br/>
    case 값:<br/>
        문장<br/>
        break;<br/>
    case 값:<br/>
        문장<br/>
        break;<br/>
    default:<br/>
        문장<br/>
        break;<br/>
}<br/>
break는 switch 조건문이나 반복문을 빠져나갈 때 사용<br/>
>삼향 연산자<br/>
연산자이지만 프로그램의 진행을 조건에 따라 변화시킬수 있다<br/>
<불 표현식> ? 참:거짓<br/>
console.log(number %2 == 0? true:false);<br/>

>|| 연산자<br/>
let test;<br/>

test = test || "초기화합니다_1"<br/>
console.log(test);<br/>
<br/>
test = test || "초기화합니다_2"<br/>
console.log(test);<br/>
<br/>
>배열<br/>
:여러 개의 자료를 한꺼번에 다룰 수 있는 자료형입니다<br/>
let array = [52, 273,'아침','점심',true,false]<br/>

## [03월23일]

>문자열
    기본 문자열: 자바스크립트는 기본적인 문자열을 생성할 때 큰따옴표나 작은따옴표를 사용합니다.
    이스케이프 문자
## [03월16일]

>자바스크립트로 할 수 있는 일
2010년까지만 해도 웹 클라이언트 개발 이외의 용도로는 사용할 수 없었다<br/>
그 이후부터 서버, 게임, 스마트폰 애플리케이션, 데스크톱 애플리케이션 개발 등에 사용하면서 굉장히 다양한 일을 할 수 있게 되었습니다.<br/>
자바스크립트로 만든 데스크톱 애플리케이션 아톰 VSCode GitKraken<br/>
유니티는 모노 플랫폼을 사용해 자바스크립트를 기반으로 만든 유니티 스크립트를 통해 다양한 플랫폼을 만들어냈다<br/>

>자바스크립트 실행 방법 명령프롬프트와 node를 이용하여 실행을 직접해봤다
hello.html을 연습실행해보았습니다

>값을 만들어 내는 간단한 코드를 표현식이라고 하고 표현식이 하나 이상 모이면 문장이라 한다. 문장 끝에는 ;을 찍어준다. 그리고 문장이 모이면 프로그래이 된다. 

>키워드 
break else instanceof true case false new try catch finally null typeof continue for return var default function switch void delete if this while do in throw with let const 등이 있다. 다음에 공부할때 다 배우니 키워드가 있다고만 알고 있자.

>식별자는 이름을 붙일 때 사용하는 단어, 변수와 함수의 이름으로 사용
    키워드를 사용하면 안됩니다.
    특수문자는 _와 $만 허용합니다.
    숫자로 시작하면 안 됩니다.
    공백은 입력하면 안 됩니다.

>주석을 사용하는 방법을 알았습니다.
// 한 줄 주석처리
/* 여러 줄 주석처리 */