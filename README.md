# Ansible role: Google Chrome

[![Build Status](https://travis-ci.org/danbohea/ansible-role-google-chrome.svg?branch=master)](https://travis-ci.org/danbohea/ansible-role-google-chrome)

Installs & configures Google Chrome on Mac OS X.


## Requirements

- Mac OS 10.9+


## Role Variables

All role default variables are listed below along with their respective default values.

```
google_chrome_appdir: "/Applications"
```

Where to install the app. The value is passed to Homebrew Cask via the `--appdir` option.

```
google_chrome_AppleEnableSwipeNavigateWithScrolls: false
```

Toggles trackpad swipe navigation. Default is to disable it.


## Dependencies

- [danbohea.homebrew](https://galaxy.ansible.com/danbohea/homebrew)


## Example Playbook

```
- hosts: macbook
  connection: local

  roles:
    - role: ansible-role-google-chrome
```

## License

MIT


## Author Information

This role was created by [Dan Bohea](http://bohea.co.uk) primarily for use with [Macsible](https://github.com/danbohea/macsible).
