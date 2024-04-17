# Projectopdracht


Welcome to the repository for the ongoing DevOps assignment.

Traefik is the reverse proxy that delegates traffic to various services.

TLS certificates are provided via CloudFlare as DNS challenges, after which each underlying service receives a self-signed certificate. Traefik is configured to route all traffic to the appropriate service based on the set route rules. It uses service labels to route requests correctly.

The self-signed certificates of each service are used for the secure connection between the client and the service. Despite being self-signed, the certificates are secure as they are used internally within the network and are not publicly available.

For an additional layer of security, all requests passing through Traefik are first verified.


## Architecture
![Architectuur](./architecture-devops.png)

## Components

- Portainer: [portainer](https://portainer.mlcrosoft-online.site)
- Todo applicatie [Todo-app](https://todo.mlcrosoft-online.site/)
- Jeknins [Jenkins CI/CD](https://jenkins.mlcrosoft-online.site/)

