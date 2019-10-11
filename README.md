# traefik-examples(v2)
this repository include configurations of some use cases of [traefik](https://traefik.io/). 

## summary
configurations of traefik v2 is separated to 2 parts - static config and dynamic config.  
i always put static config into one file `/home/data/traefik/traefik.toml` and dynamic config into different places depending on providers.(eg: `/home/data/traefik/toml/*.toml` for file provider, `docker labels` for docker provider).

## quick-start
traefik offical quick start [demo](https://docs.traefik.io/getting-started/quick-start/).

## file-provider
it's used as traditional reverse proxy and load balance service.  
+ file providers are supposed to run either on `traefik server`(server running traefik service) or another server.
+ easy to expand providers to support large requests dynamically. 

### proposal arch
![file-provider](./assets/file-provider.png)

## certs
example for automatically register let's encrypt certs (http challenge).

## http-to-https
redirect http to https.

## docker-provider
+ use docker provider
+ let's encrypt certs(http challenge).
+ support both http and https
