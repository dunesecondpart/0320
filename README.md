# Installing Apache WebServer

# install some virtual machine software like VMWare
https://www.vmware.com/products/workstation-pro.html

# Create a virtual machine, install ubuntu server
https://ubuntu.com/server

# add the apache web server
- https://httpd.apache.org/
- https://ubuntu.com/tutorials/install-and-configure-apache#1-overview (for reference only)


### simplifed instructions for installing Apache

```
sudo apt update
sudo apt install apache2
```

# Test Apache operation

## to get the ip address of the virtual machine
```
ip a
```

on your desktop computer, navigate to the ip address provided to interact with the webserver from a browser of your choice.
You should see the apache2 web page that is installed with the web server software. Typically we would replace that index.html
with our OWN index.html file

# rename the index.html to default.html
```
cd /var/www/html
ls -l
sudo su
mv index.html default.html
```

Navigate and/or reload the page to see that when NO index.html file is present, the default configuration of the web server software displays a directory listing. Navigate to the default page by specifically calling default.html in the URL.

