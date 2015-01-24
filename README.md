Role Name
=========

Sets the ``{{ march }}`` which will contain the appropriate march for the
host's CPU. Ie.::

    $ gcc -c -Q -march=native --help=target | grep march | grep -o '\w*$'
    haswell

Requirements
------------

Requires the gcc command.

Example Playbook
----------------

Example:

    - hosts: servers
      roles:
        - jpic.march

      tasks:
        - debug: var=march

License
-------

BSD
