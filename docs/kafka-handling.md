## Restarting....
  - https://github.com/gopher-goodies/robustly
  - https://github.com/taskcluster/httpbackoff

  - https://github.com/aerth/diamond (Dynamic Runlevels for Applications)



## Stream SQL
  - https://github.com/StabbyCutyou/sqltocsv


###
  - https://github.com/uber/tchannel-go/ (Go implementation of a multiplexing and framing protocol for RPC calls )

### Data Collector
  -  https://github.com/jedisct1/flowgger (RUST, compiles to a single binary)


### Data Stream Processing API for GO
  - https://github.com/drborges/rivers
  - http://drborges.github.io/rivers
  Lightweight stream processing engine for IoT
  - https://github.com/sensorbee/sensorbee
  - http://docs.sensorbee.io/en/latest/bql.html



### Http Polling
  - https://github.com/k0kubun/github-stream (GitHub API v3 has Events API. This library polls the API and queues distinct events to its channel.)
  - https://github.com/miku/esbulk (Bulk import)


### A Kafka consumer coordination library for Go.
    - https://github.com/zorkian/marshal

### Good example:
  - http://joaodlf.com/data-pipelines-cassandra-kafka-and-python-and-go.html
  + limit concurrency: http://jmoiron.net/blog/limiting-concurrency-in-go/
  - https://blog.getstream.io/building-a-performant-api-using-go-and-cassandra/ - Casandra + Golang

### Kafka / Kinesis:

Clients:
  - https://github.com/confluentinc/confluent-kafka-go
  - https://github.com/optiopay/kafka (from OptioPay!)


Gateways:
  - https://github.com/moul/kafka-gateway (Kafka Gateway (gRPC+http) micro-service)
  - https://github.com/funkygao/gafka (A full ecosystem that is built around kafka powered by golang)


Tools:
  - https://github.com/edenhill/kafkacat
  - https://github.com/serejja/kafka-offset-mgr
  - https://github.com/TwitchScience/kinsumer
  - https://github.com/vrischmann/koff (koff is a small tool to get information about Kafka offsets.)
  - https://github.com/fgeller/kt (Kafka command line tool)
  - https://github.com/truppert/pegasus (Pegasus is a library that allows very simple consuming of a kafka topic)
  - https://github.com/CAFxX/kafkabalancer (Automatically rebalance your kafka topics, partitions, replicas across your cluster)
  - https://github.com/sclasen/event-shuttle (Unix system service that collects events and reliably delivers them to kafka, relieving other services on the same system from having to do so.)
  - https://github.com/sclasen/streambolt (snapshot kinesis stream shards into boltdb files that are stored in s3, bootstrap your kinesis consumer from those boltdb files stored in s3.)



