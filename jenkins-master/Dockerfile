FROM jenkins:2.19.4
MAINTAINER jr00n
USER root

USER jenkins
ENV JAVA_OPTS="-Xmx8192m -Djenkins.install.runSetupWizard=false"


#Add reference config to disable security
COPY JENKINS_HOME /usr/share/jenkins/ref

#Add plugins
RUN /usr/local/bin/install-plugins.sh swarm:2.2 greenballs:1.15
