# VENV

python -m venv venv
source venv/bin/activate

# ping target host from command line

ansible all -m ping

# examples to run playbook

ansible-playbook -i env/hosts ping.yaml --check --ask-pass

# ansible playbook test run

ansible-playbook ping.yaml --check

# ansible playbook command to run main playbook which invokes ping.yaml

ansible-playbook site.yaml

# finally ansible playbook to run nginx

ansible-playbook nginx.yaml
