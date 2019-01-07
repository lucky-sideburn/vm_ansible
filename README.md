# Ansible practices

## Vagrant project for getting fome practice with Ansible


### Using lists

task 'Basic Template Example'

### Using secrets

https://docs.ansible.com/ansible/latest/cli/ansible-vault.html#ansible-vault-encrypt-string

```
ansible-vault create myfile.txt
ansible-vault edit myfile.txt

```
se lo lanci senza specificare la password 

fatal: [kube-node]: FAILED! => {"msg": "A vault password or secret must be specified to decrypt /Users/eugenio/WORK/ansible/vm_ansible/playbooks/myfile.txt"}

```
ansible-playbook site.yml --ask-vault-pass
```

### Creating a Role

```
ansible-galaxy init provision/roles/hello_web
```
