# [ 공식문서 예제 ]

# 이미지 변경자 추가하기

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
    <img name="a" src="images/my_picture.jpg" />
    <script src="scripts/main.js"></script>
  </body>
</html>
```

```javascript
let myImage = document.querySelector("img");

myImage.onclick = function () {
  let mySrc = myImage.getAttribute("src");
  if (mySrc === "images/my_picture.jpg") {
    myImage.setAttribute("src", "images/MimeMan.jpg");
  } else {
    myImage.setAttribute("src", "images/my_picture.jpg");
  }
};
```

이미지를 클릭이벤트로 이미지를 전환하는 코드
