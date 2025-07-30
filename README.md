# Sudoers automation with ansible

## Installation steps

- Go to you ansible project folder
- Add following to your requirements file

```
- src: https://github.com/PHKA-ZIM/ansible-role-sudoers
  name: ansible-role-sudoers
```

- Install to project roles path
```
ansible-galaxy install -r requirements.yml --roles-path ./roles
```

## Use ansible-role-sudoers

- Import role and override role variables, e.g.
```
- name: Configure sudo
  roles:
    - role: ansible-role-sudoers
```
