# ansible-bareos
Bareos client, dir, and storage configuration and management

I could not find an ansible-bareos job compatible with Bareos 16 so I do it myself. 

I like the project architecture from tiernap (https://github.com/tiernap/ansible-bareos/) so I use almost the same.

It's not perfect, but it work with bareos-webui.



It deploys 1 director, 1 storage with local backup device and any number of clients. Modify roles/bareos-dir/templates/bareos-dir.conf to change backup job definitions. Change passwords in group_vars/all
