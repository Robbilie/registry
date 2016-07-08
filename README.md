# Docker Registry (with Docker-Compose, Basic Auth, Letsencrypt)

* Install Docker Engine / Docker Compose 1.6+
* Install Apache2 tools (`htpasswd` tool is the important part)
* Install letsencrypt/certbot
* `htpasswd -c -B -C 10 htpasswd yourusername`
* `htpasswd -B -C 10 htpasswd subsequentusers`
* `letsencrypt certonly`
* Change the domain to your own for the certificate mappings in `docker-compose.yml`
* `docker-compose up -d`

## FAQ

* I've seen some letsencrypt options for the registry image, why don't you use those?

  If you figure out how they work, please let me know!
