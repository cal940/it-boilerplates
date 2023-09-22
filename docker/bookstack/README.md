# How to use
## Using the terminal
1. Download the docker-compose.yml file to your system
2. run ``docker-compose up -d`` (docker & docker-comose needs to be installed on the system)

## Using portainer:
1. Login to portainer
2. Create new Stack 
3. Copy the contents form the docker-compose.yml file to the editor in portainer

## Setup reverse proxy (nginx-proxy manager)
1. Login to your reversy proxy via web interface
2. Create new proxy host
3. Set following settings: in tab "Details":
   - **Domain names:** APP-DOMAIN
   - **Scheme:** http
   - **Forward Hostname / IP:** bookstack.local
   - **Forward Port:** 80
   - **Websockets Support:** on
4. Set following settings: in tab "SSL":
   - **SSL Certificate:** Request a new SSL Certificate
   - **Force SSL:** on
   - **HTTP/2 Support:** 
   - **Email Address for Let's Encrypt:** ADMIN-EMAIL
   - **I Agree to the Let's Encrypt Terms of Service** on