# docker-laravel9-format
Laravel9が動くdockerのフォーマット環境（m1 mac）

## 操作手順
Docekrをインストール・Dockerを起動させる
イメージを元にコンテナを作成
`$ docker-compose up -d`

コンテナが立ち上がっているか確認
`$ docker-compose ps`

上記でDockerが立ち上がる

Laravelに対してマイグレーションやインストールする場合appコンテナに入る
`$ docker-compose exec app bash`

Dockerを停止する
`$ docker compose down`

WEB：http://localhost:81/
phpmyadmin：http://localhost:8080/

## 構成
基本のLAMP環境になります。
Apache
php 8.1
mysql 8.0.30
phpmyadmin 5.2.0
Laravel 9

## Laravelの構成
初期インストールしているもの
barryvdh/laravel-debugbar：https://github.com/barryvdh/laravel-debugbar
doctrine/dbal：https://github.com/doctrine/dbal
briannesbitt/Carbon：https://github.com/briannesbitt/Carbon
Laravel Lang：https://laravel-lang.com/installation/

### npmでのインストールなどがうまくいかない場合
`$ apt update`
`$ apt install nodejs npm`
でパッケージを更新