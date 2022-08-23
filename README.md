# Konyha Hosting

Use this repository to host [Konyha](https://github.com/balzss/konyha) with the official [docker images](https://hub.docker.com/u/konyha) on a server or locally.

## Running

1. Clone this repository

```
git clone https://github.com/balzss/konyha-hosting && cd konyha-hosting
```

2. Copy the `.env.example` file to `.env` and add your variables

3. Start the containers with docker compose

```
docker compose up
```

4. If everything went right the manager app should be live at `$MANAGER_DOMAIN`, the home page and docs at
   `$SITEGEN_DOMAIN` and the published recipes at `$SITEGEN_DOMAIN/<user id>`

### Reverse proxy

Use the `reverse-proxy` profile to run with traefik:

```
docker compose --profile reverse-proxy up
```
