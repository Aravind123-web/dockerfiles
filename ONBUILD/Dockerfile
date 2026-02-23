FROM almalinux:9
RUN yum install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html # This will remove the default index.html file from nginx.
ONBUILD ADD index.html /usr/share/nginx/html/
CMD ["nginx", "-g", "daemon off;"]