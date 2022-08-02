FROM    ubuntu:20.04
RUN apt update -y
RUN apt install -y default-jdk
RUN apt install -y maven
RUN apt-get install -y git
WORKDIR build
RUN git clone https://github.com/koddas/war-web-project.git
WORKDIR war-web-project
RUN mvn package


