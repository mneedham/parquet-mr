FROM openjdk:18.0.2.1-jdk

COPY target /target
RUN ls -la /target/

ENTRYPOINT [ "java", \
            "-classpath", \
            "/target/parquet-cli-1.13.0-SNAPSHOT.jar:/target/dependency/*", \
            "org.apache.parquet.cli.Main" \
]
