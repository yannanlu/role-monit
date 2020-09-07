# role-monit
Ansible role for Monit

In order to use this role, some of the variables are required to be specified or defined, such as **monit_key_secret**. For other variables, please overwrite them as your needs.

| Name                         | Value                        | Description                       | File              |
| ---                          | ---                          | ---                               | ---               |
| monit_port                   | 2812                         | port of monit                     | defaults/main.yml |
| monit_user                   | monit                        | username of the installation      | defaults/main.yml |
| monit_passwd                 | monit                        | password for the user             | defaults/main.yml |
| monit_pemfile                | ''                           | keypair file for SSL              | defaults/main.yml |
| monit_key_secret             | xxxx                         | secret of keypair file            | defaults/main.yml |
| monit_dir                    | /etc                         | directory for configs             | defaults/main.yml |
| monit_includedir             | /etc/monit.d                 | directory for included configs    | defaults/main.yml |
| monit_idfile                 | /var/.monit.id               | id file of monit                  | defaults/main.yml |
| monit_statefile              | /var/.monit.state            | state file of monit               | defaults/main.yml |
| monit_os_release_file        | /etc/redhat-release          | release file of OS                | defaults/main.yml |
| monit_pkg_name               | monit                        | name of monit package             | defaults/main.yml |
| monit_pkg_version            | 5.25.1-1.el7                 | version of monit package          | defaults/main.yml |
| monit_allow_list             | [...]                        | list of IPs and hostnames         | defaults/main.yml |
| monit_extra_allow_list       | []                           | list of extra IPs and hostnames   | defaults/main.yml |

## Status

Tested on images of RHEL 7.3 with either Ansible Core 2.6.

## See Also
* [Ansible Docs] (http://docs.ansible.com)
