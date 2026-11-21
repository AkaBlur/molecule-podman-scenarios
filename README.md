# Molecule Podman Scenarios

Collection of all tested basic scenarios for Ansible development.

Uses regular *podman containers* for Ansible testing with an active *systemd*
initialization process.

## Scenarios (active)

### RedHat

- AlmaLinux 9
- AlmaLinux 10

- CentOS Stream 9
- CentOS Stream 10

## Debian

- Debian 12
- Debian 13

- Ubuntu 22.04
- Ubuntu 24.04
- Ubuntu 26.04

> [!info]
> Ubuntu 22.04 disables the default systemd-resolved DNS daemon to free up port
> 53 on the test instance.

## Setup

Testing setup is done using the
[Ansible-native](https://docs.ansible.com/projects/molecule/ansible-native/)
approach for Molecule testing. It utilizes regular Ansible inventory,
collections and requirements to form a complete test setup for the specified
scenario.

All scenarios are configured from the default scenario and only adapted for
specific system changes.

Tests are inluced from the tested instances themselves (inside roles,
playbooks, etc.).
