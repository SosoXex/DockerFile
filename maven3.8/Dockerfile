FROM    ubuntu:20.04
RUN apt update -y
RUN apt install -y default-jdk
RUN apt install -y maven
RUN apt-get install -y git
RUN git clone https://github.com/koddas/war-web-project.git
WORKDIR war-web-project
RUN mvn package
RUN pwd
WORKDIR ../build
RUN cp ./war-web-project/target/wwp-1.0.0.war ./ /tmp
RUN pwd
