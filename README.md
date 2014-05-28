FreeDom For People
====

Открытый проект по созданию сайта FreeDom For People на базе CMF [MODx](http://modx.com).

## Содержание

 - [Введение](#Введение)
 - [Документация](#Документация)
 - [Ошибки и пожелания по расширению функциональности](#Ошибки-и-пожелания-по-расширению-функциональности)
 - [Компиляция CSS и JavaScript](#Компиляция-CSS-и-JavaScript)
 - [Требования](#Требования)
 - [Сообщество](#Сообщество)
 - [Контроль версий](#Контроль-версий)
 - [Авторы](#Авторы)
 - [Авторское право и лицензия](#Авторское-право-и-лицензия)

##Введение

Есть как минимум два способа начать работу с шаблоном сайта:

 - [скачать архив с последней версией](https://github.com/Realetive/fdfp/archive/master.zip);
 - скопировать репозиторий: ```git clone https://github.com/Realetive/fdfp.git```.

###Что внутри?

После того, как вы скачали файлы и распаковали архив, вы увидите приблизительно следующее:

```
fdfp/
├── docs/
│   └── …
├── src/
│   ├── fonts/
│   │   ├── glyphicons-halflings-regular.eot
│   │   ├── glyphicons-halflings-regular.svg
│   │   ├── glyphicons-halflings-regular.ttf
│   │   └── glyphicons-halflings-regular.woff
│   ├── ico/
│   │   ├── 18x18.png
│   │   ├── 50x50.png
│   │   ├── 128x128.png
│   │   ├── apple-touch-icon-57-precomposed.png
│   │   ├── apple-touch-icon-72-precomposed.png
│   │   ├── apple-touch-icon-114-precomposed.png
│   │   ├── apple-touch-icon-144-precomposed.png
│   │   └── favicon.ico
│   ├── img/
│   │   └── …
│   ├── js/
│   │   ├── bootstrap/
│   │   │   └── *.js
│   │   └── custom.js
│   ├── pic/
│   │   └── …
│   └── style/
│       ├── bootstrap/
│       │   └── *.less
│       ├── custom.css
│       └── custom.less
├── CONTRIBUTING.md
├── LICENSE
├── index.html
└── README.md
```

Как вы уже могли догадаться, шаблон вёрстки FreeDom For People создаётся на базе CSS-фреймворка [Bootstrap](http://getbootstrap.com/).
Директория ```src``` содержит файлы, необходимые для вёрстки: шрифтовые иконки, фавиконы, графические материалы, файлы скриптов и стилей.

##Документация

Документация в разработке, потому что пока не о чем писать…

##Ошибки и пожелания по расширению функциональности

Нашли ошибку или есть интересная идея? Для начала, пожалуйста, ознакомьтесь с [руководством](http://google.com) и попробуйте найти существующие и закрытые проблемы на [трекере](https://github.com/Realetive/fdfp/issues). Если ваш вопрос ранее не рассматривался, вы можете [создать новое обсуждение](https://github.com/Realetive/fdfp/issues/new).

##Компиляция CSS и JavaScript

FreeDom for People использует [LESS](http://lesscss.org/) [[?]](http://ru.wikipedia.org/wiki/LESS_(%D1%8F%D0%B7%D1%8B%D0%BA_%D1%81%D1%82%D0%B8%D0%BB%D0%B5%D0%B9)) для генерации таблицы стилей на стороне клиента. Для этого можно использовать командную строку или плагины (напр., *less2css* для SublimeText или *LESS support* для PHPStorm).

##Требования

Все требования изложены в [CONTRIBUTING.md](CONTRIBUTING.md), включая управление существующими обращениями в трекере, оформление кода и заметки к совместной разработке.

##Сообщество

Проект развивается при поддержке клуба [MODx Санкт-Петербург](http://modx.spb.ru)

##Контроль версий

Для обеспечения прозрачности в нашем цикле разработок и создания обратной совместимости принят семантический принцип управления версиями. Иногда изменения могут противоречить этому принципу, но мы постараемся этого избежать, если это возможно.

Релизы будут пронумерованы в следующем формате:

`<major>.<minor>.<patch>`

Они будут придерживаться следующего принципа:

 - нарушение обратной зависимости обновляет major-ветку с обнулением minor- и patch-последовательности;
 - добавление функционала увеличивает minor-версию с обнулением patch-последовательности;
 - исправление ошибок и незначительные улучшения повышают patch-версию.

С более подробной информацией о Семантическом Версионировании вы можете ознакомиться на <http://semver.org/>.

##Авторы

**Роман *Realetive* Ганин**

 - <http://twitter.com/realetive>
 - <http://github.com/Realetive>
 - <http://vk.com/realetive>

##Авторское право и лицензия

Код, материалы и документация принадлежат [FreeDom For People](http://fdfp.ru). Код и документация распространяются по [лицензии Creative Commons](LICENSE).