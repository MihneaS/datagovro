# data.gov.ro

## Setup

1. `vagrant up`
2. Do the steps from 4 for installing from [source](http://docs.ckan.org/en/ckan-2.3/maintaining/installing/install-from-source.html).

## Folder hierarchy

- `ckan/`
  - `etc/` - symlinked to `/etc/ckan`
  - `lib/` - symlinked to `/usr/lib/ckan`
    - `default/src/ckanext-romania_theme/` - code of the theme
      - `i18n/ro/` - custom translations
- `docs/`
- `provisioning/playbook.yml` - provisioning Ansible scripts

## To Do

- [ ] configure the other steps to be run from Ansible
- [ ] provision airbrake through Ansible
