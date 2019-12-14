<!-- IGNORE THE HTML BLOCK BELOW, THE INTERESTING PART IS AFTER IT -->

<h1 align="center">Поппер. js</h1>

<p align="center">
    <strong>Библиотека, используемая для размещения выталкивания в веб-приложениях.</strong>
</p>

<p align="center">
    <img src="http://badge-size.now.sh/https://unpkg.com/popper.js/dist/popper.min.js?compression=brotli" alt="Stable Release Size"/>
  <img src="http://badge-size.now.sh/https://unpkg.com/popper.js/dist/popper.min.js?compression=gzip" alt="Stable Release Size"/>
    <a href="https://codeclimate.com/github/FezVrasta/popper.js/coverage"><img src="https://codeclimate.com/github/FezVrasta/popper.js/badges/coverage.svg" alt="Istanbul Code Coverage"/></a>
    <a href="https://www.npmjs.com/browse/depended/popper.js"><img src="https://badgen.net/npm/dependents/popper.js" alt="Dependents packages" /></a>
    <a href="https://spectrum.chat/popper-js" target="_blank"><img src="https://img.shields.io/badge/chat-on_spectrum-6833F9.svg?logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyBpZD0iTGl2ZWxsb18xIiBkYXRhLW5hbWU9IkxpdmVsbG8gMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB2aWV3Qm94PSIwIDAgMTAgOCI%2BPGRlZnM%2BPHN0eWxlPi5jbHMtMXtmaWxsOiNmZmY7fTwvc3R5bGU%2BPC9kZWZzPjx0aXRsZT5zcGVjdHJ1bTwvdGl0bGU%2BPHBhdGggY2xhc3M9ImNscy0xIiBkPSJNNSwwQy40MiwwLDAsLjYzLDAsMy4zNGMwLDEuODQuMTksMi43MiwxLjc0LDMuMWgwVjcuNThhLjQ0LjQ0LDAsMCwwLC42OC4zNUw0LjM1LDYuNjlINWM0LjU4LDAsNS0uNjMsNS0zLjM1UzkuNTgsMCw1LDBaTTIuODMsNC4xOGEuNjMuNjMsMCwxLDEsLjY1LS42M0EuNjQuNjQsMCwwLDEsMi44Myw0LjE4Wk01LDQuMThhLjYzLjYzLDAsMSwxLC42NS0uNjNBLjY0LjY0LDAsMCwxLDUsNC4xOFptMi4xNywwYS42My42MywwLDEsMSwuNjUtLjYzQS42NC42NCwwLDAsMSw3LjE3LDQuMThaIi8%2BPC9zdmc%2B" alt="Get support or discuss"/></a>
    <br />
    <a href="https://travis-ci.org/FezVrasta/popper.js/branches" target="_blank"><img src="https://travis-ci.org/FezVrasta/popper.js.svg?branch=master" alt="Build Status"/></a>
    <a href="https://saucelabs.com/u/popperjs" target="_blank"><img src="https://badges.herokuapp.com/browsers?labels=none&googlechrome=latest&firefox=latest&microsoftedge=latest&iexplore=11,10&safari=latest" alt="SauceLabs Reports"/></a>
</p>

<img src="https://raw.githubusercontent.com/FezVrasta/popper.js/master/popperjs.png" align="right" width=250 />

<!-- 🚨 HEY! HERE BEGINS THE INTERESTING STUFF 🚨 -->

## <a name="wut-poppers"></a>ВУТ? Выталкивания?

Поппер — это элемент на экране, который "выталкивает" из естественного процесса приложения.  
Распространенными примерами всплывающих подсказок являются подсказки, поповерс и раскрывающиеся окна.


## <a name="so-yet-another-tooltip-library"></a>Итак, еще одна библиотека всплывающих подсказок?

Ну, по сути, **нет**.  
Поппер. js — это **механизм позиционирования**, предназначенный для вычисления положения элемента, чтобы его можно было разместить рядом с заданном ссылочным элементом.  

