```
cd ansible
```

### Install

```
ansible-playbook monitoring/monitoring.yaml \
 --extra-vars="target=monitoring" \
 --diff --check
```
