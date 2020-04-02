FROM quay.io/kubernetes-ingress-controller/nginx-ingress-controller:0.26.1

USER root

RUN luarocks install lua-resty-jwt
USER www-data

COPY etc/nginx/template/nginx.tmpl /etc/nginx/template
COPY etc/nginx/lua/plugins/jwt-auth /etc/nginx/lua/plugins/jwt-auth
