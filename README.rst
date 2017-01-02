ansible-backup
==============

Install `Duplicity`_ package and `Duply`_ script. By default Duplicity is
installed from system package. If ``duplicity_url`` variable is specified, it is
installed from given link.

.. _Duplicity: http://duplicity.nongnu.org
.. _Duply: http://duply.net

Requirements
------------

No requirements.

Role Variables
--------------

+------------------------------------+----------+-------------------------------------------+-----------+-----------------------------------+
|                Name                |   Type   |                Description                | Mandatory |              Default              |
+====================================+==========+===========================================+===========+===================================+
| ``duplicity_url``                  |  string  | Url of custom Duplicity tarball to        |     no    |                                   |
|                                    |          | install.                                  |           |                                   |
+------------------------------------+----------+-------------------------------------------+-----------+-----------------------------------+
| ``duplicity_dist_dir``             |  string  | Path to directory where custom files are  |     no    |          /opt/duplicity           |
|                                    |          | downloaded.                               |           |                                   |
+------------------------------------+----------+-------------------------------------------+-----------+-----------------------------------+

Dependencies
------------

No dependencies.

Example Playbook
----------------

To use the role in your playbook, add something like the following to
the desired play:

.. code-block:: yaml

    - hosts: servers
      roles:
         - { role: dblenkus.duplicity }

License
-------

Licensed under the GPLv3 License. See the COPYING file for details.

Author Information
------------------

Domen Blenkuš
