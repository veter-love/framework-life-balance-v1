# Framework life balance 

![ядро: v1.1.8.18](https://img.shields.io/badge/Ядро-v1.1.8.18-blue.svg) ![интерфейс: v1.0.7.20](https://img.shields.io/badge/Интерфейс-v1.0.7.20-blue.svg)

Framework life balance предназначен для **сопровождения** всех этапов разработки отеческого сайта с любым масштабом на исходном php-коде, html-разметках ( css, image ) и js-скриптах, с применением чёткой последовательностью разработки (смотрите <a target="_blank" href="/Компоненты ядра/2.Представление/Структуры/Напутствующие/Напутствующая структура разработки.md">структуру разработки ядра</a> и <a target="_blank" href="/Компоненты интерфейса/2.Представление/Структуры/Напутствующие/Напутствующая структура разработки.md">структуру разработки интерфейса</a>) 10 компонентов сайта:

| № | Компоненты ядра | Компоненты интерфейса
 ------------- |  ------------- | ------------- | 
| 1. | Ориентировка: цели, сведения, стандарты | Ориентировка: цели, сведения, стандарты
| 2. | Представление: структуры | Представление: структуры
| 3. | Аккумуляция: нормативы | Аккумуляция: нормативы
| 4. | Движение: протоколы, функции | Движение: протоколы, функции
| 5. | Модули | Модули

<a target="_blank" href="https://framework-life-balance.ru/#about">Подробнее о проекте</a> (в том числе про этапы развёртки).

![Framework life balance](http://agappi.info/wp/wp-content/uploads/2017/02/0_1368eb_82b1ef78_orig-1024x473.png)


### Среда

У Framework life balance две среды разработки: back-end (ядро) и front-end (интерфейс). 

![Framework life balance](https://framework-life-balance.ru/Компоненты%20интерфейса/2.Представление/Структуры/Картиночные/slider/slide1_bg.jpg)

Здесь нет места для php-кода в интерфейсе, и html-а в ядре. Ядро и интерфейс разделены и изолированы, что позволяет безпрепятственно разрабатывать оба направления одновременно, почтительно дополняя (без возникновения каких либо merge) на git'e.

![Framework life balance](http://arabesko.ru/images/files/vector/arabesq/arabesko.ru_06.png)


### Ядро

В ядре реализованы Стандарты (детализации) ядра, наглядность Структуры (планировка), Функции 4-х компонентов (распределенная альтернатива контролёров в mvc), Функции категорий сайта (упрощённая альтернатива моделей в mvc) и Нормативы (упрощённая альтернатива yii2 migrate, установки и настроек). Благодаря такому подходу был реализован норматив таблиц базы данных и функция автоматической реконструкции базы данных, что освободило разработчиков от необходимости конструировать sql-запросы вручную. А так же реализован внутренний самовызов из консоли, оттого на фоновый режим отработки была переведена отправка почтового сообщения и реструктуризация базы данных, что для пользователя значительно уменьшило время ожидания ответа, а у разработчиков отпала необходимость настраивать cron.

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

- <a target="_blank" href="/Компоненты ядра/2.Представление/Структуры/Напутствующие/Напутствующая структура разработки.md">Структура разработки</a>
- <a target="_blank" href="/Компоненты ядра/2.Представление/Структуры/Базы данных/Структура таблиц базы данных.md">Структура таблиц базы данных</a>
- <a target="_blank" href="/Компоненты ядра/2.Представление/Структуры/Базы данных/Структура взаимодействия с базой данных.md">Структура взаимодействия с базой данных</a>
- <a target="_blank" href="/Компоненты ядра/2.Представление/Структуры/Функций/Структура функций компонентов.md">Структура функций компонентов</a>
- <a target="_blank" href="/Компоненты ядра/2.Представление/Структуры/Функций/Структура функций сайта.md">Структура функций сайта</a>


Нормативы:

> Под нормативом понимается объем деятельности, которому всегда принято следовать.

- <a target="_blank" href="/Компоненты ядра/3.Аккумуляция/Нормативы/Компонентов/1.Норматив компонента орентировка.md">Норматив компонента орентировка</a>
- <a target="_blank" href="/Компоненты ядра/3.Аккумуляция/Нормативы/Компонентов/2.Норматив компонента представление.md">Норматив компонента представление</a>
- <a target="_blank" href="/Компоненты ядра/3.Аккумуляция/Нормативы/Компонентов/3.Норматив компонента аккумуляция.md">Норматив компонента аккумуляция</a>
- <a target="_blank" href="/Компоненты ядра/3.Аккумуляция/Нормативы/Компонентов/4.Норматив компонента движение.md">Норматив компонента движение</a>
- <a target="_blank" href="/Компоненты ядра/3.Аккумуляция/Нормативы/Компонентов/5.Норматив компонента модули.md">Норматив компонента модули</a>
- <a target="_blank" href="/Компоненты ядра/3.Аккумуляция/Нормативы/Функций/Норматив функций компонентов.md">Норматив функций компонентов</a>


![Framework life balance](http://www.coollady.ru/pic/0003/068/41.jpg)

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

- <a target="_blank" href="/Компоненты интерфейса/2.Представление/Структуры/Напутствующие/Напутствующая структура разработки.md">Структура разработки</a>


Нормативы:

> Под нормативом понимается объем деятельности, которому всегда принято следовать.

- <a target="_blank" href="/Компоненты интерфейса/3.Аккумуляция/Нормативы/Компонентов/1.Норматив компонента орентировка.md">Норматив компонента орентировка</a>
- <a target="_blank" href="/Компоненты интерфейса/3.Аккумуляция/Нормативы/Компонентов/2.Норматив компонента представление.md">Норматив компонента представление</a>
- <a target="_blank" href="/Компоненты интерфейса/3.Аккумуляция/Нормативы/Компонентов/3.Норматив компонента аккумуляция.md">Норматив компонента аккумуляция</a>
- <a target="_blank" href="/Компоненты интерфейса/3.Аккумуляция/Нормативы/Компонентов/4.Норматив компонента движение.md">Норматив компонента движение</a>
- <a target="_blank" href="/Компоненты интерфейса/3.Аккумуляция/Нормативы/Компонентов/5.Норматив компонента модули.md">Норматив компонента модули</a>



![Framework life balance](https://resnic.com.ua/wp-content/uploads/2012/01/ornament_studio_narashivaniya_resnic_3.jpg)

### Разработка

Порядок разработки выстроен так, что равномерно переводит команду разработчиков на форму управления "холакратия", которая эффективна в непрерывной и распределительной разработке web-сайтов. При этом изучать холакратию не нужно, достаточно каждому участнику разработки соотвествовать нормативам.

> Холакратия — это способ децентрализации власти, который позволяет выстроить иерархию (холархию) таким образом, чтобы каждый сотрудник мог влиять на жизнь компании и обладал полной властью в рамках своей роли и возложенных на неё обязательств.


![Framework life balance](https://framework-life-balance.ru/Компоненты%20интерфейса/2.Представление/Структуры/Картиночные/illustrators/4values.jpg)



![Framework life balance](https://avatars.mds.yandex.net/get-pdb/1054037/b6d1c164-b8ec-41a6-9fd6-f450a1b0e4ad/s1200?webp=false)

### Примечание

Исходный код сайта https://framework-life-balance.ru подгружается с https://github.com/veter-love/framework-life-balance-v1 репозитория.