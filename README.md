# Premessa
OS : RHEL, CentOS, AmazonLinux

# Procedura
```
sudo yum install httpd-tools 
```
```
sudo htpasswd -c /etc/nginx/.htpasswd <user>
```
Verrà chiesta quindi la password.  
In Nginx si dovranno aggiungere le stringhe:
```
auth_basic "Restricted";
auth_basic_user_file /etc/nginx/.htpasswd;
```
