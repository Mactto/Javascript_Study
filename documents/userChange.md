# [ 공식문서 예제 ]

# 바뀐 사용자 환영 메세지

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
    <button>Change user</button>
    <h1></h1>
    \
    <script src="scripts/main.js"></script>
  </body>
</html>
```

```javascript
let myButton = document.querySelector("button");
let myHeading = document.querySelector("h1");

function setUsername() {
  let myName = prompt("Please enter your name.");
  localStorage.setItem("name", myName);
  myHeading.textContent = "Mozilla is cool, " + myName;
}

if (!localStorage.getItem("name")) {
  setUsername();
} else {
  let storedName = localStorage.getItem("name");
  myHeading.textContent = "Mozilla is cool, " + storedName;
}

myButton.onclick = function () {
  setUsername();
};
```

사용자가 변경되었을 경우 환영메세지를 해당 사용자에 맞게 설정

```javascript
if (!myName || myName === null) {
  setUserName();
}
```

null 입력 방지
