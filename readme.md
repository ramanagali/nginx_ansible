# ping target hosts

ansible all -m ping

# ansbile raw

ansible -i hosts mac --list-hosts
ansible -i hosts all -m raw -a 'echo "Hello GVR"'

# examples to run/test playbook

ansible-playbook -i inv/hosts ping.yaml --check
ansible-playbook -i inv/hosts ping.yaml --check --ask-pass
ansible-playbook ping.yaml --check

# ---------------------------------

# Create Ansible Roles

ansible-galaxy init configure
ansible-galaxy init runservice

# ansible playbook command to run main playbook which invokes ping.yaml

ansible-playbook site.yaml --check
ansible-playbook site.yaml

# VENV

python3 -m venv venv
source venv/bin/activate
