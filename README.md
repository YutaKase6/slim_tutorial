# Slim Framework 3 Skeleton Application

Use this skeleton application to quickly setup and start working on a new Slim Framework 3 application. This application uses the latest Slim 3 with the PHP-View template renderer. It also uses the Monolog logger.

This skeleton application was built for Composer. This makes setting up a new Slim Framework application quick and easy.

## Install the Application

Run this command from the directory in which you want to install your new Slim Framework application.

    php composer.phar create-project slim/slim-skeleton [my-app-name]

Replace `[my-app-name]` with the desired directory name for your new application. You'll want to:

* Point your virtual host document root to your new application's `public/` directory.
* Ensure `logs/` is web writeable.

To run the application in development, you can also run this command. 

	php composer.phar start

Run this command to run the test suite

	php composer.phar test

That's it! Now go build something cool.
# Slim tutorial
[Slim](https://www.slimframework.com)
## composer
何はともあれcomposer  

インストーラダウンロードしてPHPで実行。  
```
$ curl -sS https://getcomposer.org/installer | php
```

パスが通っているであろうディレクトリへ  
```
$ mv composer.phar /usr/local/bin/composer
```

composerコマンドが動けばOK。

```
$ composer
   ______
  / ____/___  ____ ___  ____  ____  ________  _____
 / /   / __ \/ __ `__ \/ __ \/ __ \/ ___/ _ \/ ___/
/ /___/ /_/ / / / / / / /_/ / /_/ (__  )  __/ /
\____/\____/_/ /_/ /_/ .___/\____/____/\___/_/
                    /_/
Composer version 1.4.2 2017-05-17 08:17:52

...

```

## ~~PHPUnit~~
~~テストのためにPHPUnitをインストールする。~~  
~~テスト、すなわち開発環境のみに必要なモジュールなので--devオプションを付けておく。~~  

```
$ composer require --dev phpunit/phpunit
```

~~composer.jsonが更新されればOK。~~  

```json
{
    "require-dev": {
        "phpunit/phpunit": "^5.7"
    }
}
```

**SlimのSkeletonを利用することでPHPUnitとMonologは一緒に入る。**  

## vendor
composerによってインストールしたモジュールはすべてvendor以下に配置される。  
vendor以下のファイルはcomposerによって管理されているためわざわざgitで管理する必要はない。  
gitignore。  

## Slim
公式サイトより  
様々なファイルや

```
$ composer create-project slim/slim-skeleton slim_tutorial
```
