# Framework life balance 

![ядро: v1.1.8.22](https://img.shields.io/badge/Ядро-v1.1.8.22-blue.svg) ![интерфейс: v1.0.7.24](https://img.shields.io/badge/Интерфейс-v1.0.7.24-blue.svg)

Framework life balance предназначен для **сопровождения** всех этапов разработки сайта (<a target="_blank" href="/Компоненты ядра/2.Условия/Структуры/Напутствующие/Напутствующая структура разработки.md">структура разработки ядра</a>) с любым масштабом на исходном php-коде, html-разметках ( css, image ) и js-скриптах, с опорой на холакратию и порядок. 

![hr](http://foto-video-montazh.ru/wa-data/public/site/img/0_b0251_20b04c67_orig-1.png)

### Состав

Framework life balance состоит из 10-ти компонентов:

| № | Компоненты ядра | Компоненты интерфейса
 ------------- |  ------------- | ------------- | 
| 1. | Ориентировка: цели, сведения, стандарты | Ориентировка: цели, сведения, стандарты
| 2. | Условия: структуры | Условия: структуры
| 3. | Распределение: нормативы | Распределение: нормативы
| 4. | Движение: протоколы, функции | Движение: протоколы, функции
| 5. | Модули | Модули

![hr](http://foto-video-montazh.ru/wa-data/public/site/img/0_b0251_20b04c67_orig-1.png)


### Среда

У Framework life balance две среды разработки: back-end (ядро) и front-end (интерфейс). 

![Framework life balance](/Компоненты%20интерфейса/2.Условия/Структуры/Картиночные/slider/slide1_bg.jpg)

Здесь нет места для php-кода в интерфейсе, и html-а в ядре. Ядро и интерфейс разделены и изолированы, что позволяет безпрепятственно разрабатывать оба направления одновременно, почтительно дополняя (без возникновения каких либо merge) на git'e.

![hr](http://foto-video-montazh.ru/wa-data/public/site/img/0_b0251_20b04c67_orig-1.png)


### Ядро

В ядре реализованы <a target="_blank" href="/Компоненты ядра/1.Ориентировка/Стандарты/Основополагающие">Стандарты</a> (детализация) ядра, наглядность <a target="_blank" href="/Компоненты ядра/2.Условия/Структуры/Функций">Структуры</a> (планировка), <a target="_blank" href="/Компоненты ядра/4.Движение/Функции/Компонентов">Функции 4-х компонентов</a> (распределенная альтернатива контролёров в mvc), <a target="_blank" href="/Компоненты ядра/4.Движение/Функции/Категорий сайта">Функции категорий сайта</a> (упрощённая альтернатива моделей в mvc) и <a target="_blank" href="/Компоненты ядра/3.Распределение/Нормативы/Функций">Нормативы</a> (упрощённая альтернатива yii2 migrate, установки и настроек). Благодаря такому подходу был реализован <a target="_blank" href="/Компоненты ядра/3.Распределение/Нормативы/Базы данных/Норматив таблиц базы данных.php">норматив таблиц базы данных</a> и функция автоматической реконструкции базы данных, что освободило разработчиков от необходимости конструировать sql-запросы вручную. А так же реализован внутренний самовызов из консоли, оттого на фоновый режим отработки была переведена отправка почтового сообщения и реструктуризация базы данных, что для пользователя значительно уменьшило время ожидания ответа, а у разработчиков отпала необходимость настраивать cron.

Стандарты: 

> Под стандартом понимается образец, эталон, модель.

- <a target="_blank" href="/Компоненты ядра/1.Ориентировка/Стандарты/Основополагающие/1.Основополагающий стандарт среды.md">Стандарт среды</a>
- <a target="_blank" href="/Компоненты ядра/1.Ориентировка/Стандарты/Основополагающие/2.Основополагающий стандарт кода.md">Стандарт кода</a>
- <a target="_blank" href="/Компоненты ядра/1.Ориентировка/Стандарты/Основополагающие/3.Основополагающий стандарт компонентов.md">Стандарт компонентов</a>
- <a target="_blank" href="/Компоненты ядра/1.Ориентировка/Стандарты/Основополагающие/4.Основополагающий стандарт разработки.md">Стандарт разработки</a>
- <a target="_blank" href="/Компоненты ядра/1.Ориентировка/Стандарты/Основополагающие/5.Основополагающий стандарт разработчиков.md">Стандарт разработчиков</a>
- <a target="_blank" href="/Компоненты ядра/1.Ориентировка/Стандарты/Нормативные/Стандарт норматива базы данных.md">Стандарт норматива базы данных</a>
- <a target="_blank" href="/Компоненты ядра/1.Ориентировка/Стандарты/Нормативные/Стандарт норматива взаимодействия с базой данных.md">Стандарт норматива взаимодействия с базой данных</a>
- <a target="_blank" href="/Компоненты ядра/1.Ориентировка/Стандарты/Нормативные/Стандарт норматива наработок.md">Стандарт норматива наработок</a>


Структуры:

> Под структурами понимается внутреннии устройства с их взаимосвязями.

- <a target="_blank" href="/Компоненты ядра/2.Условия/Структуры/Напутствующие/Напутствующая структура разработки.md">Структура разработки</a>
- <a target="_blank" href="/Компоненты ядра/2.Условия/Структуры/Базы данных/Структура таблиц базы данных.md">Структура таблиц базы данных</a>
- <a target="_blank" href="/Компоненты ядра/2.Условия/Структуры/Базы данных/Структура взаимодействия с базой данных.md">Структура взаимодействия с базой данных</a>
- <a target="_blank" href="/Компоненты ядра/2.Условия/Структуры/Функций/Структура функций компонентов.md">Структура функций компонентов</a>
- <a target="_blank" href="/Компоненты ядра/2.Условия/Структуры/Функций/Структура функций сайта.md">Структура функций сайта</a>


Нормативы:

> Под нормативом понимается объем деятельности, которому всегда принято следовать.

- <a target="_blank" href="/Компоненты ядра/3.Распределение/Нормативы/Компонентов/1.Норматив компонента орентировка.md">Норматив компонента орентировка</a>
- <a target="_blank" href="/Компоненты ядра/3.Распределение/Нормативы/Компонентов/2.Норматив компонента условия.md">Норматив компонента условия</a>
- <a target="_blank" href="/Компоненты ядра/3.Распределение/Нормативы/Компонентов/3.Норматив компонента распределение.md">Норматив компонента распределение</a>
- <a target="_blank" href="/Компоненты ядра/3.Распределение/Нормативы/Компонентов/4.Норматив компонента движение.md">Норматив компонента движение</a>
- <a target="_blank" href="/Компоненты ядра/3.Распределение/Нормативы/Компонентов/5.Норматив компонента модули.md">Норматив компонента модули</a>


![hr](http://foto-video-montazh.ru/wa-data/public/site/img/0_b0251_20b04c67_orig-1.png)

### Интерфейс

В интерфейсе реализована структура landing-page + ajax подгрузка данных с ядра по api, что позволяет пользователю взаимодействовать с сайтом без прерываний, а разработчику интерфейса иметь исходники без каких либо php-вставок.

Стандарты: 

> Под стандартом понимается образец, эталон, модель.

- <a target="_blank" href="/Компоненты интерфейса/1.Ориентировка/Стандарты/Основополагающие/1.Основополагающий стандарт среды.md">Стандарт среды</a>
- <a target="_blank" href="/Компоненты интерфейса/1.Ориентировка/Стандарты/Основополагающие/2.Основополагающий стандарт кода.md">Стандарт кода</a>
- <a target="_blank" href="/Компоненты интерфейса/1.Ориентировка/Стандарты/Основополагающие/3.Основополагающий стандарт компонентов.md">Стандарт компонентов</a>
- <a target="_blank" href="/Компоненты интерфейса/1.Ориентировка/Стандарты/Основополагающие/4.Основополагающий стандарт разработки.md">Стандарт разработки</a>
- <a target="_blank" href="/Компоненты интерфейса/1.Ориентировка/Стандарты/Основополагающие/5.Основополагающий стандарт разработчиков.md">Стандарт разработчиков</a>


Структуры:

> Под структурами понимается внутреннии устройства с их взаимосвязями.

- <a target="_blank" href="/Компоненты интерфейса/2.Условия/Структуры/Напутствующие/Напутствующая структура разработки.md">Структура разработки</a>


Нормативы:

> Под нормативом понимается объем деятельности, которому всегда принято следовать.

- <a target="_blank" href="/Компоненты интерфейса/3.Распределение/Нормативы/Компонентные/1.Норматив компонента орентировка.md">Норматив компонента орентировка</a>
- <a target="_blank" href="/Компоненты интерфейса/3.Распределение/Нормативы/Компонентные/2.Норматив компонента условия.md">Норматив компонента условия</a>
- <a target="_blank" href="/Компоненты интерфейса/3.Распределение/Нормативы/Компонентные/3.Норматив компонента распределение.md">Норматив компонента распределение</a>
- <a target="_blank" href="/Компоненты интерфейса/3.Распределение/Нормативы/Компонентные/4.Норматив компонента движение.md">Норматив компонента движение</a>
- <a target="_blank" href="/Компоненты интерфейса/3.Распределение/Нормативы/Компонентные/5.Норматив компонента модули.md">Норматив компонента модули</a>



![hr](http://foto-video-montazh.ru/wa-data/public/site/img/0_b0251_20b04c67_orig-1.png)

### Разработка

Порядок разработки выстроен так, что равномерно переводит команду разработчиков на форму управления "холакратия", которая эффективна в непрерывной и распределительной разработке web-сайтов. При этом изучать холакратию не нужно, достаточно каждому участнику разработки соотвествовать нормативам.

> Холакратия — это способ децентрализации власти, который позволяет выстроить иерархию (холархию) таким образом, чтобы каждый сотрудник мог влиять на жизнь компании и обладал полной властью в рамках своей роли и возложенных на неё обязательств.


![Холакратия](/Компоненты%20интерфейса/2.Условия/Структуры/Картиночные/illustrators/4values.jpg)

### Примечание

Исходный код сайта https://framework-life-balance.ru подгружается с https://github.com/veter-love/framework-life-balance-v1 репозитория.