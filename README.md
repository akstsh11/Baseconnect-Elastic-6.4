# Baseconnect-Elastic-6.4

## 起動方法
```
## 以下のコマンドを実行する前にdockerの環境構築・起動をしておく
##　git clone する
$ git clone git@github.com:akstsh11/Baseconnect-Elastic-6.4.git
$ cd Baseconnect-Elastic-6.4

## Dockerイメージをビルドする
$ docker-compose build

## コンテナ起動
$ docker-compose up
```

## Elasticsearchに接続
``` http://localhost:9200 ```にアクセスし、以下のようなjsonデータが表示されたらok

```
{
  "name" : "7VpN1HU",
  "cluster_name" : "docker-cluster",
  "cluster_uuid" : "N9I4RKwyQT2boP5fMb8aPA",
  "version" : {
    "number" : "6.4.3",
    "build_flavor" : "default",
    "build_type" : "tar",
    "build_hash" : "fe40335",
    "build_date" : "2018-10-30T23:17:19.084789Z",
    "build_snapshot" : false,
    "lucene_version" : "7.4.0",
    "minimum_wire_compatibility_version" : "5.6.0",
    "minimum_index_compatibility_version" : "5.0.0"
  },
  "tagline" : "You Know, for Search"
}
```

## Kibanaに接続
``` http://localhost:5601 ```にアクセスする
