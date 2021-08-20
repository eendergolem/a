<html lang="ru">
<head>
<meta charset="utf-8" />
<html>
 <head>
  <meta charset="utf-8">
 </head>
 <html>
  <head>
   <meta charset="utf-8">
   <title></title>
  </head>
  <body>
    <html lang="ru">

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
  <title>JavaScript SimpleAdaptiveSlider - Слайдер для сайта на чистом JavaScript [Example 02]</title>
  <!-- Подключаем CSS слайдера -->
  <link rel="stylesheet" href="/examples/libs/simple-adaptive-slider/simple-adaptive-slider.min.css">
  <!-- Подключаем JS слайдера -->
  <script defer src="/examples/libs/simple-adaptive-slider/simple-adaptive-slider.min.js"></script>
  <script>
    document.addEventListener('DOMContentLoaded', function () {
      // инициализация слайдера
      var slider = new SimpleAdaptiveSlider('.slider', {
        autoplay: false,
        interval: 5000,
        swipe: true,
      });
    });
  </script>
  <style>
    /* стили для элемента body */
    body {
      margin: 0;
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial,
        sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';
    }

    /* дополнительные стили для этого примера */
    .slider__items {
      counter-reset: slide;
    }

    .slider__item {
      counter-increment: slide;
    }

    .slider__item>div::before {
      content: counter(slide);
      position: absolute;
      top: 10px;
      right: 20px;
      color: #00FF00;
      font-style: italic;
      font-size: 32px;
      font-weight: bold;
    }
  </style>
</head>

</html>
 </html>
</html>
<style>
body{
  background:
#00FF00; /* Меняется фон экрана, выбирается здесь */
}

h1 {
    font-family: Verdana, Arial, Helvetica, sans-serif; /* Рубленый шрифт заголовка */
   }
   p {
    font-family: 'Times New Roman', Times, serif; /* Шрифт с засечками */
    font-style: italic; /* Курсивное начертание */
   }

#wrapper{ /* Оболочка страницы сайта */
  width: 1300px; /* Меняется ширина страницы */
  margin: 0 auto;
  background:#00FF00; /* Меняется задний фон страницы */
}

/* Шапка сайта */

#header{
position:relative; /* Задаём блоку относительное позиционирование для того, чтобы затем размещать, в нём другие элементы и позиционировать относительно его границ поверх фоновой картинки и заголовка */
  height: 250px; /* Высота шапки */
  background-color: #00FF00; /* Фон шапки */
   margin-bottom: 5px; /* Нижний отступ шапки от остального контента */
  border-radius: 5px; /* Закругляются углы блока */
  box-shadow: rgba(0,0,0,0.5) 0px 1px 3px; /* Тень. Визуально приподнимает блок над оболочкой */
}
img{ /* Фоновая картинка в шапке */
float: left; /* Разрешаем наплывание других элементов на картинку */
  margin: -40px 0 0 0;} /* Размещаем картинку в блоке header. 1-я и 3-я цифры - двигаем вверх-вниз, 2-я и 4-я цифры - двигаем вправо-влево */
h1{ /* Заголовок сайта */
  margin:0 0 10px 40px; /* Заголовок двигается верх-вправо-вниз-влево. */
  color:#464451; /* Цвет заголовка */
}
.nomer{ /*Подзаголовок (номер телефона)*/
  position:absolute; /* Позиционируем абсолютно подзаголовок, относительно границ блока header. Также можно разместить в шапке сайта ещё другие картинки и абзацы поверх фоновой картинки и заголовка */
  top:5px; /* Двигается вверх-вниз */
  left:680px; /* Двигается вправо-влево */
  font-size: 25px; /* Размер букв подзаголовка */
  font-style:italic; /* Курсив */
  font-weight:bold; /* Жирный */
  color:#464451; /* Цвет букв подзаголовка */
}

/* Сайдбар (колонка справа) */

