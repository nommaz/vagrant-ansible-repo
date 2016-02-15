eksik işler

- vsftpd.cnf dosyasindaki public ip
- /home/ftpuser chmod 775
- adduser nommazve ftpuser
- private key'in source kontrolde olmamasi
- 

nginx
 - /var/www/nginx-default/packageserver create
 
both
 - create key pair on ftp01 and add public to ftp02/authorized/keys
 - lsyncd -rsyncssh /home/ftpuser 172.25.2.101 /home/ftpuser
 
 still need to run lsyncd on start for ftp01 and repo01
 https://gist.github.com/srounet/4111191
 
 create backup!!