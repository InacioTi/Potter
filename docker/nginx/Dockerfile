FROM nginx:1.19.6-alpine

RUN echo "nameserver 8.8.8.8" > /etc/resolv.conf

RUN rm /etc/nginx/nginx.conf
COPY nginx.conf /etc/nginx/

RUN rm /etc/nginx/conf.d/default.conf
COPY potter.conf /etc/nginx/conf.d/