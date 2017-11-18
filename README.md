# Перед началом верстки
1. Стили для повторяющихся частей макета
2. Bootstrap, material designe
3. Css препроцессор (например sass)
4. В body установить шрифт и размер и line-height
5. В sass задать переменные цвета
6. Определить размеры заголовков h1-h6
7. Использовать font-awesome

# Дополнительные св-ва:


Для автоматических метатегов:
```
tmp = "Html"
<meta charset="<?php echo SITE_CODING?>">
<title><?php Core_Page::instance()->showTitle()?></title>
<meta name="description" content="<?php Core_Page::instance()->showDescription()?>">
<meta name="keywords" content="<?php Core_Page::instance()->showKeywords()?>">
<meta name="author" content="Ваше имя">
```
