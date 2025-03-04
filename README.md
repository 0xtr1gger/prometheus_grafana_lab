# Prometheus & Grafana lab

This repository contains configuration files and an Ansible role necessary to set up a monitoring infrastructure with a Prometheus server, Grafana, Node Exporter, and Alertmanager in Docker containers. The containers are orchestrated with Docker Compose that mounts configuration files and maps ports from containers to host. 

Here is the structure of the project:

![prometheus_grafana_lab](https://github.com/user-attachments/assets/8dd90b91-6d45-4104-8367-c751f83059f9)


```
.  
├── alertmanager  
│   └── alertmanager.yml  
├── docker-compose.yml  
├── playbook.yml  
├── prometheus  
│   ├── alertrules.yml  
│   ├── prometheus.yml  
│   └── targets.json  
├── README.md  
└── roles  
   ├── install_docker  
   └── prometheus_monitoring
```

To launch this lab, run the following command:

```bash
docker-compose up -p
```
