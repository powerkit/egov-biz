FROM tomcat:8-jre8
ENV TZ=Asia/Seoul
WORKDIR /usr/local/tomcat
RUN rm -rf ./webapps/*
COPY ./target/*.war ./webapps/ROOT.war
EXPOSE 8080
CMD $CATALINA_HOME/bin/startup.sh && tail -f $CATALINA_HOME/logs/catalina.out