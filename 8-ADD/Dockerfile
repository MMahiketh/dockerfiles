FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://raw.githubusercontent.com/MMahiketh/terraform-vpc-module/refs/heads/master/readme.MD /usr/share/nginx/html/index.html
RUN chmod +r /usr/share/nginx/html/index.html
ADD sample-1.tar 
CMD ["nginx", "-g", "daemon off;"]
