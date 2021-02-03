
# VENV
python -m venv venv
source venv/bin/activate

# ping target host from command line
ansible all -m ping

# examples to run playbook
ansible-playbook -i env/hosts ping.yml --check --ask-pass

# ansible playbook test run
ansible-playbook ping.yml --check

ansible-playbook playbook1.yml 

