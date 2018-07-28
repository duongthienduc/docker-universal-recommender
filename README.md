# PredictionIO + Universal Recommender 
Docker container for PredictionIO 0.12.1 + Universal Recommender 0.7.3

This container uses Apache Spark, HBase and Elasticsearch.
The PredictionIO version is 0.12.1.

### How to Start
```bash
 git clone https://github.com/nateetorn/docker-universal-recommender.git
 cd ./docker-universal-recommender
 docker build -t predictionio .
 docker run -p 8000:8000 --name predictionio_instance -it predictionio /bin/bash
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
 * [docker-ur](https://github.com/zephrax/docker-prediction.io-universal-recommender) Dockerfile for UR
