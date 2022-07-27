```
PLAY [Destroy] *****************************************************************

TASK [Destroy molecule instance(s)] ********************************************
[33mchanged: [localhost] => (item=ubuntu)[0m

TASK [Wait for instance(s) deletion to complete] *******************************
[32mok: [localhost] => (item=ubuntu)[0m

TASK [Delete docker networks(s)] ***********************************************

PLAY RECAP *********************************************************************
[33mlocalhost[0m                  : [32mok=2   [0m [33mchanged=1   [0m unreachable=0    failed=0    [36mskipped=1   [0m rescued=0    ignored=0


PLAY [Create] ******************************************************************

TASK [Log into a Docker registry] **********************************************
[36mskipping: [localhost] => (item=None) [0m
[36mskipping: [localhost][0m

TASK [Check presence of custom Dockerfiles] ************************************
[32mok: [localhost] => (item={'image': 'pycontribs/ubuntu:latest', 'name': 'ubuntu', 'pre_build_image': True})[0m

TASK [Create Dockerfiles from image names] *************************************
[36mskipping: [localhost] => (item={'image': 'pycontribs/ubuntu:latest', 'name': 'ubuntu', 'pre_build_image': True}) [0m

TASK [Discover local Docker images] ********************************************
[32mok: [localhost] => (item={'changed': False, 'skipped': True, 'skip_reason': 'Conditional result was False', 'item': {'image': 'pycontribs/ubuntu:latest', 'name': 'ubuntu', 'pre_build_image': True}, 'ansible_loop_var': 'item', 'i': 0, 'ansible_index_var': 'i'})[0m

TASK [Build an Ansible compatible image (new)] *********************************
[36mskipping: [localhost] => (item=molecule_local/pycontribs/ubuntu:latest) [0m

TASK [Create docker network(s)] ************************************************

TASK [Determine the CMD directives] ********************************************
[32mok: [localhost] => (item={'image': 'pycontribs/ubuntu:latest', 'name': 'ubuntu', 'pre_build_image': True})[0m

TASK [Create molecule instance(s)] *********************************************
[33mchanged: [localhost] => (item=ubuntu)[0m

TASK [Wait for instance(s) creation to complete] *******************************
[1;30mFAILED - RETRYING: [localhost]: Wait for instance(s) creation to complete (300 retries left).[0m
[33mchanged: [localhost] => (item={'failed': 0, 'started': 1, 'finished': 0, 'ansible_job_id': '117785625208.3261548', 'results_file': '/root/.ansible_async/117785625208.3261548', 'changed': True, 'item': {'image': 'pycontribs/ubuntu:latest', 'name': 'ubuntu', 'pre_build_image': True}, 'ansible_loop_var': 'item'})[0m

PLAY RECAP *********************************************************************
[33mlocalhost[0m                  : [32mok=5   [0m [33mchanged=2   [0m unreachable=0    failed=0    [36mskipped=4   [0m rescued=0    ignored=0


PLAY [Converge] ****************************************************************

TASK [Gathering Facts] *********************************************************
[32mok: [ubuntu][0m

TASK [Include mc] **************************************************************

TASK [mc : Install mc] *********************************************************
[33mchanged: [ubuntu][0m

PLAY RECAP *********************************************************************
[33mubuntu[0m                     : [32mok=2   [0m [33mchanged=1   [0m unreachable=0    failed=0    skipped=0    rescued=0    ignored=0


PLAY [Verify] ******************************************************************

TASK [Check mc version] ********************************************************
[32mok: [ubuntu][0m

PLAY RECAP *********************************************************************
[32mubuntu[0m                     : [32mok=1   [0m changed=0    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0


PLAY [Destroy] *****************************************************************

TASK [Destroy molecule instance(s)] ********************************************
[33mchanged: [localhost] => (item=ubuntu)[0m

TASK [Wait for instance(s) deletion to complete] *******************************
[1;30mFAILED - RETRYING: [localhost]: Wait for instance(s) deletion to complete (300 retries left).[0m
[33mchanged: [localhost] => (item=ubuntu)[0m

TASK [Delete docker networks(s)] ***********************************************

PLAY RECAP *********************************************************************
[33mlocalhost[0m                  : [32mok=2   [0m [33mchanged=2   [0m unreachable=0    failed=0    [36mskipped=1   [0m rescued=0    ignored=0
```
