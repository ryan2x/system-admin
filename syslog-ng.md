# syslog-ng setup

syslog-ng with Java

~~~

https://syslog-ng.org/syslog-ng-3-7-3-unofficial-debianubuntu-packages/

wget -qO - http://download.opensuse.org/repositories/home:/laszlo_budai:/syslog-ng/xUbuntu_14.04/Release.key | sudo apt-key add -


echo "deb http://download.opensuse.org/repositories/home:/laszlo_budai:/syslog-ng/xUbuntu_14.04 ./" | sudo tee /etc/apt/sources.list.d/syslog-ng.list

sudo apt-get install syslog-ng-core
sudo apt-get install syslog-ng-mod-kafka
sudo apt-get install syslog-ng-mod-json

echo "/usrb/jvm/java-8-openjdk-amd64/jrebd64rver/" | sudo tee /etc/ld.so.conf.d/java.conf
echo "/usrb/jvm/java-8-oracle/jrebd64rver/" | sudo tee /etc/ld.so.conf.d/java.conf
sudo ldconfig
ldconfig -p | grep libjvm
~~~

