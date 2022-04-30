# How to set it up the environment
- Comment this line in ansible.cfg file:
```
vault_password_file = ./vault/.key
```
- Now you need to generate a file to be used as vault id.
```
mkdir ./vault
echo "put some content here" > ./vault/.key
```
- Generate a encrypt a value using be key file created above (run this command to encrypt each value)
```
ansible-vault encrypt_string "putHereTheContentToBeEncrypted" --vault-id crypt@./vault/.key
```
- To ended, just copy the encrypt value and replace it in hosts.yml.

# Run it this way
All the extra informations must be set in ansible.cfg, so to call the playbook you just must run this command:
```
ansible-playbook basicConfiguration.yml
```

# Ansible references
[Encrypting content](https://docs.ansible.com/ansible/latest/user_guide/vault.html)
[Configuration file](https://docs.ansible.com/ansible/2.4/intro_configuration.html#vault-password-file)
[Ansible course](https://ambevtech.udemy.com/course/ultimate-ansible-bootcamp)