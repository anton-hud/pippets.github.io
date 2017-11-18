# Перед началом верстки
1. Стили для повторяющихся частей макета
2. Bootstrap, material designe
3. Css препроцессор (например sass)
4. В body установить шрифт и размер и line-height
5. В sass задать переменные цвета
6. Определить размеры заголовков h1-h6
7. Использовать font-awesome

# Дополнительные св-ва:
```xsl
<xsl:value-of select="property_value[tag_name='email']/value"/>
<a href="{dir}{property_value[tag_name='file']/file}" target="_blank">Скачать <xsl:value-of select="property_value[tag_name='file']/file_name"/></a>
<a href="{dir}{property_value[tag_name='file']/file}" target="_blank"><img src="{dir}{property_value[tag_name='file']/file_small}" /></a>
```
# Для автоматических метатегов:
```html
<meta charset="<?php echo SITE_CODING?>">
<title><?php Core_Page::instance()->showTitle()?></title>
<meta name="description" content="<?php Core_Page::instance()->showDescription()?>">
<meta name="keywords" content="<?php Core_Page::instance()->showKeywords()?>">
<meta name="author" content="Ваше имя">
```
# Вставить виджет
```php
<? php $this->showSection('ИМЯ_ВИДЖЕТА'); ?>
```
# Вывод Title
```php
<?php Core_Page::instance()->showTitle()?>
```
# Вывод названия страницы
```php
<?php 
$oBook = Core_Entity::factory('Structure', 88);
echo "<p>" . $oBook->name . "</p>";
?>
```
# Вывод документа
```php
	<?php
Core_Entity::factory('Document', 10)->execute();
Core_Page::instance()->execute();
?>
```
# Ссылки
[вывод в php объектов](http://www.hostcms.ru/documentation/modules/core/orm/)
