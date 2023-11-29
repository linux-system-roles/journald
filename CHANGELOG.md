Changelog
=========

[1.1.0] - 2023-11-29
--------------------

### New Features

- feat: support for ostree systems (#46)

### Other Changes

- build(deps): Bump actions/checkout from 3 to 4 (#38)
- ci: ensure dependabot git commit message conforms to commitlint (#41)
- ci: tox-lsr version 3.1.1 (#45)

[1.0.6] - 2023-09-08
--------------------

### Other Changes

- ci: Add markdownlint, test_converting_readme, and build_docs workflows (#34)

  - markdownlint runs against README.md to avoid any issues with
    converting it to HTML
  - test_converting_readme converts README.md > HTML and uploads this test
    artifact to ensure that conversion works fine
  - build_docs converts README.md > HTML and pushes the result to the
    docs branch to publish dosc to GitHub pages site.
  - Fix markdown issues in README.md
  
  Signed-off-by: Sergei Petrosian <spetrosi@redhat.com>

- docs: Make badges consistent, run markdownlint on all .md files (#35)

  - Consistently generate badges for GH workflows in README RHELPLAN-146921
  - Run markdownlint on all .md files
  - Add custom-woke-action if not used already
  - Rename woke action to Woke for a pretty badge
  
  Signed-off-by: Sergei Petrosian <spetrosi@redhat.com>

- ci: Remove badges from README.md prior to converting to HTML (#36)

  - Remove thematic break after badges
  - Remove badges from README.md prior to converting to HTML
  
  Signed-off-by: Sergei Petrosian <spetrosi@redhat.com>


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
