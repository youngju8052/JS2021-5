# 황영주[202030336]


## [05월 04일]
>1.기본 자료형과 객체 자료형의 차이<br/>
let number = 273;<br/>
let string = '안녕하세요';<br/>
let boolean = true;<br/>
<br/>
console.log(typeof number);<br/>
console.log(typeof string);<br/>
console.log(typeof boolean);<br/>
<br/>
<img src="picture/picture7-3.png" alt="캡쳐"><br/>

<br/><br/>

>2-1 메소드<br/>
예제 7-1<br/>
let number = 273.5210332;<br/>
<br/>
console.log(number.toFixed(1));<br/>
console.log(number.toFixed(4));<br/>

<img src="picture/예제7-1.png" alt="캡쳐"><br/>

>2-2 생성자 함수의 속성<br/>
예제 7-2<br/>
let numberA = Number.MAX_VALUE;<br/>
let numberB = Number.MAX_VALUE + 1;<br/>
<br/>
console.log(numberA);<br/>
console.log(numberB);<br/>
<br/>
<img src="picture/예제7-2.png" alt="캡쳐"><br/>

>3 String 객체<br/>
3-2메소드 활용 <br/>
예제 7-3<br/>
let string = '안녕하세요. 좋은 아침입니다.';<br/>
if(string.index0f('아침') >= 0){<br/>
    console.log('좋은 아침이에요...!');<br/>
}<br/>
<img src="picture/예제7-3.png" alt="캡쳐"><br/>

## [04월 27일]
>객체 기본
:객체는 여러개의 자료형을 한 번에 저장하는 자료형입니다.<br/>
<img src="picture/표6-3.png" alt="캡쳐"><br/>
6-1예제<br/>
let object = {<br/>
    name:'바나나',<br/>
    price: 1200<br/>
};<br/>
console.log(object.name);<br/>
console.log(object.price);<br/>

<img src="picture/예제6-1결과.png" alt="캡쳐"><br/>
<br/>
<br/>
>객체와 반복문
:생성한 객체에 for in 반복문으로 반복을 적용할 수 있습니다.<br/>
배열에 for in 반복문을 적용할 때 앞에 선언한 변수에 인덱스가 들어갔떤 것처럼, 객체에 for in 반복문을 적용하면 키가 들어갑니다.<br/>
예제6-2<br/>
let object = {<br/>
    name:'바나나',<br/>
    price: 1200<br/>
};<br/>
for(let key in object){<br/>
    console.log(`${key}: ${object[key]}`);<br/>
}<br/>

<img src="picture/예제6-2.png" alt="캡쳐"><br/>


## [04월13일]
>1 함수 생성
:이름을 붙이지 않고 생성하면 익명함수라고 하며, 이름을 붙여 생성하면 선언적 함수라고 한다.<br/>
1.1 익명함수<br/>
let 함수 = function (){<br/>
    console.log("함수의 첫번째 줄");<br/>
    console.log("함수의 첫번째 줄");<br/>
}<br/>
함수(a);<br/>
console.log(함수);<br/>
<br/>

1.2 선언적 함수<br/>
function 함수이름() { }<br/>
<br/>

1.3 화살표 함수<br/>
() => { }<br/>
<br/>

2 함수의 형태
<img src="picture/함수의형태.png" alt="캡쳐">

3.함수의 기본 활용<br/>
5-2예제<br/>
function sum(min,max) {<br/>
    let output = 0;<br/>
    for(let i = min; i <= max; i++){<br/>
        output += i;<br/>
    }<br/>
    return output;<br/>
}<br/>
<br/>
console.log(sum(1,100));<br/>

<img src="picture/예제_5-2.png" alt="예제결과">

4.함수 매개 변수 초기화<br/>
function print(name, count) {<br/>
    if(!count) {<br/>
        count = 1;<br/>
    }<br/>
<br/>
    console.log(`${name}이/가 ${count}개 있습니다.`)<br/>
}<br/>
print("사과");<br/><br/>

<img src="picture/예제_5-4.png" alt="예제결과"><br/>

5.콜백 함수<br/>
function callTenTimes(callback) {<br/>
    for(let i = 0; i < 10; i++>){<br/>
        callback();<br/>
    }<br/>
}<br/>
callTenTimes(function(){<br/>
    console.log('함수 호출');<br/>
});<br/><br/>

<img src="picture/예제_5-6.png" alt="예제결과"><br/>

## [04월06일]
>중첩 반복문
:반복문을 여러번 중첩해서 사용하면 중첩 반복문이라고 합니다.<br/>
별피라미드 예제<br/>
let output = "";<br/>
for (let i = 0; i < 8; i++) {<br/>
    for (let u = 0; u < 8 - i; u++) {<br/>
        output += " ";<br/>
    }<br/>
    for (let u = 0; u <= i*2; u++) {<br/>
        output += "*";<br/>
    }<br/>
    output += "\n";<br/>
}<br/>
console.log(output);<br/>
<img src="picture/피라미드.png" alt="예제결과"><br/>



>break키워드
:switch 조건문이나 반복문을 벗어날 때 사용<br/>
let i =0;<br/>
let foo = [1,3,5,7,9,2];<br/>
while (true){<br/>
    if(foo[i] % 2 == 0){<br/>
        output = foo[i];<br/>
        break;<br/>
    }<br/>
    i= i+1;<br/>
}<br/>
<br/>
console.log(`처음 발견한 짝수는 ${output}입니다`)<br/>
<img src="picture/break.png" alt="예제결과"><br/>

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