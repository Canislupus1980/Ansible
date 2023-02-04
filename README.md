# Ansible
# apt - package management

ansible all -m ping

ansible linux_servers -a "python3 --version"

ansible linux_servers -m apt -a "update_cache=yes"

#http

ansible-playbook web.yml

#https

cd playbooks/files

openssl req -x509 -nodes -days 3650 -newkey rsa:2048 -subj /CN=localhost -keyout nginx.key -out nginx.crt

ansible-playbook web-tls.yml
