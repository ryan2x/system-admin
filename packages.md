# Ubuntu Packages

Install Java 8
~~~
sudo add-apt-repository ppa:webupd8team/java
sudo apt-get update
sudo apt-get install oracle-java8-installer
~~~

### apt tips

Restore /etc/ configuration files from the default
~~~
sudo apt-get install --reinstall -o Dpkg::Options::="--force-confmiss" <package>
sudo dpkg -l | grep <package>
sudo apt-get remove <package>
sudo apt-get purge <package>
~~~
