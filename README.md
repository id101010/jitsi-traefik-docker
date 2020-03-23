# jitsi-traefik-docker

A dockerized jitsi videocall service with traefik reverse proxy that handles letsencrypt certificates and routing.

## What do I need to configure?

* docker-compose.yml:61: Change frontend rule to your FQDN
* traefik.toml:9: Add password for your traefik frontend using `htpasswd -nb $USER $PASSWORD`
* traefik.toml:25: Change acme email
* traefik.toml:34: Change domain name
* .env:18: Change FQDN

## Todo

- [ ] Add traefik setup to the docker-compose file
- [ ] Export above configs using the .env file

## Contributions are Welcome!
