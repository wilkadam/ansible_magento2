# ansible_magento2
Playbook for deployment of Magento 2 stack

To install magento test environment you need to specify your variables in group_vars/all.yml and provide proper values in inventory file. Playbook was tested and designed for Ubuntu 20.04 LTS.

## Execution of playbook
To execute playbook you need to run:
```
ansible-playbook -i inventory main.yml
```
from your ansible controller. Execution of playbook can take around 25 minutes, depending of you Internet connection and machine capabilities.
Remember to add your public key to remote machine with:
```
ssh-copy-id <user>@IP
```
and add contents of your private key to id_rsa file.
