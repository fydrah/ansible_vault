Ansible Vault module
====================

This module provides a simple way to create a ansible vaulted file.


Usage
-----

.. code-block:: yaml

       - name: create file
         ansible_vault:
           dest: /path/to/file.txt
           passphrase: mysuperpassphrase
           data: |
             my
             data:
               in: ["any"]
             "format": [
               "it": "is",
               "paste": "as"
             ]
             [raw]
             into = vaulted
             file = enjoy

Requirements
------------

* **ansible-vault** (*pip install ansible-vault*)
