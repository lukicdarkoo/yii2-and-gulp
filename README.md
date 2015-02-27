# Yii2 and Gulp
Simple app with working Yii2 asset command and Gulp.

This is configured [yiisoft/yii2-app-basic](https://github.com/yiisoft/yii2-app-basic) which works with Gulp. 

## App installation

* Install NodeJS from [here](http://nodejs.org/)
* Install Gulp globaly ``npm install -g gulp``. 
  * IMPORTANT: Make sure does Gulp work fine. Check it with ``gulp --version``, if it works you should see something like ``CLI version 3.8.11``
* Clone this repository
  ``git clone https://github.com/lukicdarkoo/yii2-and-gulp.git``
  * Navigate to ``/yii2-and-gulp`` and run ``composer update --prefer-dist``
  * Navigate to ``/yii2-and-gulp/tools/gulp`` and run ``npm update``
* To generate combined and compressed *.js and *.css files navigate to ``/yii2-and-gulp`` and run ``yii asset tools/gulp/assets-config.php config/assets-prod.php``
* FINISH! Run app and check source code, you should see only one *.js and one *.css file, combined and compressed.


## Integrate to your app

* Copy directory ``/tools`` to your application
* Change **bundles** and **targets** for your needs in ``/tools/grunt/assets-config.php``, check Yii2 Guide [Using the asset Command](http://www.yiiframework.com/doc-2.0/guide-structure-assets.html#using-the-asset-command)
* Configure component to your config file: 
```
'assetManager' => [
	'bundles' => require(__DIR__ . '/' . 'assets-prod.php' ),  
],
```
* Install NodeJS from [here](http://nodejs.org/)
* Install Gulp globaly ``npm install -g gulp``. 
  * IMPORTANT: Make sure does Gulp work fine. Check it with ``gulp --version``, if it works you should see something like ``CLI version 3.8.11``
* Navigate to ``/your-app-root/tools/gulp`` and run ``npm update``
* To generate combined and compressed *.js and *.css files navigate to ``/your-app-root`` and run ``yii asset tools/gulp/assets-config.php config/assets-prod.php``
* FINISH! Run app and check source code, you should see only one *.js and one *.css file, combined and compressed.
