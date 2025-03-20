FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/mginx/html/index.html
ADD https://github.com/daws-81s/terraform-python-ec2/blob/master/README.MD /usr/share/nginx/html/index.html
RUN chmod +xr /usr/share/nginx/html/index.html
CMD ["nginx", "-g", "daemon off;"]