#sidebar{ /* Блок сайдбара */
  background-color: #008080; /* Фон блока */
  width: 200px; /* Ширина блока */
  padding: 10px; /* Отступ текста от краёв */
  float: right; /* Размещаем блок справа от других элементов, наплывание или обтекание справа). Если делать сайдбар слева, то значение right меняем на left */
  border-radius: 5px; /* Закругляем углы блока */
  box-shadow: rgba(0,0,0,0.5) 0px 1px 3px; /* Задаём блоку тень */
}
#sideb{ /* Блок сайдбара */
  background-color: #0000CD; /* Фон блока */
  width: 200px; /* Ширина блока */
  padding: 10px; /* Отступ текста от краёв */
  float: right; /* Размещаем блок справа от других элементов, наплывание или обтекание справа). Если делать сайдбар слева, то значение right меняем на left */
  border-radius: 5px; /* Закругляем углы блока */
  box-shadow: rgba(0,0,0,0.5) 0px 1px 3px; /* Задаём блоку тень */
}
#side{ /* Блок сайдбара */
  background-color: #DAA520; /* Фон блока */
  width: 200px; /* Ширина блока */
  padding: 10px; /* Отступ текста от краёв */
  float: right; /* Размещаем блок справа от других элементов, наплывание или обтекание справа). Если делать сайдбар слева, то значение right меняем на left */
  border-radius: 5px; /* Закругляем углы блока */
  box-shadow: rgba(0,0,0,0.5) 0px 1px 3px; /* Задаём блоку тень */
}
.marcer{ /* Галочки маркеры меню */
  float: left; /* Размещаем слева от текста */
  margin: 5px 5px 0 0; /* Двигаются вверх-вправо-вниз-влево */
}

/* Контент (статья) */

#content{ /* Блок контента */
  margin-bottom: 5px; /* Отступ блока статьи от блока подвала */
  width: 800px; /* Ширина статьи */
  padding: 10px; /* Отступ текста от краёв блока */
  background: #50c878; /* Фон статьи */
  border-radius: 5px;
  box-shadow: rgba(0,0,0,0.5) 0px 1px 3px;sdsasdas
}
#sdsasdas{ /* Блок контента */
  margin-bottom: 8px; /* Отступ блока статьи от блока подвала */
  width: 850px; /* Ширина статьи */
  padding: 15px; /* Отступ текста от краёв блока */
  background: #50e878; /* Фон статьи */
  border-radius: 5px;
  box-shadow: rgba(0,0,0,0.5) 0px 1px 3px;
}
.left{
  float: left;
  margin: 30px 7px 7px 7px;
}
.right{ /* Картинка в тексте справа */
  float: right;
  margin: 7px 0 7px 7px;
}
/* Подвал */

#footer{ /* Блок подвала */
  height:80px; /* Высота блока подвала */
  background-color: #ffffff; /* Фон блока подвала */
  margin-bottom: 10px; /* Отступ снизу */
  border-radius: 5px; /* Закруглённые углы */
  box-shadow: rgba(0,0,0,0.5) 0px 1px 3px; /* Тень блока */
}
.clear{ /* Запрет наплывания. Устанавливается для того, чтобы блок контента, при заполнении текстом и изображениями не наплывал на подвал */
  clear: both;
}
  .fon{ /* Номер телефона */
  float:left; /* Разрешаем другим элементам обтекать абзац справа */
  margin:20px 0 0 20px;
}
.fax{ /* Номер факса */
  float:left;
  margin:20px 0 0 60px;
}
.mail{ /* Адрес E-mail */
  float:left;
 margin:20px 0 0 60px;
}
</style>
</head>
<body>
  <div id="wrapper"> <!--Оболочка страницы-->
<!--Шапка сайта-->
    <div id="header">
<!--Заголовок сайта-->
      <h1>Endergolem AD</h1>
<!--Описание (телефон)-->
        <p class="nomer"> <br> Официальний сайт канала endergolem</p>
