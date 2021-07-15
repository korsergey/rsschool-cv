# Sergey Korotkov

## Junior front-end developer

#### Personal Information:
Nationality: Russian\
Date of Birth: 31.12.1994\
Location: Russia, Ryazan\
Marital status: Married\
Languages: Russian – Native, English - Beginner
#### Contacts:
Mobile phone number: +79521217083\
Email:sergeykorot49@gmail.com
#### Objective:
To obtain a position of junior front-end developer
#### Skils:
HTML, CSS, JavaScript - starting level.
#### Education:
**educational courses:**
+ HTML and CSS <https://stepik.org/course/38218/syllabus>. Сertificate of completion of the course <https://stepik.org/cert/977480>.
+ JavaScript for beginners <https://stepik.org/course/2223/syllabus>. Сertificate of completion of the course <https://stepik.org/cert/949026>.
+ HTML and CSS Basics <https://stepik.org/course/52164/syllabus>.
+ HTML for beginners <https://code-basics.com/languages/html>.
+ JavaScript for beginners <https://code-basics.com/languages/javascript>.

#### Code examples:
**Example 1. Training project.**\
Разметка html:
```
<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Procrastinate.</title>
  <link rel="stylesheet" href="style.css">
  
  <link rel="stylesheet" href="https://code.s3.yandex.net/web-code/adaptive.css">
  <link rel="icon" type="image" href="https://code.s3.yandex.net/web-code/js-favicon.ico">
</head>
<body>
  <div class="header">
    <p class="logo">Procrastinate.</p>
    <div class="button">Ещё идея</div>
  </div>

  <img class="image" src="https://code.s3.yandex.net/web-code/procrastinate/9.png">

  <div class="advice">
    <span>Не писать код, а</span>
    <span class="phrase">что бы поделать?</span>
    <img class="cursor" src="https://code.s3.yandex.net/web-code/cursor.gif">
  </div>

  <p class="footer">© 2020 Коротков</p>

  <script src="https://code.s3.yandex.net/web-code/smoothly.js"></script>
  <script src="script.js"></script>
</body>
```
CSS:
```
@font-face {
  src: url(https://code.s3.yandex.net/web-code/fonts/SuisseIntl-Book.woff);
  font-family: 'Suisse';
  font-weight: normal;
}

@font-face {
  src: url(https://code.s3.yandex.net/web-code/fonts/SuisseIntl-Bold.woff
);
  font-family: 'Suisse';
  font-weight: bold;
}

html {
  height: 100%;
  margin: 0;
  -webkit-font-smoothing: antialiased;
}

body {
  background-color: #323131;
  color: white;
  position: relative;
  max-width: 540px;
  min-height: 100%;
  margin: 0 auto;
  font-family: 'Suisse';
  box-sizing: border-box;
  padding: 36px;
}

.header {
  display: flex;
  align-items: baseline;
  justify-content: space-between;
}

.logo {
  font-weight: bold;
  font-size: 24px;
  margin: 0;
}

.button {
  width: 130px;
  height: 40px;
  padding-top: 10px;
  box-sizing: border-box;
  border: 1px solid white;
  text-align: center;
  font-size: 14px;
  cursor: pointer;
  transition: opacity 0.2s;
}

.button:hover {
  opacity: 0.5;
}

.image {
  width: 80%;
  display: block;
  margin: 60px auto 50px;
}

.advice {
  font-size: 42px;
  font-weight: bold;
  line-height: 1.1;
  margin-bottom: 70px;
}

.footer {
  font-size: 16px;
  margin: 0;
  position: absolute;
  bottom: 36px;
}
```
Код на JavaScript:
```javascript 
let phrases = [
  { text: 'отправить другу смешную гифку', image: 'https://code.s3.yandex.net/web-code/procrastinate/1.gif' },
  { text: 'посмотреть скидки на авиабилеты', image: 'https://code.s3.yandex.net/web-code/procrastinate/2.png' },
  { text: 'разобраться, о чём поют рэперы', image: 'https://code.s3.yandex.net/web-code/procrastinate/3.png' },
  { text: 'Юрий Дудь', image: 'https://code.s3.yandex.net/web-code/procrastinate/4.png' },
  { text: 'расставить книги на полке по цвету', image: 'https://code.s3.yandex.net/web-code/procrastinate/5.png' },
  { text: 'читать про зарплаты в Сан-Франциско', image: 'https://code.s3.yandex.net/web-code/procrastinate/6.png' },
  { text: 'прочитать новости и ужаснуться в комментариях', image: 'https://code.s3.yandex.net/web-code/procrastinate/7.png' },
  { text: 'попасть в поток грустных песен и вспомнить все ошибки молодости', image: 'https://code.s3.yandex.net/web-code/procrastinate/8.png' },
  { text: 'посмотреть трейлер сериала и заодно первый сезон', image: 'https://code.s3.yandex.net/web-code/procrastinate/9.png' },
  { text: 'проверить непрочитанное в Telegram-каналах', image: 'https://code.s3.yandex.net/web-code/procrastinate/10.png' }
];

function getRandomElement(arr) {
  let randIndex = Math.floor(Math.random() * arr.length);
  return arr[randIndex];
}

let button = document.querySelector('.button');
let phrase = document.querySelector('.phrase');
let advice = document.querySelector('.advice');
let image = document.querySelector('.image');

button.addEventListener('click', function () {
  let randomElement = getRandomElement(phrases);
  smoothly(phrase, 'textContent', randomElement.text)
  smoothly(image, 'src', randomElement.image)

  if (randomElement.text.length > 40) {
    advice.style.fontSize = '33px';
  } else {
    advice.style.fontSize = '42px';
  }
  
});
for (i=0; i<=2; i++){
  smoothly(phrase, 'textContent', phrases[i].text);
  smoothly(image, 'src', phrases[i].image);
}
```
**Example 2.** 
Implement the filterString () function, which accepts a string and a character as input, and returns a new string in which the passed character has been deleted in all its positions.

```javascript 
const filterString = (str, simbol) => {
  let i = 0;
  let result = '';
  while (i < str.length) {
    if (str[i] !== simbol) {
      result = result + str[i];
    }
    i++;
  }
  return result;
}
```
**Example 3.** 
The numbers a and b are given. Print a string with numbers from a to b separated by spaces. It is known that b is greater than a.
```javascript
function testCycle(a, b) {
    var x = '';
    b > a;
    for (let i = a;i <= b; i++) {
    x = x + ' ' + i }// Тут нужно написать решение
    console.log(x);
}
```
**Example 4.** 
The numbers a and b are given. Output a string with the numbers between a and b including the borders, sorted in ascending order. It is not known which of the numbers is greater, but it is known that both a and b are greater than 0.
```javascript
function testCycle(a, b) {
    var x = '';
    a > 0;
    b > 0;
    if (a > b) {
         for (let i = b; i <= a; i++) {
             x = x + ' ' + i};
    };
    if (a < b) {
         for (let i = a; i <= b; i++) {
             x = x + ' ' + i};
    };
     if (a ==b) {
     x = a;
     };
return x;
}
```
**Example 5.** 
Find the greatest common divisor of the numbers a and b.
```javascript
function testCycle(a, b) {
    var x = 0;  
    while (a != 0 && b != 0) {
        if (a >= b) {
            x = b; 
            a = a % b;
        } 
        else {
            x = a;
            b = b % a;
        }   
    }
    return x;}
```
Other code examples can be found at the link:<https://github.com/korsergey/https-github.com-korsergey-basic-js/tree/main/src>.
