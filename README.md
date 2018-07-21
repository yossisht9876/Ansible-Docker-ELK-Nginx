# Ansible-Docker-ELK-Nginx
ansible playbook for deploying stack of ELK + Filebeat + Nginx

This playbook will install and run a ELK + Filebeat + Nginx using Docker containers.

Filebeat will collect docker logs and transfer it to Logstash.
Logstash will store them on in an index on Elasticsearch.
Kibana will be able to quiry the logs.
Nginx will protect Kibana with basic authentication.



usage :

clone the folder to your host
from the project working directory run :

ansible-playbook main.yaml

*dont forget to change the working directory path on the configuration files in oredr to match yours

