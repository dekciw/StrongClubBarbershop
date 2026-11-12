<p align="center">
  <img src="screenshots/logo.png" width="220" alt="Strong Club Barbershop">
</p>

<p align="center">
  <b>Лендинг мужского барбершопа: прайс на услуги, слайдер мастеров и онлайн-запись с выбором даты и времени.</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/Sass-SCSS-CC6699?logo=sass&logoColor=white" alt="SCSS">
  <img src="https://img.shields.io/badge/jQuery-0769AD?logo=jquery&logoColor=white" alt="jQuery">
  <img src="https://img.shields.io/badge/Gulp-CF4647?logo=gulp&logoColor=white" alt="Gulp">
  <a href="https://dekciw.github.io/StrongClubBarbershop/"><img src="https://img.shields.io/badge/GitHub_Pages-online-222222?logo=github&logoColor=white" alt="GitHub Pages"></a>
</p>

<p align="center">
  <a href="https://dekciw.github.io/StrongClubBarbershop/">
    <img src="https://img.shields.io/badge/Открыть_в_браузере-B08D57?style=for-the-badge" alt="Открыть в браузере">
  </a>
</p>

<br>

<p align="center">
  <img src="screenshots/screen-hero.png" width="900" alt="Первый экран: Создайте деловой имидж, который достоин Вас">
</p>

<br>

<table align="center">
  <tr>
    <th>&#8199;&#8199;&#8199;&#8199;&#8199;&#8199;Разделы&#8199;&#8199;&#8199;&#8199;&#8199;&#8199;</th>
    <th>&#8199;&#8199;&#8199;&#8199;&#8199;&#8199;Запись&#8199;&#8199;&#8199;&#8199;&#8199;&#8199;</th>
    <th>&#8199;&#8199;&#8199;&#8199;&#8199;&#8199;Вёрстка&#8199;&#8199;&#8199;&#8199;&#8199;&#8199;</th>
  </tr>
  <tr>
    <td valign="top">
      - О барбершопе<br>
      - Прайс на 14 услуг<br>
      - Скидка 15% новым гостям<br>
      - Слайдер мастеров<br>
      - Карта и контакты<br>
      - Анимации при прокрутке
    </td>
    <td valign="top">
      - Выбор услуги и мастера<br>
      - Календарь для даты<br>
      - Выбор времени<br>
      - Маска телефона<br>
      - Ошибки под каждым полем<br>
      - Отправка на тестовый сервер
    </td>
    <td valign="top">
      - Адаптив до 320 px<br>
      - Мобильное меню<br>
      - Стили на Sass<br>
      - Сборка CSS через Gulp<br>
      - jQuery и плагины<br>
      - Сайт на GitHub Pages
    </td>
  </tr>
</table>

<h3 align="center">Как это выглядит</h3>

<table align="center">
  <tr>
    <td width="50%" align="center" valign="top">
      <img src="screenshots/screen-about.png" width="420" alt="О барбершопе"><br>
      <sub>О барбершопе</sub>
    </td>
    <td width="50%" align="center" valign="top">
      <img src="screenshots/screen-price.png" width="420" alt="Прайс на услуги"><br>
      <sub>Прайс на услуги</sub>
    </td>
  </tr>
  <tr>
    <td width="50%" align="center" valign="top">
      <img src="screenshots/screen-masters.png" width="420" alt="Слайдер мастеров"><br>
      <sub>Мастера</sub>
    </td>
    <td width="50%" align="center" valign="top">
      <img src="screenshots/screen-mobile.png" width="150" alt="Мобильная версия"><br>
      <sub>Мобильная версия</sub>
    </td>
  </tr>
</table>

<br>

<details>
<summary><b>Подробнее о проекте: стек, устройство, запуск</b> (нажми, чтобы развернуть)</summary>

<br>

### Стек

<p>
- <b>Вёрстка:</b> HTML и Sass (SCSS), стили собираются Gulp в <code>dist/style.min.css</code><br>
- <b>Скрипты:</b> jQuery, jQuery UI, Masked Input для телефона<br>
- <b>Плагины:</b> Slick для слайдера мастеров, Air Datepicker для даты, WOW.js и Animate.css для анимаций
</p>

### Структура

```
.
├── index.html              # вся страница
├── gulpfile.js             # сборка SCSS в один минифицированный CSS
├── dist/style.min.css      # готовые стили, которые подключает страница
├── src/
│   ├── styles/             # исходники SCSS: основа, адаптив, кнопки, плагины
│   ├── scripts/index.js    # меню, прокрутка, слайдер, календарь, проверка и отправка формы
│   ├── scripts/            # jQuery и плагины
│   ├── images/             # фото, иконки и логотип
│   ├── fonts/              # шрифты
│   └── slick/              # стили слайдера
└── screenshots/            # скриншоты для README
```

### Как работает запись

Кнопка «Записаться» у мастера открывает форму. Все поля обязательны: если что-то не заполнено, под полем появляется подсказка. Заполненная форма отправляется на учебный сервер `testologia.ru`, после ответа показывается благодарность.

### Запуск

Откройте `index.html` в браузере, сборка не нужна: готовый CSS уже лежит в `dist/`. Чтобы пересобрать стили после правок в SCSS:

```bash
npm install
npx gulp
```

</details>
