```
cd ansible
```

### First init

```
ansible-playbook cosmos-mainnets/canto/canto.yaml \
 --extra-vars="target=cosmosMainnets" \
 --extra-vars="init=True" \
 --extra-vars="rebuild=True" \
 --diff --check
```

### Download genesis and set config values

```
ansible-playbook cosmos-mainnets/canto/canto.yaml \
 --extra-vars="target=cosmosMainnets" \
 --extra-vars="config=True" \
 --diff --check
```

### Run node

```
ansible-playbook cosmos-mainnets/canto/canto.yaml \
 --extra-vars="target=cosmosMainnets" \
 --extra-vars="run_node=True" \
 --diff --check
```

### Upgrade

```
ansible-playbook cosmos-mainnets/canto/canto.yaml \
 --extra-vars="target=cosmosMainnets" \
 --extra-vars="rebuild=True" \
 --diff --check
```
