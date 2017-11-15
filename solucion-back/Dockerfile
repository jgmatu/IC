FROM java:8 
EXPOSE 8080
VOLUME /tmp
ADD /target/solucion-back-0.0.1-SNAPSHOT.jar back.jar
#ENV JAVA_OPTS=""
RUN bash -c 'touch /back.jar'
ENTRYPOINT ["java","-Dspring.data.mongodb.uri=mongodb://mongolocal/products","-jar","/back.jar"]
