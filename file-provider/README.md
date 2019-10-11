## summary
We write all dynamic config into config file(/home/data/traefik/toml/web.toml) in that section.  
> notice: we use docker container as backend services, but proxy via url(eg: http://whoami:80), it's different from `docker-provider`.

## quick-start
it's used as traditional reverse proxy and load balance service.  
+ file providers are supposed to run either on `traefik server`(server running traefik service) or another server.
+ easy to expand providers to support large requests dynamically. 

### proposal arch
![file-provider](../assets/file-provider.png)

## certs
example for automatically register let's encrypt certs (http challenge).

## http-to-https
redirect http to https.
