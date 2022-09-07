sudo mkdir -p /home/akhalalfood/html

sudo vi /etc/selinux/config

sudo ls -dZ /home/akhalalfood/log/

sudo semanage fcontext -a -t httpd_log_t "/home/akhalalfood/log(/.*)?"

sudo restorecon -R -v /home/akhalalfood/log

sudo ls -dZ /home/akhalalfood/log

ls -lZ /home/akhalalfood/log

https://www.digitalocean.com/community/tutorials/how-to-install-the-apache-web-server-on-centos-7
