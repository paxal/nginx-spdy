nginx-spdy
==========

NGINX Ebuild with SPDY patch


How to install the repository
-----------------------------

See http://en.gentoo-wiki.com/wiki/Overlay#Local_Overlays to see how to install local overlays

Then clone repository :

    git clone http://github.com/paxal/nginx-spdy

Install nginx with spdy module
------------------------------

Unmask the ebuild : add ebuild to `/etc/portage/package.unmask` and `/etc/portage/package.keywords`, and add the `nginx_modules_http_spdy` use flag.

Note
----

This package requires `>=dev-libs/openssl-1.0.1`. This won't break linked binaries as the library is still `libssl.so.1.0.0`.
