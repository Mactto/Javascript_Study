# [ 공식문서 예제 ]

# 변수 선언 시 let과 var과 const의 차이

[Javascript 공식 문서](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Variables#The_difference_between_var_and_let)

1. 변수 초기화 후 선언
   **var은 변수를 먼저 초기화 한 후 선언이 가능함**

```javascript
a = "1234";

function print() {
  console.log(a);
}

var a; // 정상적으로 출력
let a; // 오류 발생
```

2. 변수 재선언
   **let은 한번만 var은 여러번 선언 가능**  
   변수가 여러번 선언될 필요성이 없기 떄문에 var의 단점이다.  
   떄문에 ES6 이후, 이를 보완하기 위해 let과 const가 추가되었다.

```javascript
var a = 1;
var a = 2; // 정상적으로 선언

let b = 1;
let b = 2; // 오류 발생
```
