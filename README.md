# Ansible for new computer on Ubuntu 22


## Requirements

Install ansible

```bash
python3 -m pip install --user ansible
```

Install roles

```bash
ansible-galaxy role install -r requirements.yml
```

Change template_local.ini -> local.ini and update informations

Execute playbook

```bash
ansible-playbook -i local.ini playbook.yml --diff -vv --ask-become-pass
```
