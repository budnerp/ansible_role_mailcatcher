# Ansible role for MailCatcher 
Ansible role for MailCatcher 0.7.1 installation for CentOS 7.
Catches mail and serves it through a dream.

## What's inside?
- MailCatcher 0.7.1
- SMPT host `http://{{ansible_nodename}}:1025/`
- Web interface `http://{{ansible_nodename}}:1080/`
- Dependencies:
    - Gem 2.0

##Interesting PHP dirs and files 
```
/var/log/mailcatcher.log
```
   
## Tested on

## Installation
1. Navigate to Ansible's roles folder
2. Add the repo to git modules
    ```
    git submodule add https://github.com/budnerp/ansible_role_mailcatcher.git ansible_role_mailcatcher
    ```
3. Add the role to Ansible's playbook file
    ```    
    roles:
    [...]
        - ansible_role_mailcatcher
    [...]
    ```

## Other links
- MailCatcher [https://mailcatcher.me/]()

## TO DO
-[ ] add dependencies

## License
Copyright (c) We Are Interactive under the MIT license.