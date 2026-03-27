FROM tomcat:9

ARG APP_VERSION
ARG GIT_SHA

LABEL app.name="DB-ConnectionTest"
LABEL app.version=$APP_VERSION
LABEL app.git_sha=$GIT_SHA

COPY target/app-${APP_VERSION}.war ./webapps/ROOT.war

EXPOSE 8080

CMD ["catalina.sh", "run"]

