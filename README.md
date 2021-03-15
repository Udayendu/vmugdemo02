# Changelog

## [v1.0] - 15-03-2021

### Added

- Ansible Roles
  - deploy
  - guestoscustom
  - winupdates
  - softwareupload
  - softwareinstall
  - delete

- Tag based deployment

### Software support

- ansible-3.1.0
- pyvmomi-7.0.1
- pywinrm-0.4.1


## Deployment Guide:

### To deploy the windows server, use the below command:

  $ ansible-playbook -i inventory dcwindemo.yaml --tags "deploy"

### To do the guest os customization, use the below command:

  $ ansible-playbook -i inventory dcwindemo.yaml --tags "guestoscustom"

### To update the windows for security, critical, and rollup updates:

  $ ansible-playbook -i inventory dcwindemo.yaml --tags "winupdates"

### To upload the Software(Chrome & NotePad++):

  $ ansible-playbook -i inventory dcwindemo.yaml --tags "softwareupload"

### To install the uploaded Software:

  $ ansible-playbook -i inventory dcwindemo.yaml --tags "softwareinstall"

### To delete the windows server use the below command:

  $ ansible-playbook -i inventory dcwindemo.yaml --tags "delete"

