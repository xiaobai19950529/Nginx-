# Nginx-

1. nginx 丢失nginx.pid

    有时候会遇到nginx.pid文件丢失的情况。解决办法：
    /usr/sbin/nginx  -c  /etc/nginx/nginx.conf
    前面是nginx的启动文件，后面是配置文件。
    pid文件一般在/run/路径下
    
2. 使改动过的/etc/hosts生效
    
    a.重启服务
        sudo /etc/init.d/networking restart
        
    b.重启机器
        sudo reboot
        
    c.使用hostname命令
        hostname 定义的主机名

3. sudo apt-get install http-server
   
      http-server -p port  直接在当前目录以port端口号启动http-server服务
    
      sudo nginx -s reload 或
    
      sudo service nginx restart
    
    
4. sudo nano /etc/nginx/nginx.conf
  
      负载均衡教程： http://natumsol.github.io/2016/03/16/nginx-basic/
