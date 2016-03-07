## Install Chef Server

### Ubuntu

Updating repositories:

```
curl -s https://packagecloud.io/install/repositories/chef/stable/script.deb.sh | sudo bash
sudo apt-get install chef-server-core=12.4.1-1

Installing Chef 12 package:
````
wget https://web-dl.packagecloud.io/chef/stable/packages/ubuntu/trusty/chef-server-core_12.0.5-1_amd64.deb
dpkg -i chef-server*
```

Reconfigure chef server:
```
chef-server-ctl reconfigure
```
