docker-ucp-lb
=============

docker image for HAProxy to load balance UCP
based off of haproxy:1.6-alpine

To build this image:
`docker build -t ucp-lb .`

Example usage:
`docker run -d -p 443:443 -p 8181:8181 --name ucp-lb ucp-lb`

The `haproxy.cfg` should be updated to match your environment.
