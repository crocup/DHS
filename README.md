# Dionaea-Honeypot-Script

Dionaea is meant to be a nepenthes successor, embedding python as scripting language, using libemu to detect shellcodes, supporting ipv6 and tls.

Protocols
---------

* blackhole
* epmap
* ftp
* http
* memcache
* mirror
* mqtt
* mssql
* mysql
* pptp
* sip
* smb
* tftp
* upnp

Logging
-------

* fail2ban
* hpfeeds
* log_json
* log_sqlit

Install
-------------
```bash
git clone https://github.com/crocup/DHS
cd DHS
chmod +x dhs.sh
./dhs.sh
```

Licenses
--------

* dionaea: GPLv2+
* tftp service(modules/python/tftp.py): CNRI Python License (incompatible with GPL)
* parts of ftp service(modules/python/ftp.py): MIT (compatible with GPL)

Documentation
-------------

* [Documentation](https://dionaea.readthedocs.io/)
