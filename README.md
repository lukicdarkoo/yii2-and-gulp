# Yii2 and Gulp
Simple app with working Yii2 asset command and Gulp.

## App installation

* Install NodeJS from [!here](http://nodejs.org/)
* Install Gulp globaly ``npm install -g gulp``. 
  * IMPORTANT: Make sure does Gulp work fine. Check it with ``gulp --version``, if it works you should see something like ``CLI version 3.8.11``
* Clone this repository
  ``git clone https://github.com/lukicdarkoo/yii2-and-gulp.git``
  * Navigate to ``/yii2-and-gulp`` and run ``composer update --prefer dist``
  * Navigate to ``/yii2-and-gulp/tools/gulp`` and run ``npm update``
* To generate combined and compressed *.js and *.css files navigate to ``/yii2-and-gulp`` and run ``yii asset tools/gulp/assets-config.php config/assets-prod.php``
* FINISH! Run app and check source code, you should see only one *.js and one *.css file, combined and compressed.
