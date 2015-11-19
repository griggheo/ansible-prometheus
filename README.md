Ansible-Prometheus
=========

Installs the Prometheus monitoring server and the node_exporter binary and runs them as Upstart services.

Role Variables
--------------

```yml
prometheus_version: 0.16.1
node_exporter_version: 0.12.0rc1
prometheus_root_dir: /opt/prometheus
prometheus_config_dir: /etc/prometheus
prometheus_server_dir: "{{ prometheus_root_dir }}/prometheus-server"
prometheus_bin_dir: "{{ prometheus_root_dir }}/bin"
prometheus_dist_dir: "{{ prometheus_root_dir }}/dist"
prometheus_db_dir: "{{ prometheus_root_dir }}/databases"
prometheus_host_domain_name: example.com
```

Example Playbook Role Usage
----------------

## Simple setup

Install and run Prometheus and node_exporter using Upstart.

```yml
roles:
    - { role: ansible-prometheus }
```


License
-------

Apache v2.0

Author Information
------------------

Grig Gheorghiu
http://agiletesting.blogspot.com
