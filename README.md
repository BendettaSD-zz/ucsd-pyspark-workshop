## PySpark Workshop

### Directions to start:

It is easiest to get a standalone cluster for Spark running with Docker. We will be using Spark 2.0.x and jupyter for this example.

- Install [Docker](https://docs.docker.com/)
- Find a Spark 2.0.x docker image to pull (or build one yourself). I like the one found [here](https://hub.docker.com/r/produktion/jupyter-pyspark/) by Produktion
```
docker pull produktion/jupyter-pyspark:latest
```
- Clone this repo somewhere memorable
```
git clone https://github.com/BendettaSD/ucsd-pyspark-workshop.git /path/to/usce-pyspark-workshop
```
- Start your docker container
```
docker run -d -p 4040:4040 -p 7077:7077 -p 8080:8080 -p 6066:6066 -p 8888:8888 -v /path/to/ucsd-pyspark-workshop:/home/jovyan/work produktion/jupyter-pyspark:latest
```
- Go to [http://localhost:8888] to view you jupyter notebook server. You should see pyspark_introduction.ipynb in the list of available files
- Open [http://localhost:4040] for the Spark UI page. Nothing will be visible at the moment

Follow along!
