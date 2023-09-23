# Installation
## Using the terminal
1. Download the docker-compose.yml file to your system
2. run ``docker-compose up -d`` (docker & docker-comose needs to be installed on the system)

## Using portainer:
1. Login to portainer
2. Create new Stack 
3. Copy the contents form the docker-compose.yml file to the editor in portainer

## Configuration
1. Login to your reversy proxy via web  using the following credentials:
   - **User:** admin@example.com
   - **Password:** changeme
2. Change login information on prompt
3. Create new proxy host
4. Set following settings: in tab "Details":
   - **Domain names:** proxy.domain.tld
   - **Scheme:** http
   - **Forward Hostname / IP:** localhost
   - **Forward Port:** 81
   - **Websockets Support:** on
5. Set following settings: in tab "SSL":
   - **SSL Certificate:** Request a new SSL Certificate
   - **Force SSL:** on
   - **HTTP/2 Support:** 
   - **Email Address for Let's Encrypt:** ADMIN-EMAIL
   - **I Agree to the Let's Encrypt Terms of Service** on