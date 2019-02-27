# Art WooCommerce Order One Click

Плагин под WooCommerce.  Включает три режима: каталог, заказать, предзаказ

Прагин работает только с плагином Contact Form 7

[Полное описание](https://wpruse.ru/my-plugins/order-one-click/)

[Скачать плагин](https://github.com/artikus11/art-woo-order-one-click/releases)

[Плагин в репозитории WordPress](https://wordpress.org/plugins/art-woocommerce-order-one-click/)

## Changelog

###= 2.1.0 =
* Добавлено - опция отключения показа количества в окне
* Исправлено - создание заказов с любой формы на странице
* Исправлено - поведение окна на мобильных
* Исправлено - поведение окна при отключении все элементов, форма растягивается на всю ширину
* Изменено - при отключении всех элементов, все нужные данные отправляются в письмо

### = 2.0.0 =
* Добавлено - локализация, теперь можно переводить на разные языки
* Добавлено - проверка на наличие/отсутсвие ID товара при открытие окна
* Добавлено - появление кнопки заказать, если в вариативных товарах нет цены
* Исправлено - ошибка работы окна на простых товарах
* Исправлено - предупреждения и ошибки
* Исправлено - форма вставки поля в CF7
* Исправлено - ошибка вывода кнопки Купить если нет цены на простых товарах
* Исправлено - работа кнопки в Быстром просмотре
* Изменено - проведена проверка и рефакторинг кода
* Изменено - изменена система проверки на обязательные плагины
* Удалено - фильтр `awooc_html_add_to_cart`

### = 1.8.10 =
* Исправлено - скрытие окна на всехх страницах сайта
* Исправлено - очистка данных при выводе окна
* Изменено - обновление readme

### = 1.8.9 =
* Исправлено - ошибка определения типа продукта
* Изменено - обновление readme
   
### = 1.8.8 =
* Исправлено - обзод блокировки скрипта при работе плагина Popup Maker
* Изменено - обновление readme для добавления в репозиторий WP

### = 1.8.7 =
* Исправлено - скрипт вызова окна

### = 1.8.6 =
* Исправлено - ошибка отправки формы, если на странице есть еще формы
* Изменено - внешний вид вывода атрибутов
* Добавлено - ограничение загрузки скриптов и стилей плагина только на страницах WooCommerce
* Добавлено - работа сплывающего окна в режиме Быстрого просмотра

### = 1.8.5 =
* Исправлено - ошибка REST API при подключении плагина
* Изменено - сброс настроек при деактивации плагина на сброс при деинсталяции плагина
* Добавлено - проверка на выбор атрибутов в вариативных товарах, аналокично штатной кнопке, если атрибуты не выбраны то кнопка не работает

### = 1.8.4 =
* Исправлено - вывод в заголовке хмтл-сущьностей
* Добавлено - поддержка плагина Contact Form 7 – Phone mask field
* Добавлено - комментарии в js файле

### = 1.8.3 =
* Добавлено - скрытие +/- для поля количество в режиме каталога и предзаказа

### = 1.8.2 =
* Исправлено - заказы созаются со статусом "Ожидание заказа"
* Исправлено - вывод картинки для вариаций, если картинки нет, то выводится родительская
* Удалено - настройка отключения отправки писем клиенту при создании заказа

### = 1.8.1 =
* Исправлено получение данных с хтмл тегами. Теперь приходят только чистые данные
* Исправлен вывод формы во всплывающем окне, если отключен вывод данных
* Изменено включение всплывающего окна. Теперь окно загружается сразу с данными
* Добавлена загрузка формы во всплывающем окне через ajax

### = 1.8.0 =
* Переписан код
* Исправлена ошибка видимости окна в подвале
* Исправлено отправка писем при создании заказа
* Добавлена поддержка WPCS
* Добавлено отключение отправки писем пользователю при создании заказа
* Добавлено передача количества в заказ
* Добавлен хук `awooc_before_button` для добавления чего-нибудь перед кнопкой
* Добавлен хук `awooc_after_button` для добавления чего-нибудь после кнопки
* Добавлен хук `awooc_attributes_button` для добавления аттрибутов внутри кнопки
* Добавлен хук `awooc_after_mail_send` для ловли отправки письма и создания заказа
* Удален хук `awooc_popup_before_image`
* Удален хук `awooc_popup_after_image`


### = 1.7.0 =
* Добавлен фильтр `awooc_popup_attr_label` для возможности изменения надписи перед атрибутами в окне
* Добавлена вывод и отправка выбранного количества товаров
* Удалены хуки `awooc_popup_title_html_tag_open`, `awooc_popup_title_html_tag_close`
* Удалены хуки `awooc_popup_image_width`, `awooc_popup_image_heigh`
* Удалены хуки `awooc_popup_before_price`, `awooc_popup_after_price`
* Удалены хуки `awooc_popup_before_sku`, `awooc_popup_after_sku`
* Удалены хуки `awooc_popup_before_attr`, `awooc_popup_after_attr`
* Исправлены ошибки

### = 1.6.9 =
* Переименнованы файлы
* Добавлена function_exists для возможности изменения функций
* Переписан функционал вывода всплывающего окна
* переписано получение данных в модальном окне
* Добавлено отправка ссылки на выбранный товар в письме
* Добавлен фильтр `awooc_html_add_to_cart` для возможности изменения хтмл кнопки
* Добавлен фильтр `awooc_classes_button` для возможности добавления классов к кнопке
* Добавлен фильтр `awooc_popup_title_html` для возможности изменения стилей заголовка модального окна
* Добавлен фильтр `awooc_popup_title_html_tag_open` для изменения открывающего тега заголовка модального окна
* Добавлен фильтр `awooc_popup_title_html_tag_close` для изменения закрывающего тега заголовка модального окна
* Добавлен фильтр `awooc_popup_title_html_classes` для добавления классов к заголовку модального окна
* Добавлен фильтр `awooc_popup_image_html``` для возможности изменения хтмл изображения в окне
* Добавлен фильтр `awooc_popup_image_alt` для добавления alt к изображению в окне
* Добавлен фильтр `awooc_popup_image_classes` для добавления классов к изображению в окне
* Добавлен фильтр `awooc_popup_image_width` для изменения ширины изображения в окне
* Добавлен фильтр `awooc_popup_image_heigh` для изменения высоты изображения в окне
* Добавлен хук `awooc_popup_before_image` для добавления чего-нибудь перед изображением в окне
* Добавлен хук `awooc_popup_after_image` для добавления чего-нибудь после изображением в окне
* Добавлен фильтр `awooc_popup_price_html` для возможности изменения хтмл цены в окне
* Добавлен фильтр `awooc_popup_price_label` для возможности изменения надписи перед ценой в окне
* Добавлен хук `awooc_popup_before_price``` для добавления чего-нибудь перед ценой в окне
* Добавлен хук `awooc_popup_after_price` для добавления чего-нибудь после ценой в окне
* Добавлен фильтр `awooc_popup_sku_html` для возможности изменения хтмл артикула в окне
* Добавлен фильтр `awooc_popup_sku_label` для возможности изменения надписи перед артикулом в окне
* Добавлен хук `awooc_popup_before_sku` для добавления чего-нибудь перед арикулом в окне
* Добавлен хук `awooc_popup_after_sku` для добавления чего-нибудь после артикула в окне
* Добавлен хук `awooc_popup_before_attr` для добавления чего-нибудь перед атрибутами в окне
* Добавлен хук `awooc_popup_after_attr` для добавления чего-нибудь после атрибутов в окне
* Добавлен хук `awooc_popup_before_form` для добавления чего-нибудь перед формой в окне
* Добавлен хук `awooc_popup_after_form` для добавления чего-нибудь после формой в окне
* Добавлен хук `awooc_popup_before_column`
* Добавлен хук `awooc_popup_column_left`
* Добавлен хук `awooc_popup_column_right`
* Добавлен хук `awooc_popup_after_column`
* Добавлены стили тени и овефлоу к сплывающему окну
* Изменено поведение окна при ошибке ввода полей формы
* При закрытии окна удаляется хеш из урла


### = 1.6.8 =
* Добавлен фильтр `awooc_enable_add_to_card_style` для возможности изменения стилей
* Добавлен фильтр ```awooc_disable_add_to_card_style``` для возможности изменения стилей
* Исправлены скрытия кнопки Купить в первом режиме
* Обновлен код

### = 1.6.7 =
* Добавлен фильтр ```awooc_classes_button``` для добавления классов к кнопке
* Добавлен фильтр ```awooc_thumbnail_name``` для названия миниатюры во всплывающем окне
* Переименованы файлы, для исключения конфликтов
* Исправлены стили

### = 1.6.6 =
* Добавлена проверка на версию php
* Добавлена ссылка на настройки в списке плагинов
* Добавлена ссылка на статью в описании плагина
* Изменен второй режим работы, теперь кнопка Купить работает в штатном режиме
* Исправлены ошибки стилей

### = 1.6.5 =
* Добавлено определение распродажной цены
* Исправлены ошибки стилей

### = 1.6.4 =
* Добавлена отправка цены товара в скрытом поле
* Добавлены описания строк в скрытом поле для отправки в письме
* Изменено скрытие цены
* Исправлены ошибки

### = 1.6.3 =
* Исправлены ошибки

### = 1.6.2 =
* Добавлено появление кнопки Заказать, если нет цены у товара, в режиме управления запасами
* Исправлена логика появления кнопки Заказать при управлении запасами
* Исправлены ошибки

### = 1.6.1 =
* Исправлена ошибка использования отмененной функции

### = 1.6.0 =
* Добавлена адаптивность окна
* Добавлена кнопка закрытия окна
* Добавлено отключение кнопки Купить в Похожих и Апселлах
* Добавлен функционал создания заказов
* Добавлена настройка включения/выключения созданием заказов
* Добавлены комментарии к коду
* Изменены настройки режимов работы, теперь три режима
* Изменены настройки по умолчанию при выводе элементов окна
* Исправлено скрытие кнопки Купить
* Исправлены ошибки

### = 1.5.3 =
* Исправлены ошибки

### = 1.5.2 =
* Исправлены ошибки
* Добавлено удаление опций при деинсталяции

### = 1.5.1 =
* Исправлены ошибки

### = 1.5.0 =
* Добавлена настройка управления режимом каталога
* Добавлена настройка управления отображением элементов в попап окне
* Добавлена настрока управления надписью на кнопке
* Добавлена отправка артикула
* Исправлены ошибки

### = 1.4.0 =
* Добавлена кнопка при редактировании формы Contact Form 7
* Добавлены настройки для управления формами
* Обновлены проверки на наличие плагинов
* Исправление ошибок

### = 1.3.0 =
* Обновление настроек
* Исправление ошибок

### = 1.2.0 =
* Обновление настроек

### = 1.1.0 =
* Обновление функций
* Добавление проверок
* Добавление настроек

### = 1.0.0 =
* Релиз
