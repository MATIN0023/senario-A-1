kubetail command help :

for url web : 
```BASH
kubetail serve
```

for use ssl : 
openssl req \
  -subj "/C=RU/ST=XXX-XXX/L=XXX-XXX/O=Labecs, Inc./OU=GitLab/CN=git.mydomain.ru" \
  -newkey rsa:4096 -nodes -sha256 -keyout ./git.mydomain.ru-ss.key \
  -x509 -days 3650 -out ./git.mydomain.ru-ss.crt

move file for ssl :

cp /etc/ssl/gitlab/git.mydomain.ru-ss.crt /etc/gitlab/trusted-certs/