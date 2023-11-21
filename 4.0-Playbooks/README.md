# Ansible Playbook


## 4.1 ping and uname playbook
```
mkdir playbooks
vim playbook/ping.yaml 
ansible-playbook playbooks/ping.yaml                                           
vim ansible.cfg                                                                
ansible-playbook playbooks/ping.yaml                                           
vim playbooks/uname.yaml                                                       
ansible-playbook playbooks/uname.yaml                                          

```


## 4.2 Playbooks, service handlers
```
ansible-playbook playbooks/yum-update-01.yml
cat hosts-dev
ansible-playbook playbooks/yum-update-01.yml


cat playbooks/install-services.yml
ansible-playbook playbooks/install-services.yml

cat playbooks/yum-update-01.yml
cat ansible.cfg
cat playbooks/install-services.yml
cat playbooks/uname.yaml

cat playbooks/ping.yaml

nano yum-update.yml

cp ping.yaml yum-update-01.yml
vim yum-update-01.yml
nano yum-update-01.yml
vim ../ansible.cfg
vim install-services.yml
nano install-services.yml
vim install-services.yml
nano install-services.yml
cd ansible/playbooks/

ansible-playbook playbooks/install-services.yml

cat playbooks/install-services.yml
nano playbooks/install-services.yml
cd ansible/
vim playbooks/install-services.yml
ansible-playbook playbooks/install-services.yml
echo "<h1> Hello world! This is Ansibe page" > index.php
cat index.php
ls
echo "<h1> Hello world! This is Ansibe page</h1>" > index.php

vim index.php
vim playbooks/setup-app.yml
ansible-playbook playbooks/setup-app.yml
vim playbooks/setup-app.yml
ansible-playbook playbooks/setup-app.yml
vim index.php
ansible-playbook playbooks/setup-app.yml
vim index.php
ansible-playbook playbooks/setup-app.yml
vim playbooks/setup-app.yml
ansible-playbook playbooks/setup-app.yml
mkdir config
vim config/lb-config.j2
cd ansible/
cat config/lb-config.j2
vim playbooks/setup-lb.yml
ansible-playbook playbooks/setup-lb.yml
ansible-playbook playbooks/setup-app.yml
vim playbooks/setup-app.yml
ansible-playbook playbooks/setup-app.yml
vim playbooks/setup-app.yml
ansible-playbook playbooks/setup-app.yml
vim playbooks/setup-app.yml
ansible-playbook playbooks/setup-app.yml
vim playbooks/setup-lb.yml
ansible-playbook playbooks/setup-lb.yml

cat playbooks/ping.yaml
ansible-playbook playbooks/ping.yaml
ansible-playbook playbooks/uname.yaml

cat playbooks/yum-update.yml
cat playbooks/yum-update-01.yml
ansible-playbook playbooks/yum-update-01.yml
cat ansible.cfg
ansible-playbook playbooks/yum-update-01.yml
ansible-playbook playbooks/install-services.yml

ansible-playbook playbooks/setup-app.yml

ansible-playbook playbooks/setup-lb.yml
ansible-playbook playbooks/setup-app.yml
cat playbooks/setup-lb.yml


vim playbooks/all-playbooks.yml
ansible-playbook playbooks/all-playbooks.yml
cat playbooks/yum-update

vim playbooks/all-playbooks.yml
ansible-playbook playbooks/all-playbooks.yml
vim playbooks/check-status.yml
ansible-playbook playbooks/check-status.yml
vim playbooks/check-status.yml
ansible-playbook playbooks/check-status.yml


ansible -m service -a "name=httpd state=stopped" -become loadbalancers
ansible-playbook playbooks/check-status.yml
ansible -m service -a "name=httpd state=started" -become loadbalancers
ansible-playbook playbooks/check-status.yml
vim playbooks/all-playbooks.yml
ansible-playbook playbooks/all-playbooks.yml

```

## 4.3 Variables

```
http://3.229.151.112/balancer-manager
```
Create variables from info returned tasks ran using `register`.

Use the `debug` module anytime to see variables and debug out playbooks