<!--Фоновая картинка в шапке сайта-->
      <img src="https://static.wikia.nocookie.net/minecraft_ru_gamepedia/images/4/4f/EnderdragonFlying.gif/revision/latest?cb=20170318092936">
    </div>
<!--Сайдбар-->
    <div id="sidebar">
<!--меню-->
<h3>Наши web-услуги</h3>
<!--Картинки маркеров меню (галочки)-->
  <p><img class="marcer" src="http://trueimages.ru/img/99/91/dea39f15.png" width="10" height="10">Сайти</p>
  <p><img class="marcer" src="http://trueimages.ru/img/99/91/dea39f15.png" width="10" height="10">Youtube</p>
  <p><img class="marcer" src="http://trueimages.ru/img/99/91/dea39f15.png" width="10" height="10">3-D моделирование</p>
          <hr width="50" color="#00FF00" size="5">
<!--Общая информация в сайдбаре-->
      <h3>И так далее</h3>
    </div>
<!--Основной контент (статья)-->
    <div id="content">
<!--Картинка слева-->
      <img class="left" src="https://i.pinimg.com/originals/34/87/26/3487260ce5665ddf6286bc142673b7c6.gif">
<!--Заголовок статьи-->
        <h3>Реклама</h3>
<!--Текст статьи-->
<italic>Рекламу у меня на канале ви можете заказать за 1$</italic>
<p>На канале на момент последнего написания сайта 530 подпищиков</p>
<button>Купить</button>


<p>
</p>
    </div>
<!--Запрет наплывания-->
  <div class="clear"></div>
<html>
<head>
<style>
.mainmenubtn {
    background-color: green;
    color: yellow;
    border: none;
    cursor: pointer;
    padding:20px;
    margin-top:20px;
}
.dropdown {
    position: relative;
    display: inline-block;
}
.dropdown-child {
    display: none;
    background-color: yellow;
    min-width: 200px;
}
.dropdown-child a {
    color: green;
    padding: 20px;
    text-decoration: none;
    display: block;
}
.dropdown:hover .dropdown-child {
    display: block;
}
</style>
</head>
<body>
<div class="dropdown">
  <button class="mainmenubtn">3-D арт</button>
  <div class="dropdown-child">
    <li>Легкий стиль<s>60 грн</s><b>40 грн</b></li>
    <button>Купить</button>
    <li>Средний стиль<s>80 грн</s><b>60 грн</b></li>
    <button>Купить</button>
    <li>Сложний стиль<s>100 грн</s><b>80 грн</b></li>
    <button>Купить</button>
  </div>
</div>
</body>
</html>
</style>
</head>
<body>
<div class="dropdown">
  <button class="mainmenubtn">YouTube</button>
  <div class="dropdown-child">
    <li>Шапка<s>80 грн</s><b>20 грн</b></li>
    <button>Купить</button>
    <li>Інтро<s>100 грн</s><b>50 грн</b></li>
    <button>Купить</button>
    <li>Логотип<s>50 грн</s><b>30 грн</b></li>
    <button>Купить</button>
    <img class="left" src="https://www.meme-arsenal.com/memes/0cb82a8d2c2833a4475d6cda216e6830.jpg"
  </div>
</div>
</body>
</html>
  <html>
  <head>
  <style>
  .mainmenubtn {
      background-color: red;
      color: white;
      border: none;
      cursor: pointer;
      padding:20px;
      margin-top:20px;
  }
  .dropdown {
      position: relative;
      display: inline-block;
  }
  .dropdown-child {
      display: none;
      background-color: green;
      min-width: 200px;
  }
  .dropdown-child a {
      color: white;
      padding: 20px;
      text-decoration: none;
      display: block;
  }
  .dropdown:hover .dropdown-child {
      display: cover;
  }
  </style>
  </head>
  </html>
