# Ansible Role: MariaDB

Installs MariaDB, modified with https://github.com/geerlingguy/ansible-role-mysql

## Supported platforms

```
CentOS 6 & 7
Ubuntu 14.04
```

## Post install

Run `mysql_secure_installation`

## Requirements

None

## Role Variables

MariaDB version:

```
mariadb_version: 10.0
```

Configuration template:

```
mysql_conf_tpl: change_me
```

Configuration filename:

```
mysql_conf_file: settings.cnf
```

## Dependencies

None

## Example Playbook

```
- hosts: servers
  roles:
    - { role: pcextreme.mariadb }
```

## License

MIT / BSD

## Author Information

Created by [Attila van der Velde](https://github.com/vdvm).

Modified script is created by geerlingguy (https://github.com/geerlingguy/ansible-role-mysql)
