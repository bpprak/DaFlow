ARG HADOOP_VERSION=2.8.4
ARG HIVE_VERSION=2.3.3
ARG SPARK_VERSION=2.3.1
FROM abhioncbr/daflow-spark-base:${SPARK_VERSION}

COPY adhoc.sh /opt/spark

ENV SPARK_WORKER_WEBUI_PORT 8081
ENV SPARK_WORKER_LOG /spark/logs
ENV SPARK_MASTER "spark://spark-master:7077"

CMD ["/bin/bash", "/opt/spark/adhoc.sh"]