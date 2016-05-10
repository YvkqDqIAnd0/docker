FROM jenkins:1.651.1
MAINTAINER DaiAndo

USER root
RUN mkdir /var/log/jenkins
RUN mkdir /var/cache/jenkins
RUN chown -R  jenkins:jenkins /var/log/jenkins
RUN chown -R  jenkins:jenkins /var/cache/jenkins
USER jenkins

ENV JAVA_OPTS="-Xms768m -Xmx1G -XX:MaxMetaspaceSize=128m"
ENV JENKINS_OPTS="--logfile=/var/log/jenkins/jenkins.log --webroot=/var/cache/jenkins/war"

