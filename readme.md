# DockerによるWordpress構築について

データを保存するデータ専用コンテナを作成する。Dockerfileに記述されているので、buildを行う。

```
docker build -t dataonly .
```

データ専用コンテナの起動

```
docker run -it --name dataonly dataonly
```

コンテナ群のバックグラウンド起動

```
docker-compose up -d
```