</div>
</body>
</html>
<body>
<div class="dropdown">
<button class="mainmenubtn">Игри</button>
<div class="dropdown-child">
  <li>Unity<s>120 грн</s><b>100 грн</b></li>
  <button>Купить</button>
  <li>Construct 3<s>80 грн</s><b>50 грн</b></li>
  <button>Купить</button>
  <img class="left" src="https://www.meme-arsenal.com/memes/0cb82a8d2c2833a4475d6cda216e6830.jpg"
</div>
</div>
</body>
</html>
<body>
<div class="dropdown">
  <button class="mainmenubtn">3-D проекти</button>
  <div class="dropdown-child">
    <li>3-D проект двух-етажного дома<s>700 грн</s><b>600 грн</b></li>
    <button>Купить</button>
    <li>3-D проект одно-етажного дома<s>300 грн</s><b>200 грн</b> </li>
    <button>Купить</button>
    <li>3-D проект дизайнерского предмета<s>100 грн</s><b>70 грн</b></li>
    <button>Купить</button>
    <li>3-D проект обичного моста<s>300 грн</s><b>200 грн</b></li>
    <button>Купить</button>
    <li>3-D проект роздвижного моста<s>1000 грн</s><b>800 грн</b></li>
    <button>Купить</button>
  </div>
</div>
</body>
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<title></title>
<style type="text/css">
body {
font: 0.8em Arial, Helvetica, sans-serif; /* Шрифт на веб-странице */
background: #00FF00; /* Цвет фона */
color: #000000; /* Цвет текста */
}
a { color: #008BCE; /* Цвет ссылок */ }
#container {
width: 1200px; /* Ширина макета */
margin: 0 auto; /* Выравниваем по центру */
background: #FCE600; /* Цвет колонок */
}
#hea {
font-size: 2em; /* Размер текста */
text-align: center; /* Выравнивание по центру */
padding: 3px; /* Отступы вокруг текста */
background: #B22222; /* Цвет фона шапки */
}
#sdsaf {
font-size: 2em; /* Размер текста */
text-align: center; /* Выравнивание по центру */
padding: 3px; /* Отступы вокруг текста */
background: #F73910; /* Цвет фона шапки */
}
#nav, #aside {
float: left; width: 75px; padding: 5px;
}
#content {
background: #54B948;
margin: 1px; /* Ширина колонок */
padding: 8px;
}
#cont {
background: #54B948;
margin: 1px; /* Ширина колонок */
padding: 6px;
}
#head {
background: #00008B;
margin: 1px; /* Ширина колонок */
padding: 8px;
}
#aside {
float: right; color: #000;
}
h2 { margin: 0 0 2em; }
#footer {
clear: both; /* Отменяем действие float */
padding: 14px; /* Отступы вокруг текста */
background: #D71920; /* Цвет фона подвала */
}
</style>
</head>
<body>
<div id="container">
<html>
  <head>
   <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
   <title>Покупка</title>
   <style type="text/css">
    acronym {
     border-bottom: 1px dashed blue; /* Подчеркивание текста */
     color: #000000; /* Цвет текста */
    }
    </body>
 </body>
</html>
  <style>
  .mainmenubtn {
      background-color: green;
      color: yellow;
      border: none;
      cursor: pointer;
      padding:20px;
      margin-top:20px;
  }
  .dropdown {
      position: relative;
      display: inline-block;
  }
  .dropdown-child {
      display: none;
      background-color: yellow;
      min-width: 200px;
  }
  .dropdown-child a {
      color: green;
      padding: 20px;
      text-decoration: none;
      display: block;
  }
  .dropdown:hover .dropdown-child {
      display: block;
  }
  </style>
  <body>

  </body>
  </html>

</div>
<div id="aside">
  <html>
  <head>
  <style>
  .mainmenubtn {
      background-color: green;
      color: yellow;
      border: none;
      cursor: pointer;
      padding:30px;
      margin-top:20px;
  }
  .dropdown {
      position: relative;
      display: inline-block;
  }
  .dropdown-child {
      display: none;
      background-color: black;
      min-width: 200px;
  }
  .dropdown-child a {
      color: green;
      padding: 20px;
      text-decoration: none;
      display: block;
  }
  .dropdown:hover .dropdown-child {
      display: block;
  }
  </style>
  </head>

