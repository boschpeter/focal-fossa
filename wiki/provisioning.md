## Focal fossa

|nr|Filesystem   |  ipadres                   | alias |  status|free| df -h|
|--|-------------|--------------------------- |-------|--------|----|--------|
|1 |raspberry   |  ssh ubuntu@192.168.2.17   | ub1   |pending |4GB|32GB|
|2 |raspberry   |  ssh ubuntu@192.168.2.18   | ub2   |pending |4GB|16GB|
|3 |raspberry   |  ssh ubuntu@192.168.2.21   | ub3   |pending |4GB|64GB|
|4 |hp          |  ssh ubuntu@192.168.2.61   | hp1   |pending |4GB|450GB|
|5 |vmWare      |  ssh ubuntu@192.168.2.16   | vm1   |pending |4GB|20G|
|6 |VirtualBox  |  ssh ubuntu@192.168.2.22   | vb1   |pending |4GB|24G|
|7 |OracleCloud |  ssh ubuntu@158.101.192.41 | oc1   |pending |10GB|45GB|

|8 Azure       |  | az1 | ..  | ..  |



## hosts

````
# ansible -i hosts vmware -m ping
# sudo apt-get install sshpass

[vmware]

# |nr|Filesystem   |  ipadres                   | alias |  status|free| df -h|
# |--|-------------|--------------------------- |-------|--------|----|--------|
# |1 |raspberry   |  ssh ubuntu@192.168.2.17   | ub1   |pending |4GB|32GB|
# |2 |raspberry   |  ssh ubuntu@192.168.2.18   | ub2   |pending |4GB|16GB|
# |3 |raspberry   |  ssh ubuntu@192.168.2.21   | ub3   |pending |4GB|64GB|
# |4 |hp          |  ssh ubuntu@192.168.2.61   | hp1   |pending |4GB|450GB|
# |5 |vmWare      |  ssh ubuntu@192.168.2.16   | vm1   |pending |4GB|20G|
# |6 |VirtualBox  |  ssh ubuntu@192.168.2.22   | vb1   |pending |4GB|24G|
# |7 |OracleCloud |  ssh ubuntu@158.101.192.41 | oc1   |pending |10GB|45GB|


192.168.2.17   ansible_user=ubuntu  #  ub1 
192.168.2.18   ansible_user=ubuntu  #  ub2
192.168.2.21   ansible_user=ubuntu  #  ub3
192.168.2.61   ansible_user=ubuntu  #  hp1
192.168.2.16   ansible_user=ubuntu  #  vm1
192.168.2.22   ansible_user=ubuntu  #  vb1
158.101.192.41 ansible_user=ubuntu  #  oc1

````

## boscp08@kubernetes-worker2:~/.../baremetal$ ansible -i hosts vmware -m ping
192.168.2.16 | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/bin/python3"
    },
    "changed": false,
    "ping": "pong"
}
192.168.2.22 | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/bin/python3"
    },
    "changed": false,
    "ping": "pong"
}
192.168.2.61 | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/bin/python3"
    },
    "changed": false,
    "ping": "pong"
}
192.168.2.18 | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/bin/python3"
    },
    "changed": false,
    "ping": "pong"
}
192.168.2.21 | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/bin/python3"
    },
    "changed": false,
    "ping": "pong"
}
192.168.2.17 | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/bin/python3"
    },
    "changed": false,
    "ping": "pong"
}
158.101.192.41 | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/bin/python3"
    },
    "changed": false,
    "ping": "pong"
