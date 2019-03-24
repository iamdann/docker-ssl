# Docker & Automatic SSL = 😍
This is a simple working example how to automatically secure your 
NodeJS / whatever application using a NGINX reverse proxy and [Certbot](https://certbot.eff.org/). 

This makes use of the [automatic NGINX proxy](https://github.com/jwilder/nginx-proxy) 
and [letsencrypt-nginx-proxy-companion](https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion).

## How to use

**Development:**
- Clone or download this repo
- **Modify** the `.env` located in `.env.example` to match your environment.  
- Run: `docker-compose up --build`

**Production:**
- Clone or download this repo
- **Modify** the `.env` located in `.env.example` to match your environment.  
- Run: `docker-compose -f docker-compose.yml -f docker-compose.production.yml up --build`