# DHS (Dionaea-Honeypot-Script)
* [Documentation](https://dionaea.readthedocs.io/)
* [Github repo Dionaea](https://github.com/DinoTools/dionaea)

Dionaea is meant to be a nepenthes successor, embedding python as scripting language, using libemu to detect shellcodes, supporting ipv6 and tls.
## About 
Dionaea Hobeypot `Docker` Image

Logging
-------
* log_json
* log_sqlite

Install
-------------
```bash
$ git clone https://github.com/crocup/DHS
$ cd DHS/
$ sudo docker build . -t honey
$ sudo docker run -it --rm -v /opt/honey/log:/opt/dionaea/var/log -p 21:21 -p 80:80 -p 123:123 -p 443:443 -p 445:445 -p 1443:1443 -p 11211:11211 --name dio honey
```

Exec docker
--------
```bash
$ sudo docker exec -it dio /bin/bash
```

Log files
--------
JSON
```bash
$ cat /opt/honey/log/dionaea.json
```

Database(SQLite)
```sqlite
select * from connections
```

Licenses
--------
* dionaea: GPLv2+
* all my files MIT (compatible with GPL)
-------------

In the Future
--------
- create analytic program: Core(FastAPI)