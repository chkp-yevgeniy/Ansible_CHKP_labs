# Check Point Management (CHKP MGMT) automation with loop and data from an external file.

### 1. Purpose
This role is an example on how to create object, policy packages and rulebases in CHKP MGMT in an efficient way by means of loops and config data stored in a yaml file.  
Config data are stored in vars/.  
Loops are used in playbooks to iterate via config data.  


Following CheckPoint Ansible modules are used:
https://galaxy.ansible.com/check_point/mgmt
The modules (and therefore this role) are idempotent which is great! 


### 2. Requirements
- Ansible => 2.9
- Python => 2.7


### 3. How to run the role 

3.1 Adjust inventory according to your environment:  
```bash
 inventory.yml
```

3.2 Start playbook with: 
```bash
 ansible-playbook -i inventory.yml main.yml -vv
```

!!! Note: 
Make sure:
- Management server is reachable via 443
- API is running and allowed for automation server IP



### 4. References
Ansible CHKP Modules command reference:   
https://docs.ansible.com/ansible/latest/modules/list_of_network_modules.html#check-point

Ansible CHKP Modules galaxy documentation:     
https://galaxy.ansible.com/check_point/mgmt