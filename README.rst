================
packer-templates
================

Packer_ template(s).

Currently contains a Centos 7 template with Vagrant post-processor.

The current intention is to create a docker host for local use.

Inspired by https://github.com/tacahilo/packer-centos-7

How to use
==========

Install Packer
______________

`Packer docs`_

Install Virtualbox
__________________

`VirtualBox Downloads`_

Build
_____

- Validate template

  `packer validate basebox.json`

- Initiate build

  `packer build basebox.json`

Notes
_____

- When debugging build issues, remove headless flag from basebox.json
- For faster build, download iso and modify iso_url value in basebox.json to fs path

.. _Packer: http://www.packer.io/
.. _`Packer Docs`: http://www.packer.io/docs/installation.html
.. _`VirtualBox Downloads`: https://www.virtualbox.org/wiki/Downloads
