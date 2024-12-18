`sudo vi /var/snap/caddy-gael/current/Caddyfile`

```
{
        # Global options block
        admin off
        email gael.legoff@gmail.com
}

# What's on public site
whatson.legoff.be {
        # Enable automatic HTTPS with Let's Encrypt
        tls gael.legoff@gmail.com

        # Define the root directory for your site
        root * /var/snap/caddy-gael/common/whatson.legoff.be/www/html

        # Enable file server
        file_server
}
```

`sudo snap restart caddy-gael.caddy`
