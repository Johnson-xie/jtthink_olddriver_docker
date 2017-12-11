```
// docker 
// run 
// --privileged 
// -d 
// -p 8080:80 
// --name  myhttpd 
// -v /home/shenyi/myweb:/var/www/html 
// centos:httpd 
// /usr/sbin/init
docker run --privileged -d -p 8080:80 --name  myhttpd -v /home/shenyi/myweb:/var/www/html centos:httpd /usr/sbin/init
```