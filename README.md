# Publik virtual dev machine

See https://doc-publik.entrouvert.com/dev/installation-developpeur/

## Instructions

On host:

```
vagrant up && vagrant ssh
```

On guest:

```
git clone https://git.entrouvert.org/publik-devinst.git && cd publik-devinst
ansible-playbook -K -i inventory.yml install.yml
ansible-playbook -i inventory.yml deploy-tenants.yml
```
