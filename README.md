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
    build_jobs:
      - https://raw.githubusercontent.com/maxstack/packer-ansible-jenkins/master/_jenkins/packer-ansible-jenkins-pipeline.xml
      - https://raw.githubusercontent.com/maxstack/aws-pipelines/master/destroy-ami/aws-pipelines-destroy-ami.xml


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
      build_jobs:
        - https://raw.githubusercontent.com/maxstack/packer-ansible-jenkins/master/_jenkins/packer-ansible-jenkins-pipeline.xml
        - https://raw.githubusercontent.com/maxstack/aws-pipelines/master/destroy-ami/aws-pipelines-destroy-ami.xml

