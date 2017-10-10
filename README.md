#docker-ghost-blog

A docker composition of GHOST, NGINX with SSL termination and MYSQL database.

## Requirements
- Docker https://www.docker.com/
- Docker-Compose https://docs.docker.com/compose/
- A server
- A domain
- An SSL certificate and key
- An email account (SMTP service)

## How to run
1. Clone this project to your server
2. Add your SSL certificate and key to nginx/ssl/
3. Set the server_name and ssl_certificate in nginx/default.conf
4. Edit database settings in docker-compose.yml
5. Edit settings in ghost/config.production.json
    - Blog domain
    - Database settings
    - Email settings
6. Run ```docker-compose up -d```
7. Check https://yourUrl.com/ (if your domain's DNS is point to your server)
