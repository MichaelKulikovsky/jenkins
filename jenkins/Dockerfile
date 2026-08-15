FROM jenkins/jenkins:lts-jdk17

USER root 

RUN apt-get update && \
    atp-get install -y docker.io curl && \
    curl -fsSL http://deb.nodesource.com/setup_20.x | bash - && \
    apt-get install -y nodejs && \ 
    apt-get clean && rm -rf /var/lib/apt/lists/*

USER jenkins

