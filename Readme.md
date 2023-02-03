 Install java 8  centos manually
 -------------------------------------
 * Here install java 8
 * [refer here](https://www.liquidweb.com/kb/install-java-8-on-centos-7/)
  ```
sudo yum -y update
sudo yum install java-1.8.0-openjdk
java -version
  ```
   ![image](images/ansible1.png)
   ![image](images/ansible2.png)
   ![image](images/ansible3.png)

 Install java 11  centos manually
 -------------------------------------
 * Here install java 11
 * [refer here](https://linuxize.com/post/install-java-on-centos-7/)
  ```
sudo yum install java-11-openjdk-devel
java  -version
  ```
![image](images/ansible4.png)
![image](images/ansible5.png)

dotnet 7.0 install on centos manually
-------------------------------------
* Here install dotnet 7.0 
* [refer](https://learn.microsoft.com/en-us/dotnet/core/install/linux-centos)
  ```
  sudo rpm -Uvh https://packages.microsoft.com/config/centos/7/packages-microsoft-prod.rpm

  sudo yum install dotnet-sdk-7.0
  ```
![image](images/ansible6.png)
![image](images/ansible7.png)

Nopcommerce application on ubuntu manually
------------------------------------------

* Here install nopcommerce
* [refer here](https://docs.nopcommerce.com/en/installation-and-upgrading/installing-nopcommerce/installing-on-linux.html)
  
 ```
  sudo apt update
  wget https://packages.microsoft.com/config/ubuntu/20.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb
  sudo dpkg -i packages-microsoft-prod.deb
  sudo apt-get update
  sudo apt-get install -y apt-transport-https aspnetcore-runtime-7.0
  dotnet --list-runtimes
  sudo apt-get install nginx
  sudo systemctl start nginx
  sudo systemctl status nginx
  sudo vi /etc/nginx/sites-available/default
  sudo mkdir /var/www/nopCommerce
  cd /var/www/nopCommerce
  sudo wget https://github.com/nopSolutions/nopCommerce/releases/download/release-4.60.1/nopCommerce_4.60.1_NoSource_linux_x64.zip
  sudo apt-get install unzip
  sudo unzip nopCommerce_4.60.1_NoSource_linux_x64.zip
  sudo mkdir bin
  sudo mkdir logs
  cd ..
  sudo chgrp -R www-data nopCommerce/
  sudo chown -R www-data nopCommerce/
  sudo vi /etc/systemd/system/nopCommerce.service
  sudo systemctl start nopCommerce.service
  sudo systemctl status nopCommerce.service
  sudo systemctl restart nginx
    "http://publicip/install"

 ``` 
 ![preview](images/nop1.png)
 ![preview](images/nop2.png)
 ![preview](images/nop3.png)
 ![preview](images/nop4.png)
 ![preview](images/nop5.png)
 ![preview](images/nop6.png)

 
