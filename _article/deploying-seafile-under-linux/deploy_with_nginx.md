---
post_title: Configure Seafile with Nginx under Linux
layout: ht_kb
published: true
---
# Configure Seafile with Nginx under Linux

## Important

According to this [security advisory](https://www.djangoproject.com/weblog/2013/aug/06/breach-and-django/) published by Django team, we recommend to disable [GZip compression](http://wiki.nginx.org/HttpGzipModule) to mitigate [BREACH attack](http://breachattack.com/).

## Deploy Seahub/FileServer with Nginx

Seahub is the web interface of Seafile server. FileServer is used to handle raw file uploading/downloading through browsers. By defaults, it listens on port 8082 for HTTP request.

TO BE DONE

Please see http://manual.seafile.com/deploy/deploy_with_nginx.html
