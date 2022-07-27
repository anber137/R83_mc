```
root@debian:/home/R83_java# ansible-playbook site.yml                                              
[WARNING]: Found both group and host with same name: ubuntu

PLAY [all] ***************************************************************************************************************************

TASK [Gathering Facts] ***************************************************************************************************************
[WARNING]: The "docker" connection plugin has an improperly configured remote target value, forcing "inventory_hostname" templated
value instead of the string
[WARNING]: The "docker" connection plugin has an improperly configured remote target value, forcing "inventory_hostname" templated
value instead of the string
ok: [ubuntu]
ok: [centos7]

TASK [mnt-homeworks-ansible : Upload .tar.gz file containing binaries from local storage] ********************************************
skipping: [ubuntu]
skipping: [centos7]

TASK [mnt-homeworks-ansible : Upload .tar.gz file conaining binaries from remote storage] ********************************************
[WARNING]: The "docker" connection plugin has an improperly configured remote target value, forcing "inventory_hostname" templated
value instead of the string
[WARNING]: The "docker" connection plugin has an improperly configured remote target value, forcing "inventory_hostname" templated
value instead of the string
changed: [ubuntu]
changed: [centos7]

TASK [mnt-homeworks-ansible : Ensure installation dir exists] ************************************************************************
[WARNING]: The "docker" connection plugin has an improperly configured remote target value, forcing "inventory_hostname" templated
value instead of the string
[WARNING]: The "docker" connection plugin has an improperly configured remote target value, forcing "inventory_hostname" templated
value instead of the string
changed: [centos7]
changed: [ubuntu]

TASK [mnt-homeworks-ansible : Extract java in the installation directory] ************************************************************
[WARNING]: The "docker" connection plugin has an improperly configured remote target value, forcing "inventory_hostname" templated
value instead of the string
[WARNING]: The "docker" connection plugin has an improperly configured remote target value, forcing "inventory_hostname" templated
value instead of the string
changed: [ubuntu]
changed: [centos7]

TASK [mnt-homeworks-ansible : Export environment variables] **************************************************************************
[WARNING]: The "docker" connection plugin has an improperly configured remote target value, forcing "inventory_hostname" templated
value instead of the string
[WARNING]: The "docker" connection plugin has an improperly configured remote target value, forcing "inventory_hostname" templated
value instead of the string
changed: [centos7]
changed: [ubuntu]

PLAY RECAP ***************************************************************************************************************************
centos7                    : ok=5    changed=4    unreachable=0    failed=0    skipped=1    rescued=0    ignored=0   
ubuntu                     : ok=5    changed=4    unreachable=0    failed=0    skipped=1    rescued=0    ignored=0   
```
