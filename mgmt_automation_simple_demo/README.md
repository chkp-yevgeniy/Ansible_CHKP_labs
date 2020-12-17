# Very simple demo to start with Check Point Management automation.

### 1. Purpose
These role has a very simple example on how to create an object in an MDS CMA.


Following CheckPoint Ansible modules are used:
https://galaxy.ansible.com/check_point/mgmt

The modules (and therefore this role) are idempotent which is great! 

Modules are documented in: 
https://docs.ansible.com/ansible/latest/modules/list_of_network_modules.html#check-point


### 2. Requirements
- Ansible 2.9 (latest)
- Python 2.7 (latest)
- Install modules:
- https://galaxy.ansible.com/check_point/mgmt


### 3. How to run the role 
To get started with the automation you might want to test a very simple playbook in:
```bash
 playbooks/mgmt_automation_simple_demo/
```

3.1 Adjust inventory to your needs
```bash
 verySimpleDemoInventory.yml
```

3.2 Start playbook with: 
```bash
 ansible-playbook -i demo_inventory.yml mgmt_automation_simple_demo.yml -v
```

!!! Note: 
Make sure:
- Management server is reachable via 443
- API is running and allowed for automation server IP
