1. docker image build -t mykeycloak .
2. docker container run -e KEYCLOAK_USER=admin -e KEYCLOAK_PASSWORD=admin -e KEYCLOAK_IMPORT=/tmp/realm-export.json --publish 8080:8080 --name mykeycloak --net mynet mykeycloak