<html>
<head>
<style>
.mainmenubtn {
    background-color: green;
    color: yellow;
    border: none;
    cursor: pointer;
    padding:20px;
    margin-top:20px;
}
.dropdown {
    position: relative;
    display: inline-block;
}
.dropdown-child {
    display: none;
    background-color: black;
    min-width: 200px;
}
.dropdown-child a {
    color: green;
    padding: 20px;
    text-decoration: none;
    display: block;
}
.dropdown:hover .dropdown-child {
    display: block;
}
</style>
</head>
<body>
  <html>
  <head>
  <style>
  .mainmenubtn {
      background-color: green;
      color: yellow;
      border: none;
      cursor: pointer;
      padding:20px;
      margin-top:20px;
  }
  .dropdown {
      position: relative;
      display: inline-block;
  }
  .dropdown-child {
      display: none;
      background-color: yellow;
      min-width: 200px;
  }
  .dropdown-child a {
      color: green;
      padding: 20px;
      text-decoration: none;
      display: block;
  }
  .dropdown:hover .dropdown-child {
      display: block;
  }
  <style>
  .mainmenubtn {
      background-color: yellow;
      color: yellow;
      border: none;
      cursor: pointer;
      padding:20px;
      margin-top:20px;
  }
  .dropdown {
      position: relative;
      display: inline-block;
  }
  .dropdown-child {
      display: none;
      background-color: yellow;
      min-width: 200px;
  }
  .dropdown-child a {
      color: yellow;
      padding: 20px;
      text-decoration: none;
      display: block;
  }
  .dropdown:hover .dropdown-child {
      display: block;
  }
  </style>
  </head>
  </div>
  </body>
  </html>


  <style>
  .mainmenubtn {
      background-color: yellow;
      color: green;
      border: none;
      cursor: pointer;
      padding:20px;
      margin-top:20px;
  }
  .dropdown {
      position: relative;
      display: inline-block;
  }
  .dropdown-child {
      display: green;
      background-color: green;
      min-width: 100px;
  }
  .dropdown-child a {
      color: green;
      padding: 10px;
      text-decoration: none;
      display: block;
  }
  .dropdown:hover .dropdown-child {
      display: block;
  }
  </style>

  </body>
  </html>
  <body>
