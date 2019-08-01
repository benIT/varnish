## Purpose

A basic test of varnish cache server as reverse proxy with an apache2 backend.
    
## Usage

    docker-compose up -d
    
## Test

### Send a request

    curl http://localhost

### Check if webserver has been accessed 

    docker exec varnish_web_1 tail -f /var/log/apache2/access.log