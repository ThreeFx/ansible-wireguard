wireguard
=========

Role to set up wireguard on Debian systems.

Note that for Debians systems until buster you have to enable at least testing
(Codename: bullseye) repositories, since wireguard is only packaged for bullseye
and later. See [this role](https://github.com/ThreeFx/apt) for an Ansible role
for this.

Requirements
------------

A Debian bullseye or newer system, or, equivalently, access to bullseye or newer
packages.

Role Variables
--------------

| Variable Name | Default Value | Description |
--------------- |---------------|--------------
`wireguard_enable_ip_forwarding` | False | Whether to enable ip forwarding.
`wireguard_apt_release` | "testing" | Apt release to install wireguard from.
`wireguard_configurations` | [] | See `defaults/main.yml` for more information.

Dependencies
------------

None.

Example Playbook
----------------

See `molecule/default/playbook.yml`.

License
-------

BSD

Author Information
------------------

Find me on [GitHub](https://github.com/ThreeFx).
