# docker-laravel9-format
Laravel9が動くdockerのフォーマット環境（m1 mac）

## 操作手順

### appコンテナに入る
### -itオプションをつけないと、コマンド入力しても反応してくれない
$ docker exec -it app bash

## 構成
基本のLAMP環境になります。
Apache
php 8.1
mysql 8.0.30
phpmyadmin 5.2.0

## Laravelの構成
初期インストール
barryvdh/laravel-debugbar：https://github.com/barryvdh/laravel-debugbar
doctrine/dbal：https://github.com/doctrine/dbal
briannesbitt/Carbon：https://github.com/briannesbitt/Carbon
