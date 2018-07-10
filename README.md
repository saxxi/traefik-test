# Træfik example


## Through docker compose

```
cd through-docker-compose
docker-compose up
```
Now http://whoami.docker.localhost/ and http://portainer.docker.localhost/ should start working.

If it doesn't please add in your `/etc/hosts` file:

```
127.0.0.1 whoami.docker.localhost
127.0.0.1 portainer.docker.localhost
```

And flush your DNS before starting your docker instances.

## Through binary file

Grab the binary from [here](https://github.com/containous/traefik/releases).
For OS it's the Darwin one.

```
cd through-binary
[install your traefik binary]
sudo ./traefik -c Traefik.toml
```

