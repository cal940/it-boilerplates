# Installation
1. Download the docker-compose.yml file to your system
2. run ``docker-compose up -d`` (docker & docker-comose needs to be installed on the system)

## Setup reverse proxy (nginx-proxy manager)
1. Login to your reversy proxy via web interface
2. Create new proxy host
3. Set following settings: in tab "Details":
   - **Domain names:** portainer.domain.tld
   - **Scheme:** https
   - **Forward Hostname / IP:** portainer.local
   - **Forward Port:** 9443
   - **Websockets Support:** on
4. Set following settings: in tab "SSL":
   - **SSL Certificate:** Request a new SSL Certificate
   - **Force SSL:** on
   - **HTTP/2 Support:** 
   - **Email Address for Let's Encrypt:** ADMIN-EMAIL
   - **I Agree to the Let's Encrypt Terms of Service** on