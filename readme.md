# ping target host from command line

ansible all -m ping

# examples to run playbook

ansible-playbook -i inv/hosts ping.yaml --check --ask-pass

# ansible playbook test run

ansible-playbook ping.yaml --check

# ---------------------------------

# Create Ansible Roles

ansible-galaxy init install
ansible-galaxy init configure
ansible-galaxy init runservice

# ansible playbook command to run main playbook which invokes ping.yaml

ansible-playbook site.yaml --check
ansible-playbook site.yaml

# VENV

python -m venv venv
source venv/bin/activate
