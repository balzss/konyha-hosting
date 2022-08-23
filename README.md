# Konyha Hosting

Use this repository to host [Konyha](https://github.com/balzss/konyha) with the official [docker images](https://hub.docker.com/u/konyha) on a server.

## Running

1. Clone this repository

```
git clone https://github.com/balzss/konyha-hosting && cd konyha-hosting
```

2. Copy the `.env.example` file to `.env` and add your variables

3. Start containers with docker compose

```
docker compose up
```

### Reverse proxy

Use the `reverse-proxy` profile to run with traefik:

```
docker compose --profile reverse-proxy up
```
