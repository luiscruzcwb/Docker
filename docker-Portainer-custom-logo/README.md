# Portainer com logo personalizada


```yaml
docker run -d -p 9000:9000 -p 8000:8000 -v /var/run/docker.sock:/var/run/docker.sock portainer/portainer-ce --logo https://logodetimes.com/times/flamengo/logo-flamengo-antigo-2048.png
```

```yaml
version: '3'
services:
  portainer:
    image: portainer/portainer-ce
    ports:
      - 9000:9000
      - 8000:8000
    volumes:
      - /var/run/docker.sock:/var/run/docker.sock
    command: --logo https://logodetimes.com/times/flamengo/logo-flamengo-antigo-2048.png

```

Para mais informações sobre o Portainer - administração de containers acesse: https://docs.portainer.io

<p><strong><img style="float: left;" src="https://www.portainer.io/hubfs/portainer-logo-black.svg" alt="" width="200" height="200" /></strong></p>