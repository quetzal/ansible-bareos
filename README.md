# ansible-bareos
Bareos client, dir, and storage configuration and management

I could not find an ansible-bareos job compatible with Bareos 16 so I do it myself. 

I like the project architecture from tiernap (https://github.com/tiernap/ansible-bareos/) so I use almost the same.

It's not perfect, but it work with bareos-webui (it install webui).

It deploys 1 director, 1 storage with local backup device and any number of clients. Modify roles/bareos-dir/templates/bareos-dir.d/ to change backup job definitions.
Il you add some file, add them to tasks. Change passwords in group_vars/all

It include bareos-xtrabackup plugin for mysql-like backups: https://github.com/bareos/bareos-contrib/tree/master/fd-plugins/bareos_percona
