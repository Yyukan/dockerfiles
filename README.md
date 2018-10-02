# dockerfiles

## Cassandra
Build 

```cd cassandra```
```docker build -t yukan/cassandra-lucene:3.11.3 .```

Run

```docker run --name cassandra-lucene -d -p 7199:7199 -p 7000:7000 -p 9042:9042 -p 9160:9160 -p 7001:7001 yukan/cassandra-lucene:3.11.3```

Connect

```docker run -it --link cassandra-lucene:cassandra --rm cassandra cqlsh cassandra```

