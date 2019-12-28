1. docker image build -t mykeycloak .
2. docker container run -e KEYCLOAK_USER=admin -e KEYCLOAK_PASSWORD=admin -e KEYCLOAK_IMPORT=/tmp/realm-export.json --publish 8080:8080 --name mykeycloak --net mynet mykeycloak

3. login http://localhost:8080/auth/admin/master/console/#/realms/mvp/identity-provider-settings
4. update github secret key to 331c33b15ecc6ea549a93bd6e8c60db6fd6a5788, save.
