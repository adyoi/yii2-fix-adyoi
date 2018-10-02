# yii2-fix-adyoi
Yii2 Fix by adyoi

## Yii2 on PHP 7 ##
Rename File /vendor/yii2/base/Object.php change to /vendor/yii2/base/BaseObject.php

use find tool in whole directory '/vendor/' 
- use case sensitive search and rename 'Object' to 'BaseObject'
- except /vendor/yii2/assets/*.*
- except /vendor/yii2/views/errorHandler/exception.php

## Session.php ##
Filename : /vendor/yiisoft/yii2/web/Session.php

Version : **PHP 7**

Error Class : yii\debug\FlattenException

**Error Message** : **session_set_cookie_params(): Cannot change session cookie parameters when headers already sent**

**Fix** : https://github.com/adyoi/yii2-fix-adyoi/blob/master/Session.php
