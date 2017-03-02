ansible cleanup
===============
[![Build Status](https://travis-ci.org/ypsman/ansible-cleanup.svg?branch=master)](https://travis-ci.org/ypsman/ansible-cleanup)

Clean a Server to create a Base Image from.

After the run, shutdown the mashine and make a Clean base image.

Clears:
-------
  - maildir
  - tmp files
  - Postfix logfiles
  - user/root bash_history
  - all logs in /var/log

Example Playbook
----------------

    - hosts: all
      roles:
        - role: ypsman.cleanup
