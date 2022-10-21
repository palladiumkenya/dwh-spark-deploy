# dwh-spark-deploy
This repository is a deployment guide for running a spark cluster.
In the `local` folder, you'll find a docker compose file with service configurations
for a spark master and two work nodes.

## Requirements
- Docker Compose

## Running the cluster
1. Navigate to the `/local` folder
2. Configure any relevant environment variables in the ``.env`` file.
   Take note of the `SPARK_MASTER_URL`. If you're running the containers locally,
   this should be your host local IP
```bash
cd local
docker-compose up 
```
3. Check the spark master UI (port 8085) in out case. You should be able to see the 
  worker nodes listed.