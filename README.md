# Ansible
# apt - package management system
ansible all -m ping
ansible linux_servers -a "python3 --version"
ansible linux_servers -m apt -a "update_cache=yes"
ansible-playbook web.yml
