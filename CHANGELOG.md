Changelog
=========

[1.3.5] - 2025-01-09
--------------------

### Other Changes

- ci: Use Fedora 41, drop Fedora 39 (#91)
- ci: Use Fedora 41, drop Fedora 39 - part two (#92)

[1.3.4] - 2024-10-30
--------------------

### Other Changes

- ci: Add tags to TF workflow, allow more [citest bad] formats (#84)
- ci: ansible-test action now requires ansible-core version (#85)
- ci: add YAML header to github action workflow files (#86)
- refactor: Use vars/RedHat_N.yml symlink for CentOS, Rocky, Alma wherever possible (#88)
- test: disable service start limit to avoid errors during testing (#89)

[1.3.3] - 2024-08-19
--------------------

### Other Changes

- ci: Add tft plan and workflow (#75)
- ci: Update fmf plan to add a separate job to prepare managed nodes (#77)
- ci: Bump sclorg/testing-farm-as-github-action from 2 to 3 (#78)
- ci: Add workflow for ci_test bad, use remote fmf plan (#79)
- ci: Fix missing slash in ARTIFACTS_URL (#80)
- test: fix check for max journal size (#81)

[1.3.2] - 2024-07-02
--------------------

### Bug Fixes

- fix: add support for EL10 (#73)

### Other Changes

- ci: ansible-lint action now requires absolute directory (#72)

[1.3.1] - 2024-06-11
--------------------

### Other Changes

- ci: use tox-lsr 3.3.0 which uses ansible-test 2.17 (#67)
- ci: tox-lsr 3.4.0 - fix py27 tests; move other checks to py310 (#69)
- ci: Add supported_ansible_also to .ansible-lint (#70)

[1.3.0] - 2024-04-04
--------------------

### New Features

- feat: Add options for rate limit interval and burst (#64)

### Other Changes

- ci: fix python unit test - copy pytest config to tests/unit (#62)
- ci: Bump ansible/ansible-lint from 6 to 24 (#63)
- ci: Bump mathieudutour/github-tag-action from 6.1 to 6.2 (#65)

[1.2.3] - 2024-01-23
--------------------

### Other Changes

- refactor: improve template formatting (#60)

[1.2.2] - 2024-01-16
--------------------

### Bug Fixes

- fix: Compress applies to all storage modes, SyncInterval only to persistent (#58)

[1.2.1] - 2024-01-10
--------------------

### Bug Fixes

- fix: ForwardToSyslog only set for volatile (#56)

[1.2.0] - 2024-01-09
--------------------

### New Features

- feat: Adding support for ForwardToSyslog (#54)

### Other Changes

- ci: support ansible-lint and ansible-test 2.16 (#52)
- ci: Use supported ansible-lint action; run ansible-lint against the collection (#53)

[1.1.1] - 2023-12-08
--------------------

### Other Changes

- ci: Bump actions/github-script from 6 to 7 (#49)
- refactor: get_ostree_data.sh use env shebang - remove from .sanity* (#50)

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
