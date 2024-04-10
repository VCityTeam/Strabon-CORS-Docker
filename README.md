# Strabon-CORS-Docker
A CORS enabled RDF-Store for storing/serving spatio-temporal semantic graph data with a stSPARQL REST API.

## Links
- Original work : [Strabon](https://strabon.di.uoa.gr/)
- Sources : [bde2020/strabon](https://hub.docker.com/r/bde2020/strabon) on Docker hub
- Images published on [Docker hub](https://hub.docker.com/r/vcity/strabon-cors).

## Modifications from source:
**Dockerfile:**
- Configure Strabon credentials at build time with arguments
- Add new tomcat configuration file

**web.xml:**
- A simple CORS enabled tomcat configuration file 
