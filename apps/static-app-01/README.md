see [`manifest.yml`](manifest.yml)

```sh
# deploy
cf push static-app-01 -n static-app-01 -m 64M
```

### Custom Domain

add custom domain via `route(s)` in [`manifest.yml`](manifest.yml)
```yml
  routes:
  - route: static-app-01.minote.net
```

update on DNS provider
e.g. `static-app-01.minote.net` via hover DNS for `minote.net` domain
![](https://www.evernote.com/l/AAFuWrkBAfZInIzyH50s7WCxTPZxj41FUB4B/image.png)