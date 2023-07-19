Changelog
=========

[1.0.5] - 2023-07-19
--------------------

### Bug Fixes

- fix: facts being gathered unnecessarily (#31)

### Other Changes

- ci: Add pull request template and run commitlint on PR title only (#28)
- ci: Rename commitlint to PR title Lint, echo PR titles from env var (#29)
- ci: ansible-lint - ignore var-naming[no-role-prefix] (#30)

[1.0.4] - 2023-05-26
--------------------

### Other Changes

- docs: Consistent contributing.md for all roles - allow role specific contributing.md section
- docs: use None for Requirements

[1.0.3] - 2023-04-27
--------------------

### Other Changes

- test: check generated files for ansible_managed, fingerprint
- ci: Add commitlint GitHub action to ensure conventional commits with feedback

[1.0.2] - 2023-04-13
--------------------

### Other Changes

- add pipefail for shell commands (#18)

[1.0.1] - 2023-04-06
--------------------

### Other Changes

- Add README-ansible.md to refer Ansible intro page on linux-system-roles.github.io (#15)
- Fingerprint RHEL System Role managed config files (#16)

[1.0.0] - 2023-01-27
--------------------

### New Features

- initial version - manage systemd-journald

### Bug Fixes

- none

### Other Changes

- none
