Role Name
=========

Consul is a tool for discovering and configuring services in your infrastructure. It provides several key features:
	

    1. *Service Discovery*: Clients of Consul can provide a service using DNS or HTTP.

    2. *Health Checking*: Consul clients can provide any number of health checks with services or node

    3. *Key/Value Store*: Applications can make use of Consul's hierarchical key/value store for dynamic configuration.

    4. *Multi Datacenter*: Consul supports multiple datacenters out of the box. This means users of Consul do not have to worry about building additional layers of abstraction to grow to multiple regions.


Requirements
------------
1. Ansible need to be installed
2. Clester of nodes and it's hostname shoud get entry into your inventory file

Role Variables
--------------

default variables: (can be changed while running playbook)

1. unzip_version: "6.0*"
2. consul_binary_link: "https://releases.hashicorp.com/consul/0.6.4/consul_0.6.4_linux_amd64.zip"

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: prabhuvignesh.consul_installer, x: 42 }

License
-------

opensource

Author Information
------------------

..*Prabhu Vignesh Kumar Rajagopal
..*http://prabhuvignesh.github.io
