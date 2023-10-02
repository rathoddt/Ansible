#  Setting Up Environment

Installation

```
sudo apt-get install python3-pip

sudo pip install ansible
```



Checking Ansible version

`ansible --version`

### Basic Commands
```
ls                                                                                  
ansible --list-hosts all                                                            
ansible -i host-dev --list-hosts all                                                
vim host-dev                                                                        
ansible -i host-dev --list-hosts all                                                
vim ansible.cfg                                                                     

ansible --list-hosts all                                                            
                                                                                  
cat ansible.cfg                                                                     
ls                                                                                  

ansible --list-hosts all                                                            
ansible --list-hosts webservers                                                     
ansible --list-hosts loadbalancers                                                  

ansible --list-hosts all                                                            

ansible --list-hosts "*"                                                            
ansible --list-hosts app*                                                           
ansible --list-hosts webservers:loadbalanccsers                                     
ansible --list-hosts webservers:loadbalancers                                       
ansible --list-hosts \!control                                                      
ansible --list-hosts webservers[0] 
```