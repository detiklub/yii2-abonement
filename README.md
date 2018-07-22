Расширение для yii2
===================
Описание расширения abonement

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist detiklub/yii2-abonement "*"
```

or add

```
"detiklub/yii2-abonement": "*"
```

to the require section of your `composer.json` file.


	Регистрируем компонент в файле config/main.php

'components' => [
	'message' => [
           'class' => 'frontend\components\AbonementComponent',
	],
],

	Вызов компонента
	Вставляем следующую строку:

<? Yii::$app->message->display('Печатаем Abonement - компонент Yii2'); ?>

	На сайте отобразится 'Печатаем Abonement'. Если убираем параметр 'Печатаем Abonement' и не передаем ни какого значения в компонент, то выведется строка 'Текст по умолчанию'
	
Usage
-----

Once the extension is installed, simply use it in your code by  :

```php
<?= \detiklub\abonement\AbonementComponent::widget(); ?>```
