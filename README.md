# Advance Laravel開発環境

Docker + Laravelのローカル開発環境（教材使用）

## 起動手順
```
# 任意のディレクトリ名でクローン
git clone https://github.com/seki0603/advance-laravel.git 新しいディレクトリ（クローン先）

# ディレクトリに移動
cd 新しいディレクトリ

# .envファイルを作成
cp src/.env.example src/.env

# Dockerコンテナ起動
docker-compose up -d

# Laravel依存パッケージをインストール
docker-compose exec app composer install

# アプリケーションキーの生成
docker-compose exec app php artisan key:generate
```
