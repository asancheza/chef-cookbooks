## Install Chef Server

### Ubuntu

Updating repositories:

```
curl -s https://packagecloud.io/install/repositories/chef/stable/script.deb.sh | sudo bash
sudo apt-get install chef-server-core=12.4.1-1
```
Installing Chef 12 package:
````
wget https://web-dl.packagecloud.io/chef/stable/packages/ubuntu/trusty/chef-server-core_12.0.5-1_amd64.deb
dpkg -i chef-server*
```

### Configuration

Reconfigure chef server:
```
chef-server-ctl reconfigure
```

Create username:
```
chef-server-ctl user-create USERNAME FIRST_NAME LAST_NAME EMAIL PASSWORD
```

Example
```
chef-server-ctl user-create admin admin admin admin@example.com examplepass -f admin.pem
```
```
chef-server-ctl org-create neurowork "Neurowork" --association_user admin -f neurowork-validator.pem
```

