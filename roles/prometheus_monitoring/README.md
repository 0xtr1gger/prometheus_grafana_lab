Prometheus, Grafana, Node Exporter, and Alertmanager setup
=========

This role is used to automatically set up Prometheus server, Grafama, Node Exporter, and Alertmanager Docker containers on a Linux machine. Docker Compose is used to orchestrate the containers.

Dependencies
------------

- [`community.docker`](https://docs.ansible.com/ansible/latest/collections/community/docker/index.html)

Role Variables
--------------

|Variable|Description|Default Value|
|-|-|-|
|api_directory|The directory created on the target machine where the configuration files will be copied.|`/app`|
|slack_url|The Slack webhook URL| |


Example Playbook
----------------

```YAML
---
- name: VM setup
  hosts: all
  become: true
  roles:
    - prometheus_monitoring
```

License
-------

BSD

Author Information
------------------

[0xtr1gger](https://github.com/0xtr1gger)
