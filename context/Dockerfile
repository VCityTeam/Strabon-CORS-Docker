FROM bde2020/strabon

LABEL maintainer "VCityTeam"
LABEL source.repo "https://github.com/VCityTeam/Strabon-CORS-Docker/"

ARG STRABON_USERNAME=endpoint
ARG STRABON_PASSWORD

# Add connection/credential properties for Strabon if they exist
RUN if [ -n "$STRABON_USERNAME" && -n "$STRABON_PASSWORD" ] ; then \
        echo username=${STRABON_USERNAME} > /tomcat/webapps/strabon/WEB-INF/credentials.properties ;\
        echo password=${STRABON_PASSWORD} >> /tomcat/webapps/strabon/WEB-INF/credentials.properties ;\
    fi

# Enable CORS support for Tomcat 
COPY web.xml /tomcat/conf/web.xml
