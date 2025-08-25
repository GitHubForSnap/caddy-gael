_This is NOT an original piece of work, just a snap of caddy_

Caddy - Every site on HTTPS
Caddy is an extensible server platform that uses TLS by default

**First-time users**

* Read the doc at https://caddyserver.com/docs/

* Configure the server

`sudo vi /var/snap/caddy-gael/current/Caddyfile`

```
{
        # Global options block
        email mail@example.com
}

# File server
fileserver.example.com {
        # Define the root directory for your site
        root * /var/snap/caddy-gael/common/fileserver.example.com/www/html

        # Enable file server
	encode zstd gzip
        file_server browse
}
```

* Restart the server

`sudo snap restart caddy-gael.caddy`

**2025-08-25**
* v2.10.2 available on amd64

**2025-08-22**
* v2.10.1 available on amd64

**2025-04-27**
* v2.10.0 available on amd64

**2025-01-08**
* v2.9.1 available on amd64

**2025-01-04**
* v2.9.0 available on amd64

