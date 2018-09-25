# Ansible Role: Tor

[![Build Status][travis-build-status]][travis-tests] [![Ansible Role][ansible-role-shield]][ansible-role]

---

:rocket: Development has moved to **[git.feneas.org]**.

(The repository on GitHub is only a mirror, so fork on Feneas to contribute. No registration needed, just sign in with your GitHub account.)

---

This role installs [Tor] on a RedHat or Debian-based linux system.

## Requirements

None.

## Dependencies

None.

## Role Variables

See [`defaults/main.yml`][defaults] for all available variables.

## Example Playbook

    - hosts: servers
      vars_files:
        - vars/main.yml
      roles:
        - noplanman.tor

*Inside `vars/main.yml`*:

    tor_http_port: "8080"

## Tests

Docker is used to test the role with different operating systems.

Check the [`tests`] folder.

## License

MIT

[travis-build-status]: https://img.shields.io/travis/noplanman/ansible-role-tor.svg?style=flat-square "Travis-CI Build Status"
[travis-tests]: https://travis-ci.org/noplanman/ansible-role-tor "Travis-CI Tests"
[ansible-role-shield]: https://img.shields.io/ansible/role/21806.svg?style=flat-square "Tor on Ansible Galaxy"
[ansible-role]: https://galaxy.ansible.com/noplanman/tor "Tor on Ansible Galaxy"
[git.feneas.org]: https://git.feneas.org/noplanman/ansible-role-tor "Ansible Role Tor on Feneas"
[Tor]: https://www.torproject.org/ "Tor Project"
[defaults]: https://git.feneas.org/noplanman/ansible-role-tor/blob/master/defaults/main.yml "Default variables"
[`tests`]: https://git.feneas.org/noplanman/ansible-role-tor/tree/master/tests "Tests"
