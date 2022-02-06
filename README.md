# Ansible Role grub

Library of Ansible plugins and roles for deploying various services.
See [ansible-roles](https://github.com/davidfischer-ch/ansible-roles) for additional documentation.

This repository hosts the role grub and may depend of other roles and plugins of the library.

## Status

I only used it to fix Linux Mint not booting properly on an Asus ZenBook Pro!

## Dependencies

This role has no requirements.

## Variables

TODO VARIABLES

## Example

Any variable prefixed by grub_ will be converted to upper case and used for
configuring /etc/default/grub. Value is written verbatim, meaning you need
to add quotes for string parameters.

### PlayBook

```
---

- hosts:
    - localhost
  roles:
    - grub
  vars:
    grub_cmdline_linux_default: '"nouveau.modeset=0 quiet splash"'
```

## License

See [LICENSE.rst](LICENSE.rst).

## Authors

See [AUTHORS](AUTHORS).

2014-2022 - David Fischer
