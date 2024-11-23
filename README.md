## 今日のゴール
- Laravelの概要を知る
- Hello Worldする
## Laravelとは
- PHPで一番使われてる**フレームワーク** 
- フルスタック　画面もAPIも
## とりあえずプロジェクトを作ってみる
### Dockerある場合（Mac）
- Docker Desktop起動
  ```bashocdmt041@

  curl -s "https://laravel.build/tutorial-app" | bash
  ```

- コンテナ起動
  ```bash
  cd tutorial-app
  ./vendor/bin/sail up
  ```
- これで起動⚪︎
- `localhost`にアクセス
- port被ったらdocker-compose.yamlのポートかえる
  - 
  - `3310:3306`

```テーブルのマイグレーション
sail php artisan migrate
```

###  Dockerない場合
- Laravel installerのインストール
https://readouble.com/laravel/11.x/ja/installation.html

```bash
# Windows PowerShell
# 管理者として実行する
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://php.new/install/windows'))
```
```
composer global require laravel/installer
```

```
laravel new tutorial-app
```
```
cd example-app
npm install && npm run build
composer run dev
```
