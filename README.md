# general

This is a ansible role to upgrade your [gitea](https://github.com/go-gitea/gitea) to the latest version. First a backup is done ([docs](https://docs.gitea.io/en-us/backup-and-restore/)) to have a fallback, after that the upgrade is done. The previous version of the gitea binary is stored as `gitea.old`. Finally there is an healthcheck to check if the server is up an running again.

The role was developed on [Raspbian](https://raspbian.org/), but should run on every Debian based system. The used ansible version was 2.8.4, the used gitea version v1.9.2.

# how to use

1. change the variables in the inventory/group_vars/gitea file.
2. change the inventory/hosts file

After that you can run it with the command `ansible-playbook playbooks/nextcloud.yml`


