# resolv

- GitHub: [![Build Status](https://travis-ci.org/hudecof/ansible_resolv.svg?branch=master)](https://travis-ci.org/hudecof/ansible_resolv)

This roles enables users to configure the /etc/resolv.conf. It will write also ansible facts file into ``/etc/ansible/facts.d/resolv.fact``


## Requirements

- ansible: 1.4

## Role Variables

See ``man resolv.conf`` for more informations.

- `resolv_file`: points to **/etc/resolv.conf**. Do not change until you know what are you doing.
- `resolv_domain`: **domain** in */etc/resolv.conf*, default is **null**
- `resolv_search`: **search** in */etc/resolv.conf*, default is **empty list**
- `resolv_nameserver`: **nameserver** in */etc/resolv.conf*, default is **Google Public DNS service**
- `resolv_sortlist`: **sortlist** in */etc/resolv.conf*, default is **empty list**
- `resolv_options`: **options** in */etc/resolv.conf*, default is **[rotate]**

## Dependencies

None

## Example Playbook

    - hosts: all
      roles:
        - role: hudecof.resolv


## License

BSD

## Author Information

Peter Hudec
