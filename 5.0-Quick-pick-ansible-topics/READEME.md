
## 5.1 Roles
```
cp -r ansible/ ansible-v2/
ls
ls ansible-v2/
cd ansible-v2/
mkdir roles
mv ansible.cfg roles/
mv index.php roles/
mv hosts-dev roles/
ls roles/
mv roles/ ansible-roles
ls
cd ansible-roles/
mkdir roles
ansible-galaxy roles/webservers init
ls
ansible-galaxy role roles/webservers init
ls
ls roles/
ansible-galaxy init roles/webservers
ls roles/
ls roles/webservers/
cat roles/webservers/README.md
ls
ls roles/webservers/
ls ../../
cat ../playbooks/setup-app.yml
ls roles/webservers/
vim roles/webservers/tasks/main.yml
vim roles/webservers/vars/main.yml
vim roles/webservers/handlers/main.yml
vim roles/webservers/tasks/main.yml
ls
mv index.php roles/webservers/files/
ls
vim roles/webservers/tasks/main.yml
vim ../playbooks/setup-app.yml
ansible-playbook ../playbooks/setup-app.yml
ls roles/
vim ../playbooks/setup-app.yml
ansible-playbook ../playbooks/setup-app.yml
mv ../playbooks/setup-app.yml .
ls
ansible-playbook setup-app.yml
mv ../playbooks/ping.yaml .
ls
ansible-playbook ping.yaml
ls
ls ../
cp ../key.pem
cp ../key.pem .
ansible-playbook ping.yaml
ansible-playbook setup-app.yml
```


## 5.2 Check Mode
Dry run the heck book
```
ansible-playbook playbooks/setup-app-check-mode.yml --check
```


## 5.3 Error handling
```
vim playbooks/check-status.yml
ansible-playbook playbooks/check-status.yml
```

## 5.4 Tags
```
ansible-playbook playbooks/setup-tags.yml --tags upload
ansible-playbook playbooks/setup-tags.yml --tags create-info-page
ansible-playbook playbooks/setup-tags.yml --skip-tags upload
```