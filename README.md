nginx
=====

The nginx image runs [nginx](http://nginx.org/) on top of the
[phusion/baseimage](https://registry.hub.docker.com/u/phusion/baseimage/)
container.


Usage
-----

You can get a simple static content server up and running by using the following
command:

```bash
$ docker run
  --name nginx \
  -p 0.0.0.0:80:80
  -v /some/content:/usr/share/nginx/html:ro
  jleight/nginx
```