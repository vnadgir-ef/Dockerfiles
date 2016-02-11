FROM oberthur/docker-alpine-java

ENV M2_HOME=/usr/lib/mvn M2=/usr/lib/mvn/bin PATH=$PATH:/usr/lib/mvn:/usr/lib/mvn/bin

RUN apk add --update wget \
 && wget http://ftp.fau.de/apache/maven/maven-3/3.3.9/binaries/apache-maven-3.3.9-bin.tar.gz \
 && tar -zxvf apache-maven-3.3.9-bin.tar.gz \
 && rm apache-maven-3.3.9-bin.tar.gz \
 && mv apache-maven-3.3.9 /usr/lib/mvn \
 && apk del wget && rm /var/cache/apk/*

