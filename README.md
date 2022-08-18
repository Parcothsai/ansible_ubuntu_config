# Ansible for new computer on Ubuntu 22


## Requirements

Install ansible

```bash
python3 -m pip install --user ansible
```

## HOW TO USE

```bash
git clone https://github.com/Parcothsai/ansible_ubuntu_config.git
cd ansible_ubuntu_config
cp template_local.ini local.ini
```
Execute playbook

```bash

ansible-galaxy role install -r requirements.yml
ansible-playbook -i local.ini playbook.yml --diff -vv
```
