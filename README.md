Yii2 Mailgun Mailer
===================
Mailgun mailer for Yii 2 framework.

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist ivan1911/yii2-mailgun-mailer "*"
```

or add

```
"ivan1911/yii2-mailgun-mailer": "*"
```

to the require section of your `composer.json` file.


Usage
-----

Once the extension is installed, simply use it in your code by  :

```php
<?php
Yii::$app->mailer->compose('<view_name>', <option>)
->setFrom("<from email>")
->setTo("<to email>")
->setSubject("<subject>")
->addTags(['<tag1>', '<tag2>'])
->addCampaignId('<compaignId>')
//->setHtmlBody("<b> Hello User </b>")
//->setTextBody("Hello User")
->send();
?>```
