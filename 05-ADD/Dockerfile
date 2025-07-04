FROM almalinux:9
RUN dnf install nginx -y
RUN rm -f /usr/share/nginx/html/index.html
ADD https://raw.githubusercontent.com/vijayrajkoduru/Terraform/refs/heads/main/12-user-data/ec2.tf /usr/share/nginx/html/index.html
RUN chmod +r /usr/share/nginx/html/index.html
CMD ["nginx", "-g", "daemon off;"]
