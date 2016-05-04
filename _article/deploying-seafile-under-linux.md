---
ID: 53
post_title: Deploying Seafile under Linux
author: Alexander Jackson
post_date: 2016-05-03 19:20:43
post_excerpt: ""
layout: ht_kb
permalink: >
  https://support.seafile.de/knowledge-base/deploying-seafile-under-linux/
published: true
---
# Deploying Seafile under Linux

Here we describe how to deploy Seafile from prebuild binary packages.

### Deploy Seafile in Home/Personal Environment

*   [Deploying Seafile with SQLite][1]

### Deploy Seafile in Production/Enterprise Environment

In production environment we recommend using MySQL as the database and config Seafile web behing Nginx or Apache. For those who are not familiar with Nginx and Apache. We recommend Nginx, since it is easier to config than Apache.

Note: We have prepared an installation script [Deploy Seafile with an installation script][2]. The installer offer a quick and easy way to set up a production ready Seafile Server using MariaDB, Memcached and NGINX as a reverse proxy in under 5 minutes.

You can also install Seafile manually without the installation script as following:

Basic:

*   [Deploying Seafile with MySQL][3]
*   [Config Seahub with Nginx][4]
*   [Enabling Https with Nginx][5]
*   [Config Seahub with Apache][6]
*   [Enabling Https with Apache][7]

Advanced:

*   [Add Memcached][8], adding memcached is very important if you have more than 50 users.
*   [Start Seafile at System Bootup][9]
*   [Firewall settings][10]
*   [Logrotate][11]

User Authentication:

Seafile supports a few external user authentication methods.

*   [Configure Seafile to use LDAP][12]
*   [Shibboleth Authentication][13]

Other Deployment Issues

*   [Deploy Seafile behind NAT][14]
*   [Deploy Seahub at Non-root domain][15]
*   [Migrate From SQLite to MySQL][16]

Check [configuration options][17] for server config options like enabling user registration.

**Read here** if you have troubles setting up Seafile server

1.  Read [Seafile Server Components Overview][18] to understand how Seafile server works. This will save you a lot of time.
2.  [Common Problems for Setting up Server][19]
3.  Go to our [forum][20] for help.

## Upgrade Seafile Server

*   [Upgrade Seafile server][21]

## For those that want to package Seafile server

If you want to package seafile yourself, (e.g. for your favorite Linux distribution), you should always use the correspondent tags:

*   When we release a new version of seafile client, say 3.0.1, we will add tags `v3.0.1` to ccnet, seafile and seafile-client.
*   Likewise, when we release a new version of seafile server, say 3.0.1, we will add tags `v3.0.1-server` to ccnet, seafile and seahub.
*   For libsearpc, we always use tag `v3.0-latest`.

**Note**: The version numbers of each project has nothing to do with the tag name.

 [1]: using_sqlite.md
 [2]: https://forum.seafile-server.org/t/seafile-server-installer-for-production-ready-seafile-ce-and-pro-installations/1464
 [3]: using_mysql.md
 [4]: deploy_with_nginx.md
 [5]: https_with_nginx.md
 [6]: deploy_with_apache.md
 [7]: https_with_apache.md
 [8]: add_memcached.md
 [9]: start_seafile_at_system_bootup.md
 [10]: using_firewall.md
 [11]: using_logrotate.md
 [12]: using_ldap.md
 [13]: shibboleth_config.md
 [14]: deploy_seafile_behind_nat.md
 [15]: deploy_seahub_at_non-root_domain.md
 [16]: migrate_from_sqlite_to_mysql.md
 [17]: ../config/README.md
 [18]: ../overview/components.md
 [19]: common_problems_for_setting_up_server.md
 [20]: https://forum.seafile-server.org/
 [21]: upgrade.md