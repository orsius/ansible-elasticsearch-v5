# Data-Essential - ansible - elasticsearch v5 - cluster setup (3 nodes with x-pack)
Simple Ansible Template to Install a 3 nodes elasticsearch(v5) cluster on centos7 (or rhel7)

## Requirements
The prerequisits are simples:
* have 3 centos7 servers ready to go with network already configure
* have ansible properly install on your workstation (with the ssh key setup on your 3 servers)

* [DE - blogpost ](https://www.data-essential.com/category/blog/)

## Technology included

* [Centos7](https://www.centos.org/download/), [RHEL7](https://access.redhat.com/downloads)
* [Ansible](http://docs.ansible.com/ansible/)
* [VirtualBox](https://www.virtualbox.org/)
* [Vagrant](https://www.vagrantup.com/docs/getting-started/)

* [Elasticsearch](https://www.elastic.co/guide/en/elasticsearch/reference/current/index.html)
* [Kibana](https://www.elastic.co/guide/en/kibana/current/index.html)


## Running

* Clone the repository.
* Change directory into the cloned project.
* Modify the host names in hosts file.

### Elasticsearch cluster
Run the following command.

```sh
$ PLAYBOOK=elasticsearch.yml

$ ansible-playbook ${PLAYBOOK}.yml --list-hosts
```
If all your servers respond you are ready to go and re-do the command withou the --list-hosts parameter.

Enjoy ;)

### Kibana
Complete this 3 nodes cluster with a kibana server

```sh
$ PLAYBOOK=kibana.yml
$ ansible-playbook ${PLAYBOOK}.yml --list-hosts
```

## information

More information can be found on our blog
* [DE - blogpost ](https://www.data-essential.com/category/blog/)