Модуль полностью модульный и большинство его компонентов реализуются как **модификаторы** (аналогично промежуточным или подключаемым по).  
База кода целиком написана в ES2015, а ее компоненты автоматически тестируются на реальных браузерах с [сауцелабс](https://saucelabs.com/) и [трависЦи](https://travis-ci.org/).

Поппер. js имеет нулевые зависимости. Нет jQuery, без LoDash, Nothing.  
Он используется крупными компаниями, такими как [Twitter в начальной загрузке v4](https://getbootstrap.com/), [Майкрософт в веб](https://github.com/OneNoteDev/WebClipper) – [атласкит и атлассиан в](https://aui-cdn.atlassian.com/atlaskit/registry/).

### <a name="popperjs"></a>Поппер. js

Это обработчик, Библиотека, которая вычисляет и, при необходимости, применяет эти стили к средствам выталкивания.

Вот некоторые ключевые моменты:

- Располагать элементы в исходном контексте DOM (не запутаться с моделью DOM!);
- Позволяет экспортировать вычисляемые сведения для интеграции с другими библиотеками представлений;
- Поддерживает теневые элементы DOM;
- Полностью настраиваемая с учетом структуры модификаторов;

Посетите [страницу проекта](https://fezvrasta.github.io/popper.js) , чтобы увидеть множество примеров того, что можно делать с Поппер. js!

Здесь вы найдете [документацию](/docs/_includes/popper-documentation.md).


### <a name="tooltipjs"></a>ToolTip. js

Так как многим пользователям достаточно простого способа интеграции мощных всплывающих подсказок в своих проектах, мы создали **ToolTip. js**.  
Это небольшая библиотека, которая упрощает автоматическое создание всплывающих подсказок с помощью ядра Поппер. js.  
Его API почти идентичны с помощью знаменитой системы всплывающих подсказок начальной загрузки, таким образом, она будет легко интегрироваться в проекты.  
Всплывающие подсказки, создаваемые ToolTip. js, доступны благодаря `aria` тегам.

Здесь вы найдете [документацию](/docs/_includes/tooltip-documentation.md).


## <a name="installation"></a>Установка
Поппер. js доступен для следующих диспетчеров пакетов и сети CDN:

| Source |                                                                                  |
|:-------|:---------------------------------------------------------------------------------|
| npm    | `npm install popper.js --save`                                                   |
| Yarn   | `yarn add popper.js`                                                             |
| NuGet  | `PM> Install-Package popper.js`                                                  |
| Bower  | `bower install popper.js --save`                     |
| унпкг  | [`https://unpkg.com/popper.js`](https://unpkg.com/popper.js)                     |
| кднжс  | [`https://cdnjs.com/libraries/popper.js`](https://cdnjs.com/libraries/popper.js) |

Подсказка и JS:

| Source |                                                                                  |
|:-------|:---------------------------------------------------------------------------------|
| npm    | `npm install tooltip.js --save`                                                  |
| Yarn   | `yarn add tooltip.js`                                                            |
| Бовер * | `bower install tooltip.js=https://unpkg.com/tooltip.js --save`                   |
| унпкг  | [`https://unpkg.com/tooltip.js`](https://unpkg.com/tooltip.js)                   |
| кднжс  | [`https://cdnjs.com/libraries/popper.js`](https://cdnjs.com/libraries/popper.js) |

\*: Бовер не поддерживается, его можно использовать для установки ToolTip. js только траугх сети CDN unpkg.com. Этот метод имеет ограничение, недоступное для определения определенной версии библиотеки. Бовер и Поппер. js предлагают использовать для проектов NPM или Yarn.  
Для получения дополнительных сведений [Ознакомьтесь со связанной ошибкой](https://github.com/FezVrasta/popper.js/issues/390).

### <a name="dist-targets"></a>Целевые объекты Redist

В настоящее время Поппер. js поставляется с 3 целевыми объектами: УМД, ЕСМ и Еснекст.

- УМД — определение универсального модуля: AMD, Рекуирежс и глобальные компоненты;
- ЕСМ-ES modules: for Pack/ROLLUP или браузер, поддерживающий спецификацию;
- Еснекст: доступно в `dist/`, может использоваться с пакетом Pack и `babel-preset-env`;

Обязательно используйте нужную подправку. Если вы хотите импортировать его с помощью `<script>` тега, используйте УМД.

## <a name="usage"></a>Применение

При наличии существующего узла DOM Поппер запросите Поппер. js, чтобы разместить его рядом с кнопкой

```js
var reference = document.querySelector('.my-button');
var popper = document.querySelector('.my-popper');
var anotherPopper = new Popper(
    reference,
    popper,
    {
        // popper options here
    }
);
```

### <a name="callbacks"></a>Обратных вызовов

Поппер. js поддерживает два вида обратных вызовов, а `onCreate` обратный вызов вызывается после инициализации Поппер. `onUpdate` Он вызывается при каждом последующем обновлении.

```js
const reference = document.querySelector('.my-button');
const popper = document.querySelector('.my-popper');
new Popper(reference, popper, {
    onCreate: (data) => {
        // data is an object containing all the informations computed
        // by Popper.js and used to style the popper and its arrow
        // The complete description is available in Popper.js documentation
    },
    onUpdate: (data) => {
        // same as `onCreate` but called on subsequent updates
    }
});
```

### <a name="writing-your-own-modifiers"></a>Написание собственных модификаторов

Поппер. js основан на архитектуре "подключаемый модуль", большинство ее функций полностью инкапсулируются в качестве модификаторов.  
Модификатор — это функция, которая вызывается каждый раз, когда Поппер. js необходимо вычислить положение Поппер. По этой причине модификаторы должны быть очень производительными, чтобы избежать узких мест.  

Чтобы узнать, как создать модификатор, [прочитайте документацию по изменениям](docs/_includes/popper-documentation.md#modifiers--object)


### <a name="react-vuejs-angular-angularjs-emberjs-etc-integration"></a>Интеграция, Vue. js, угловая, AngularJS, Ембер. js (и т. д.)

Интеграция сторонних библиотек в реагирующие или в других библиотеках может быть очень недостаточной, так как они обычно изменяют модель DOM и блокируют библиотеки Crazy.  
Поппер. js применяет все изменения DOM в `applyStyle` пределах модификатора, вы можете просто отключить его и вручную применить координаты Поппер с помощью библиотеки выбора.  

Полный список библиотек, которые позволяют использовать Поппер. js в существующих платформах, можно найти на странице [упоминания](/MENTIONS.md) .

Кроме того, вы можете даже переопределить свой `applyStyles` собственный пользователь и интегрировать Поппер. js самостоятельно!

```js
function applyReactStyle(data) {
    // export data in your framework and use its content to apply the style to your popper
};

const reference = document.querySelector('.my-button');
const popper = document.querySelector('.my-popper');
new Popper(reference, popper, {
    modifiers: {
        applyStyle: { enabled: false },
        applyReactStyle: {
            enabled: true,
            fn: applyReactStyle,
            order: 800,
        },
    },
});

```

### <a name="migration-from-popperjs-v0"></a>Миграция из Поппер. js v0

Так как API изменился, мы подготовили некоторые инструкции по миграции для упрощения обновления до Поппер. js v1.  

https://github.com/FezVrasta/popper.js/issues/62

Если у вас возникнут вопросы, вы можете прокомментировать эту ошибку.

### <a name="performances"></a>перформанцес

Поппер. js очень производительно. Обычно он занимает 0,5 мс, чтобы вычислить положение Поппер (на ИМАК с Intel Core i5 с 3,5-е ГГц).  
Это означает, что он не будет вызывать никаких [жанк](https://www.chromium.org/developers/how-tos/trace-event-profiling-tool/anatomy-of-jank), что приводит к гладкому взаимодействию с пользователем.

## <a name="notes"></a>Примечания

### <a name="libraries-using-popperjs"></a>Библиотеки, использующие Поппер. js

Цель Поппер. js состоит в том, чтобы предоставить стабильный и мощный механизм позиционирования, готовый для использования в сторонних библиотеках.  

Посетите страницу [упоминания](/MENTIONS.md) , чтобы получить обновленный список проектов.


### <a name="credits"></a>Сведения об авторах
Я хочу поблагодарить некоторых друзей и проектов для работы, которая выполнялась следующим образом:

- [@AndreaScn](https://github.com/AndreaScn) для своей работы на странице GitHub и ручного тестирования, проведенного во время разработки;
- [@vampolo](https://github.com/vampolo) для исходной идеи и для имени библиотеки;
- [Сисдиг](https://github.com/Draios) все функции, полученные в течение этих лет, которые делают возможным написание этой библиотеки;
- Для [модема. js](http://github.hubspot.com/tether/) существуют проблемы с написанием библиотеки размещений, готовой для реального мира;
- [Участники](https://github.com/FezVrasta/popper.js/graphs/contributors) для получения очень оцененных запросов на включение внесенных изменений и отчетов об ошибках;
- **вы** хотите присвоить этому проекту звезду, чтобы сделать проект недопустимым.🙂

### <a name="copyright-and-license"></a>Авторские права и лицензия
Авторские права на код и документация 2016 **Федерико зиволо**. Код, выпущенный под [лицензией MIT](LICENSE.md). Документы, выпущенные в Creative Commons.
