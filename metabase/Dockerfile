FROM eclipse-temurin:19-jdk

ENV MB_PLUGINS_DIR=/home/plugins/

COPY metabase.jar /home/metabase.jar
COPY duckdb.metabase-driver.jar /home/plugins/duckdb.metabase-driver.jar

RUN chmod 744 /home/plugins/duckdb.metabase-driver.jar

CMD ["java", "-jar", "/home/metabase.jar"]