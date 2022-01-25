ARG TAG=PLEASE_PROVIDE
FROM quay.io/alfresco/alfresco-share:$TAG

ARG TOMCAT_DIR=/usr/local/tomcat

COPY alfresco-ai-share-1.4.0.amp $TOMCAT_DIR/amps_share/
RUN java -jar $TOMCAT_DIR/alfresco-mmt/alfresco-mmt*.jar install $TOMCAT_DIR/amps_share $TOMCAT_DIR/webapps/share -directory -nobackup