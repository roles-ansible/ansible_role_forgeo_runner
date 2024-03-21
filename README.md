[![Ansible Galaxy](https://ansible.l3d.space/svg/roles-ansible.forgeo_runner.svg)](https://galaxy.ansible.com/ui/standalone/roles/roles-ansible/forgeo_runner/)
[![BSD-3 Clause](https://ansible.l3d.space/svg/roles-ansible.forgeo_runner_license.svg)](LICENSE)
[![Maintainance](https://ansible.l3d.space/svg/roles-ansible.forgeo_runner_maintainance.svg)](https://ansible.l3d.space/#roles-ansible.forgeo_runner)

 ansible role forgeo_runner
=======================
Ansible role to install and Setup forgeo runner.

Visit [code.forgejo.org/forgejo/runner](https://code.forgejo.org/forgejo/runner) for more information about forgejo actions.

 Requirements
--------------

This role requires either to be able to start docker containers as ``forgejo_runner`` User or you change the ``forgejo_runner__mode`` variable to run actions directly without containerisation which could break your system.

 Variables
-----------
| Variable | Value | Description |
| -------- | ----- | ----------- |
| ``forgejo_runner__version`` | ``latest`` | Forgejo runner version or latest to use latest |
| ``forgejo_runner__user`` | ``forgejo_runner`` | Forejo runner UNIX User |
| ``forgejo_runner__group`` | ``forgejo_runner`` | Forgejo runner UNIX Group |
| ``forgejo_runner__user_home`` | ``/var/lib/forgejo-runner`` | Unix Home and working directory |
| ``forgejo_runner__full_executable_path`` | ``/usr/local/bin/forgejo_runner`` | Path for executable binary |
| ``forgejo_runner__gpg_id`` | ``EB114F5E6C0DC2BCDD183550A4B61A2DC5923710`` | Forgejo runneer GPG Key |
| ``forgejo_runner__instance_address`` | | Forgejo Instance Address |
| ``forgejo_runner__token`` | | Token for runner of your forgejo instance |
| ``forgejo_runner__mode`` | ``daemon`` | Forgejo runner mode. Change to ``exec`` for local Runner execution |
| ``submodules_versioncheck`` | ``false`` | optional simple version check |

 Contribution
--------------
Please feel free to open an issue or Pull-Request
