
## Keycloak Server

docker-compose file with the intention to make it easy to start up a keycloak server.

Things to be aware of:

- Create a **"C:\keycloak_themes"** folder on your Windows OS to bind it with the **/opt/keycloak/themes** directory inside the container, as configured on the volumes section, **OR** change the names accordingly to your scenario;
- Change KEYCLOAK_ADMIN and KEYCLOAK_ADMIN_PASSWORD from 'admin' to any other values if you wish so. These credentials will be used to access the **Administration Console** on the keycloak web ui;
- Start up with build by running the command **docker-compose up --build -d** in the same directory of the docker-compose.yml file.