# rails_docker

## 資料

https://github.com/ValLaboratory/rookie-training/blob/master/virtualization/README.md

## コマンド

1. イメージの作成 ( Dockerfile を元にイメージを作成 )
    - $ docker-compose build
1. コンテナの起動 ( docker-compose.yml の設定を元にコンテナを起動する )
    - $ docker-compose up --detach
1. コンテナへ接続 （ 対象のコンテナに対して`bash`を実行する ）（ exitで接続解除 ）
    - $ # execの後はdocker-compose.ymlでのserviceネームを指定する
    - $ docker-compose exec rails_web bash
1. コンテナの削除
    - $ docker-compose down

### 他に使えそうなコマンド

- $ docker-compose ps
  - 立ち上がってるContainer（service）を確認できる
