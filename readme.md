# Ansible Kafka Playbook

Ansible role for [Apache Kafka](https://kafka.apache.org/).

Before working with this playbook, you must install ansible.

```sh
$ virtualenv --python=`which python3` ~/.ansible_env
$ source ~/.ansible_env/bin/activate
$ pip install ansible
(.ansible_env) $ # Your're good to go...
```

## Installing & Configuring

### Clone this repository.
```sh
(.ansible_env) $ git clone https://github.com/rajuthapa8086/ansible-kafka-playbook.git
```

### `cd` into the directory.
```sh
(.ansible_env) $ cd ansible-kafka-playbook.git
```

### Adding inventory file.
```sh
(.ansible_env) $ cp ./inventory.dist ./inventory
```

### Adding group_vars file.
```sh
(.ansible_env) $ cp ./group_vars/all.dist ./group_vars/all
```

Edit both files.

## Running
```sh
(.ansible_env) $ ansible-playbook -i inventory kafka.yml
```
