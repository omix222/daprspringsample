# Dapr でSpringBootアプリをビルドするサンプル

## 手順
- pack build myapp --builder cnbs/sample-builder:bionic
  - myappの部分がイメージ名になる
  - Dockerイメージ作成とローカルへの登録までをDockerfile無しでやれることが特徴
- docker run --rm -p 8080:8080 myapp
  - このコマンドで動作確認可能