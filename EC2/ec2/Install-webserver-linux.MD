## After Launching an EC2 with Amazon Linux AMI

### Become the super user . The super user like Admin user on Windows. No restrictions.
```
sudo su
```
### Install the web server
```
yum install -y httpd
```

### Start the web server
```
service httpd start
```

### Make sure the webserver is started after restart
```
chkconfig httpd on
```

### Add permissions to make the web server publicly available
```
chmod 755 -R /var/www/
```

### Browse the IP of the instance in a web browser 

### Add your content to the index.html file
```
 echo "hello from VA 1 ">/var/www/html/index.html
```

### Browse the IP of the instance in a web browser again. 