</div>
</body>
</div>
</body>
</html>
</div>
</body>
</html>
         </style>
        </head>

      </html>

      <html>
       <head>
        <title>Ширина</title>
        <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
        <style type="text/css">
         #layer1 {
          width: 100%; /* Ширина первого слоя */
          padding: 10px; /* Поля вокруг текста */
          background: #fa0; /* Цвет фона */
         }
         #layer2 {
          width: 100%; /* Ширина второго слоя */
          background: #cc0; /* Цвет фона */
         }
         #layer2 P {
          padding: 10px; /* Поля вокруг параграфа */
         }
         #layer3 {
          background: #3ca; /* Цвет фона третьего слоя */
          padding: 10px; /* Поля вокруг текста */
         }
        </style>
       </head>
       <body>
        <div id="layer1">При покупке двух продуктов, второй идет в стоимость 75%</div>
        <div id="layer2"><p>При покупке трех продуктов, третий идет в стоимость 50%</p></div>
        <div id="layer3">При покупке четирех продуктов, четвертий идет в стоимость 25%</div>
       </body>
      </html>
         }
        </style>
       </head>
       <body>
        <div id="container">
         <div id="#layer1">Сайти</div>
         <div id="side">
          <h3>Тип сайта</h3>
          <p>Сайт-Биография</p>
          <p>Сайт-магазин</p>
          <p>Сайт-откритка</p>
         </div>
         <div id="aside">
          <h3>Цена</h3>
          <p>75 грн</p>
          <p>100 грн</p>
          <p>25 грн</p>
         </div>
         <div id="cont">
         <strong>На моем сайте ви можете заказать код для вашего сайта</strong>
          <ul>
           <li></li>
           <li></li>
           <li></li>
           <li></li>
           <li></li>
          </ul>
         </div>
        </div>
       </body>
      </html>
      <html>
       <head>
        <meta charset="utf-8">
        <title></title>
        <style>
         body {
          font: 11pt Arial, Helvetica, sans-serif; /* Рубленый шрифт текста */
          margin: 0; /* Отступы на странице */
         }
         h1 {
          font-size: 36px; /* Размер шрифта */
          margin: 0; /* Убираем отступы */
          color: #fc6; /* Цвет текста */
         }
         h2 {
          margin-top: 0; /* Убираем отступ сверху */
         }
         #header { /* Верхний блок */
          background: #0080c0; /* Цвет фона */
          padding: 10px; /* Поля вокруг текста */
         }
         #sidebar { /* Левая колонка */
          float: left; /* Обтекание справа */
          border: 1px solid #333; /* Параметры рамки вокруг */
          width: 20%; /* Ширина колонки */
          padding: 5px; /* Поля вокруг текста */
          margin: 10px 10px 20px 5px; /* Значения отступов */
         }
         #content { /* Правая колонка */
          margin: 10px 5px 20px 25%; /* Значения отступов */
          padding: 5px; /* Поля вокруг текста */
          color: #0000FF;
          border: 1px solid #333; /* Параметры рамки */
         }
         #footer { /* Нижний блок */
          background: #333; /* Цвет фона */
          padding: 5px; /* Поля вокруг текста */
          color: #fff; /* Цвет текста */
          clear: left; /* Отменяем действие float */
         }
        </style>
       </head>
       <body>
        <div id="head"><h1>Продажа мелодий на заказ</h1></div>
        <div id="#sideb"
          <img class="left" src="https://i.gifer.com/7vnr.gif">
        </div>
        <div id="content">
          <h2>Цена соответственно по порядку </h2>
          <p>2 вида бита, мелодия длиной 1 минуту=10 грн</p>
          <p>3 вида битов, мелодия длиной 2 минути=20 грн</p>
          <p>8 видов битов, мелодия длиной 2 минути=30 грн</p>
        <button>Купить</button>
       </body>
      </html>
      <html>
       <head>
        <meta charset="utf-8">
        <title></title>
        <style>
         body {
          font: 11pt Arial, Helvetica, sans-serif; /* Рубленый шрифт текста */
          margin: 0; /* Отступы на странице */
         }
         h1 {
          font-size: 36px; /* Размер шрифта */
          margin: 0; /* Убираем отступы */
          color: #fc6; /* Цвет текста */
         }
         h2 {
          margin-top: 0; /* Убираем отступ сверху */
         }
         #header { /* Верхний блок */
          background: #0071c0; /* Цвет фона */
          padding: 12px; /* Поля вокруг текста */
         }
         #sidebar { /* Левая колонка */
          float: left; /* Обтекание справа */
          border: 1px solid #333; /* Параметры рамки вокруг */
          width: 20%; /* Ширина колонки */
          padding: 7px; /* Поля вокруг текста */
          margin: 15px 7px 15px 7px; /* Значения отступов */
         }
         #content { /* Правая колонка */
          margin: 15px 7px 15px 7%; /* Значения отступов */
          padding: 7px; /* Поля вокруг текста */
          border: 5px solid #343; /* Параметры рамки */
         }
         #footer { /* Нижний блок */
          background: #335; /* Цвет фона */
          padding: 6px; /* Поля вокруг текста */
          color: #fdf; /* Цвет текста */
          clear: left; /* Отменяем действие float */
         }
        </style>
        </body>
      </head>
    </style>
    </head>
  </ul>
 </div>
