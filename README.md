# Run it this way
ansible-playbook -i inventory/hosts.ini --extra-vars "ansible_ssh_user=userHere ansible_ssh_pass=passHere ansible_sudo_pass=sudoPassHere" basicConfiguration.yml