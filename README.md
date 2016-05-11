sa-lighttable
=============

[![Build Status](https://travis-ci.org/softasap/sa-lighttable.svg?branch=master)](https://travis-ci.org/softasap/sa-lighttable)

Example of use:

- hosts: dev

  vars:
    - root_dir: "{{playbook_dir}}/../"


  pre_tasks:
    - debug: msg="Pre tasks section"

  roles:

    - {
        role: "sa-lighttable"
      }


  tasks:
    - debug: msg="Tasks section"



Possible overrides:

  lighttable_version: X.Y.Z  - defaults to 0.8.1

