# MySQLコンテナ

## 使用方法
1. docker-compose.ymlファイルのディレクトリに移動する
2. イメージのビルド
   ```
   docker-compose build
   ```
3. コンテナの作成
   ```
   docker-compose up -d
   ```
4. MySQLにログイン
   ```
   mysql -u root -p -h 127.0.0.1
   ```
5. コンテナの停止
   ```
   docker-compose stop
   ```
6. イメージ、コンテナ、ボリューム、ネットワークを削除
   ```
   docker-compose down
   ```

## その他コマンド
- 起動したコンテナにログイン
  ```
  docker exec -it Docker-mysql_mysql_1 bash -p
  ```
- docker-composeにて作成されたコンテナの状態確認
  ```
  docker-compose ps
  ```

## 参考資料
- [DockerでMySQLを使ってみる](https://qiita.com/TAMIYAN/items/ed9ec892d91e5af962c6)