## Purpose

A basic test of varnish cache server as reverse proxy with an apache2 backend.
    
## Usage

    docker-compose up -d
    
## Test

### Send a request via varnish

    curl http://localhost
    
### Send a request directly

    curl http://localhost:8080

### Check if webserver has been accessed 

    docker exec varnish_web_1 tail  /var/log/apache2/access.log