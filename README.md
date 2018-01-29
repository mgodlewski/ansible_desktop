# ansible_desktop
Ansible role to install and configure my favorite tools for my destop computer:
- git
- bash preference (history shortcuts)
- nemo (file manager)
- i3 (coming)


Sample playbook:

``` yaml
- hosts: localhost
  roles:
   - role: ansible_desktop
     git_email: john.doe@inter.net
     git_name: John Doe
     git_signingkey: XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
```

Ansible run:
``` shell
ansible-playbook -i localhost, -c local playbook.yml --diff -K
```

