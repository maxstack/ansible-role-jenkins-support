# ansible-role-jenkins-support

RHEL/CentOS - Support packages for jenkins

## Requirements

None

## Role Variables

Available variables are listed below, along with default values:

    packages:
      - python-pip
      - vim
      - git

## Dependencies

None

## Example Playbook

    - hosts: all
      roles:
        - role: maxstack.jenkins-support
          packages:
            - python-pip
            - vim
            - git
