ARG HADOOP_VERSION=2.8.4
ARG HIVE_VERSION=2.3.3
ARG SPARK_VERSION=2.4.3
FROM abhioncbr/daflow-spark-base:${SPARK_VERSION}

COPY master.sh /opt/spark

ENV SPARK_MASTER_PORT 7077
ENV SPARK_MASTER_WEBUI_PORT 8080
ENV SPARK_MASTER_LOG /opt/spark/logs

EXPOSE 8080 7077 6066

CMD ["/bin/bash", "/opt/spark/master.sh"]
