## basic traefik configuration

the following command initializes traefik with monitoring at traefik.manseau.dev

```
$ docker network create web && touch acme.json && chmod 600 acme.json && docker-compose up -d
```

to create a new monitoring user/pass, copy the output of the following command into traefik_dynamic.yml
```
$ htpasswd -nb admin secure_password
```
