ARG BASE_IMAGE=inseefrlab/onyxia-vscode-python:py3.11.6
FROM $BASE_IMAGE

LABEL maintainer="odysseu <uboucherie1@gmail.com>"

# If not specified in ci, will install java-17
ARG JAVA_VERSION="17"
ENV JAVA_VERSION=${JAVA_VERSION}
ENV JAVA_HOME="/usr/lib/jvm/java-$JAVA_VERSION-openjdk-amd64"
ENV PATH="${JAVA_HOME}/bin:${PATH}"

USER root

RUN apt-get update && \
    # Install JDK
    /opt/install-java.sh && \
    apt-get install maven -y

RUN code-server --install-extension adamraichu.zip-viewer && \
    code-server --install-extension redhat.java && \
    code-server --install-extension vscjava.vscode-java-pack

USER 1000

CMD ["java --version"]