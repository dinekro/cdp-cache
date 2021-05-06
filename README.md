## Для запуска отладки используем команды
из текущей директории

`docker run -it -p 443:443 --mount type=bind,source="%cd%",target=/app golang:1.14 bash`

`cd /app && go get -u github.com/caddyserver/xcaddy/cmd/xcaddy && PATH=$PATH:/app`

`xcaddy run --config ./Caddyfile-dev`