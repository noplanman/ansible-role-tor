# Ansible Role: Tor

[![build-status-badge]][build-status]

Installs [Tor] on a RedHat or Debian-based linux system.

## Requirements

None.

## Dependencies

None.

## Role Variables

See [`defaults/main.yml`](defaults/main.yml) for all available variables.

## Example Playbook

    - hosts: servers
      vars_files:
        - vars/main.yml
      roles:
        - noplanman.tor

*Inside `vars/main.yml`*:

    tor_http_port: "8080"

## License

MIT

[build-status-badge]: https://img.shields.io/travis/noplanman/ansible-role-tor.svg
[build-status]: https://travis-ci.org/noplanman/ansible-role-tor "Build status on Travis-CI"

[Tor]: https://www.torproject.org/
