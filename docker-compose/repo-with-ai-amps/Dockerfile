ARG TAG=PLEASE_PROVIDE
FROM quay.io/alfresco/alfresco-content-repository:$TAG

ARG TOMCAT_DIR=/usr/local/tomcat

USER root

COPY alfresco-ai-repo-1.4.0.amp $TOMCAT_DIR/amps/
RUN java -jar $TOMCAT_DIR/alfresco-mmt/alfresco-mmt*.jar install $TOMCAT_DIR/amps $TOMCAT_DIR/webapps/alfresco -directory -nobackup