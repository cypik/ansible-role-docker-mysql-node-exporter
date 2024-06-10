<!-- This file was automatically generated by the `geine`. Make all changes to `README.yaml` and run `make readme` to rebuild this file. -->


<p align="center"> <img src="https://user-images.githubusercontent.com/50652676/62451340-ba925480-b78b-11e9-99f0-13a8a9cc0afa.png" width="100" height="100"></p>

<h1 align="center">
    Ansible Role Docker MySQL Node Exporter


</h1>

<p align="center" style="font-size: 1.2rem;">
    This ansible role is used to setup MySQL node exporter with docker.
     </p>

<p align="center">




</p>
<p align="center">



</p>
<hr>



We eat, drink, sleep and most importantly love **DevOps**. DevOps always promotes automation and standardisation. While setting up various environments like local, dev, testing, production, etc. it is critical to maintain the same environment across. This can easily be achieved using automating the environment setup & installation with the help of ansible-playbooks.

Smaller roles are created for each environment elements; which also include tasks & tests. These roles can then be grouped together in [ansible-playbook](https://docs.ansible.com/ansible/latest/user_guide/playbooks_intro.html) to achieve the desired yet consistent results.



## Prerequisites

This module has a few dependencies:

- [Ansible2.8](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)
- [Python](https://www.python.org/downloads)
- [Docker](https://docs.docker.com/install/linux/docker-ce/ubuntu)
- [MySQL](https://github.com/cypik/ansible-role-docker-mysql)




## What Includes

Following things includes in this role:

- mysql-node-exporter






## Example Playbook

**IMPORTANT:** Since the `master` branch used in `source` varies based on new modifications, we suggest that you use the release versions [here](https://github.com/cypik/ansible-role-docker-mysql-node-exporter/releases).


```yaml
- hosts: localhost
  remote_user: ubuntu
  become: true
  roles:
    - cypik.ansible_role_docker_mysql_node_exporter
```


## Variables

```yaml
  node_exporter_port: 9100
  mysql_root_password: "root_password"
  mysql_exporter_version: latest
  mysql_port: 3306
  mysql_database: "my_database"
  mysql_user: ""
  mysql_pass: ""
  mysql_custom_config:
    option1: value1
    option2: value2

```


## Installation

```console
  $ ansible-galaxy install cypik.ansible_role_docker_mysql_node_exporter
```


## About us

At [cypik][website], we offer expert guidance, implementation support and services to help organisations accelerate their journey to the cloud. Our services include docker and container orchestration, cloud migration and adoption, infrastructure automation, application modernisation and remediation, and performance engineering.

License
-------
This project is licensed under the MIT License - see the [LICENSE](https://github.com/cypik/ansible-role-docker-mysql-node-exporter/blob/master/LICENSE) file for details.
