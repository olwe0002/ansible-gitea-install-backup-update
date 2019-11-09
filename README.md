# general

This is a ansible role to instll and upgrade your [gitea](https://github.com/go-gitea/gitea) to the latest version. First a backup is done ([docs](https://docs.gitea.io/en-us/backup-and-restore/)) to have a fallback, after that the upgrade is done. The previous version of the gitea binary is stored as. Finally there is an healthcheck to check if the server is up an running again.
Additionally a cron job creates a database backup every night.

The role was developed on [Raspbian](https://raspbian.org/), but should run on every Debian based system. 

# how to use

1. change the variables in the inventory/group_vars/{gitea,all} files.
2. change the inventory/hosts file

After that you can run it with the command `ansible-playbook playbooks/gitea.yml`


