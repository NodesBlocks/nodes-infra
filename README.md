## Note

> :info: We didn't have intention to make this repo reusable for everyone.</br>
> It's just an example part of our infrastructure and scripts which we use to speed up our node management and to control configuration changes.

To start you have to configure following things:

1. Add `inventory.yaml`
   This file contain list of your nodes / group nodes and some global variables for them.
   There is `inventory.yaml.example` which you can use as example.
2. Add secret varaibles to `group_vars/` directory.
   There is an example in file `all.yaml.example`
3. Change moniker, wallet address, valoper address and other variables in manifests if it is necessary.

> :info: `inventory.yaml` and `group_vars/.yaml` added to gitignore you feel free to keep them in your folder and do not worry about accidentally adding them to the repository

Some directories contains own README.md with some cheatsheets how to use this manifests.

## Repository content

In our configurations we mostly use ansible and docker.
We have already tried to use nomad to as workload management system but decided not to use it and looking closely to cheap k8s providers.

If you have any suggesstions how to substitute ansible we are glad to hear it in chats/issues/PR's

`ansible/cosmos-mainnets` - our mainnet nodes and their configurations
`ansible/monitoring` - our monitoring stack
