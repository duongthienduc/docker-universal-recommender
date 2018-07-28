# PredictionIO + Universal Recommender 
Docker container for PredictionIO 0.12.1 + Universal Recommender 0.7.3

This container uses Apache Spark, HBase and Elasticsearch.
The PredictionIO version is 0.12.1.

### How to Start
```bash
 docker pull nateetorn/predictionio-ur:0.1
 docker run -d -ti -p 8000:8000 nateetorn/predictionio-ur:0.1
```
Then in docker container, start all services and check they are started
```bash
 pio-start-all
 pio status
```

Test Universal Recommender are working 
```bash
 cd /universal-recommender-0.7.3
 ./example/integration-test
```

### Thanks

 * [docker-predictionio](https://github.com/shimamoto/docker-predictionio) Dockerfile for PIO
 * [docker-ur](https://github.com/zephrax/docker-prediction.io) Dockerfile for UR
