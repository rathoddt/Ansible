# Ansible Tasks

Ansible tasks are ad hoc commands executed against inventory

```
ansible -m ping all                                                            
vim key.pem                                                                    
vim ansible.cfg                                                                
chmod 400 key.pem                                                              
vim ansible.cfg                                                                
ansible -m ping all                                                            
ansible -m shell -a "uname" webservers:loadbalancers"                          
ansible -m shell -a "uname" webservers:loadbalancers                           
ansible -m command -a "/bin/false" \!local
```