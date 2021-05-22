https://github.com/ned300889/utilities/actions/workflows/main.yml/badge.svg

Role Name
=========

Install my utilities and dot files to a new fedora workstation

Requirements
------------

Create a user and update vars/main.yml

Role Variables
--------------


    # Default theme
    oh_my_zsh_theme: robbyrussell

    # Default plugins
    oh_my_zsh_plugins:
      - git

    # Wether to install by default for all specified users.
    # May be overridden by `oh_my_zsh: install:` under each user.
    oh_my_zsh_install: yes

    # User configuration
    # Important: oh-my-zsh is installed per user so you need to specify the users to install it for.
    users:
      - username: nsimpson
        oh_my_zsh:
          theme: robbyrussell
          plugins:
            - git


Example Playbook
----------------

    - hosts: localhost
      roles:
         - { role: ned300889.utilities}

License
-------

GPL 2.0

