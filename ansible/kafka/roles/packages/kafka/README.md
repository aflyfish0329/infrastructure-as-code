# Role Name
## kafka

## Table of contents
- [Role Name](#role-name)
  - [kafka](#kafka)
  - [Table of contents](#table-of-contents)
- [Usage](#usage)
- [Example Playbook](#example-playbook)
- [Example Inventory](#example-inventory)

# Usage
``` shell
export _INVENTORY=</path>/<to>/<inventory>
export _HN=<host_name>
export _PLAYBOOK=<path>/<to>/<playbook>

ansible-playbook -i ${_INVENTORY} -e "hn=${_HN}" ${_PLAYBOOK}
```

# Example Playbook
``` yaml
- hosts: '{{ hn }}'
  roles:
      - role: kafka
```

# Example Inventory
``` ini
[<groupname>]
<hostname> ansible_user=xxxx
<hostname> ansible_user=xxxx
<hostname> ansible_user=xxxx
```