</div>
</body>
</html>
<body>
<img class="left" src="https://img1.picmix.com/output/stamp/normal/2/9/6/0/210692_86d98.gif">
<img class="left" src="https://img1.picmix.com/output/stamp/normal/2/9/6/0/210692_86d98.gif">
 <div id="sdsaf"><h1>Робототехника</h1></div>
 <div id="#layer1">

 </div>
 <div id="#sdsasdas">
   <div id="sdsasdas">
     <ul>
  <li><strong>Алгоритм шага = 10 грн</strong></li>
  <li><strong>Алгоритм переноски об'єктов = 20 грн</strong></li>
  <li><strong>Алгоритм анализирования и преодаления припятствий = 50 грн</strong></li>
  <li><strong>Алгоритм анализирования, преодаления припятствий і переноски предметов = 75 грн</strong></li>
  <button>Купить</button>
    <ul>
</body>
</html>
<html>
<head>
 <meta charset="utf-8">
 <title></title>
 <style>
  body {
   font: 11pt Arial, Helvetica, sans-serif; /* Рубленый шрифт текста */
   margin: 0; /* Отступы на странице */
  }
  h1 {
   font-size: 36px; /* Размер шрифта */
   margin: 0; /* Убираем отступы */
   color: #fc6; /* Цвет текста */
  }
  h2 {
   margin-top: 0; /* Убираем отступ сверху */
  }
  #header { /* Верхний блок */
   background: #2151b0; /* Цвет фона */
   padding: 12px; /* Поля вокруг текста */
  }
  #sidebar { /* Левая колонка */
   float: left; /* Обтекание справа */
   border: 1px solid #333; /* Параметры рамки вокруг */
   width: 20%; /* Ширина колонки */
   padding: 7px; /* Поля вокруг текста */
   margin: 15px 7px 15px 7px; /* Значения отступов */
  }
  #content { /* Правая колонка */
   margin: 25px 7px 15px 7%; /* Значения отступов */
   padding: 20px; /* Поля вокруг текста */
   border: 5px solid #343; /* Параметры рамки */
  }
  #footer { /* Нижний блок */
   background: #1243; /* Цвет фона */
   padding: 6px; /* Поля вокруг текста */
   color: #faf; /* Цвет текста */
   clear: left; /* Отменяем действие float */
  }
 </style>
 </body>
</head>
</style>
</head>
</ul>
</div>
</div>
</body>
</html>
<body>
 <div id="hea"><h1>Обработка фото</h1></div>
 <div id="#layer1">

 </div>
 <div id="#content">
   <div id="content">
     <ul>
  <li><strong>Наложение одного ефекта = 2 грн</strong></li>
  <li><strong>Наложение двух ефектов= 3 грн</strong></li>
  <li><strong>Подравнение деформаций (лица) = 5 грн</strong></li>
  <li><strong>Подравнение деформаций (тела) = 10 грн</strong></li>
  <button>Купить</button>
    <ul>
</body>
</div>
</div>
<body>
   <div id="nav">
     <body>
      <div id="sdsaf"><h1>Мульт</h1></div>
      <div id="#layer1">

      </div>
      <div id="#sdsasdas">
        <div id="sdsasdas">
          <img class="left" src="https://thumbs.gfycat.com/AmbitiousBleakHornet-max-1mb.gif">
      <li><strong>Мульт на бумаге</strong><p>30 грн</p></li>
      <li><strong>Мульт из домино</strong><p>50 грн</p></li>
      <li><strong>Мульт на комп. графике</strong><p>75 грн</p></li>
            <button>Купить</button>
     </body>
     </html>
   </div>
     <li></li>
     <li></li>
     <li></li>
     <li></li>
     <li></li>
<div id="sdsaf"><h1>Продажа готовой компании</h1></div>
<div id="sdsaf"><h1>(с бизнес схемой)</h1></div>
<div id="content">
  <li><strong>Masterskaya GOLEM</strong><p>                               500 грн</p></li>
  <li><strong>SMM Ender</strong><p>                               350 грн</p></li>
  <li><strong>Multi Golem</strong><p>                               200 грн</p></li>
<button>Купить</button>
