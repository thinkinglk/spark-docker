# spark-docker

Run spark standalone cluster in docker compose:

```bash
docker-compose build # build image
docker-compose up # start cluster (master + 1 worker)
docker-compose scale worker=3 # Optionally, you can scale the cluster to up to N workers
```

Once the cluster is up and running, you can connect to it from the driver machine:

```bash
spark-shell --master spark://localhost:7077
```
