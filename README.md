# Reverse proxy

## Traefik
Add the following to your hosts file:
```shell
echo '127.0.0.1 proxy.test mail.test' | sudo tee -a /etc/hosts
```

### start 
```shell
docker compose up --detach --build
```

You can now visit: http://proxy.test

For emails, visit: http://mail.test

### stop
```shell
docker compose down --volumes
```

