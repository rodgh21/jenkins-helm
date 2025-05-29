FROM jenkins/jenkins:jdk21
ENV PLUGINS_FORCE_UPGRADE=true \
  TRY_UPGRADE_IF_NO_MARKER=true
COPY resources/plugins.txt /usr/share/jenkins/ref/plugins.txt
RUN jenkins-plugin-cli --plugin-file /usr/share/jenkins/ref/plugins.txt --verbose
