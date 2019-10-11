# traefik-examples(v2)
This repository include configurations of some use cases of [traefik](https://traefik.io/). 

## summary
Configurations of traefik v2 are separated to 2 parts - static config and dynamic config.  
In my examples, I always put static config into one file `/home/data/traefik/traefik.toml` and dynamic config into different places depending on providers.(eg: `/home/data/traefik/toml/*.toml` for file provider, `docker labels` for docker provider).

## providers
As we all known, traefik supports multi type of providers, I will write example configurations for [docker-provider](./docker-provider) and [file-provider](./file-provider).

## contributions


