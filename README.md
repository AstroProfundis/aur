Packages I'm maintaining on AUR
======

These are the packages I'm currently maintaining on `AUR` (Arch User Repository):

* `bind-rl`: BIND named server with Response Rate Limiting(RRL) patch. (RRL helps to avoid an open DNS server from being used for [DNS flood](http://blog.cloudflare.com/the-ddos-that-knocked-spamhaus-offline-and-ho) DDoS attack, read [this article](http://www.redbarn.org/dns/ratelimits) on how to configure RRL.)
* `eaccelerator-git`: A free open-source PHP accelerator, optimizer, and dynamic content cache. ([The git version](https://github.com/eaccelerator/eaccelerator) supports `PHP 5.5.x`)
* `mod_fcgid-legacy`: A FastCGI module for Apache HTTP Server, build with apache httpd 2.2 (apache22)
* `mod_python`: An Apache module that embeds the Python interpreter within the server
* `mod_python2`: An Apache module that embeds the Python 2.7 interpreter within the server
* `mod_python2-legacy`: An Apache 2.2 module that embeds the Python 2.7 interpreter within the server
* `mod_remoteip`: A backport of [`mod_remoteip`](http://httpd.apache.org/docs/current/mod/mod_remoteip.html) in apache httpd 2.4.x
* `nginx-accesskey`: Lightweight HTTP server and IMAP/POP3 proxy server, with [`ngx_http_accesskey_module`](http://wiki.nginx.org/HttpAccessKeyModule).
* `nginx-tcp`: Lightweight HTTP server and IMAP/POP3 proxy server, with [`nginx_tcp_proxy_module`](https://github.com/yaoweibin/nginx_tcp_proxy_module).
* `tengine`: A web server based on Nginx and has many advanced features, originated by Taobao.
* `tengine-extra`: A web server based on Nginx and has many advanced features, originated by Taobao. With some extra modules enabled.
* `tsar-git`: Taobao System Activity Reporter

Repository
======

I also provide a binary repository than includes all my AUR packages, It now have both `i686` and `x86_64` arch.

To use this `aspro` repo, add these to the end of your `/etc/pacman.conf` file:

    [aspro]
    SigLevel = TrustAll
    Server = http://fun.atr.me/archlinux/$arch

And you may need to sign my key, otherwise you'll have to set `SigLevel = Never`:

    sudo pacman-key --lsign-key BB01E61B

Read more about `pacman-key` on [wiki](https://wiki.archlinux.org/index.php/Pacman-key).
