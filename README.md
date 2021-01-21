## fonts

[![CI](https://github.com/Oefenweb/ansible-fonts/workflows/CI/badge.svg)](https://github.com/Oefenweb/ansible-fonts/actions?query=workflow%3ACI)
[![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-fonts-blue.svg)](https://galaxy.ansible.com/Oefenweb/fonts)

Set up fonts in Debian-like systems.

#### Requirements

* `fontconfig` (will be installed)

#### Variables

* `fonts_font_paths`: [default: `[]`]: Font path declarations
* `fonts_font_paths.{n}.src`: [required]: The local path of the font directory
* `fonts_font_paths.{n}.dest`: [required]: The remote path of the font directory
* `fonts_font_paths.{n}.state`: [optional, default: `present`]: State

* `fonts_rsync_path`: [default: `rsync`]: Specify the `rsync` command to run on the remote host

## Dependencies

None

#### Example

```yaml
---
- hosts: all
  roles:
    - fonts
```

#### License

MIT

#### Author Information

Mischa ter Smitten

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Oefenweb/ansible-fonts/issues)!
