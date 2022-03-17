python-gitlab 2022
=============

.. image:: https://github.com/python-gitlab/python-gitlab/workflows/Test/badge.svg
   :target: https://github.com/python-gitlab/python-gitlab/actions

.. image:: https://badge.fury.io/py/python-gitlab.svg
   :target: https://badge.fury.io/py/python-gitlab

.. image:: https://readthedocs.org/projects/python-gitlab/badge/?version=latest
   :target: https://python-gitlab.readthedocs.org/en/latest/?badge=latest

.. image:: https://codecov.io/github/python-gitlab/python-gitlab/coverage.svg?branch=main
    :target: https://codecov.io/github/python-gitlab/python-gitlab?branch=main

.. image:: https://img.shields.io/pypi/pyversions/python-gitlab.svg
   :target: https://pypi.python.org/pypi/python-gitlab

.. image:: https://img.shields.io/gitter/room/python-gitlab/Lobby.svg
   :target: https://gitter.im/python-gitlab/Lobby

.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/python/black

``python-gitlab 2022`` Es un paquete de Python que brinda acceso a la API del servidor de GitLab.


Admite la API v4 de GitLab y proporciona una herramienta CLI (``gitlab``).

Instalacion
------------

Es compatible con Python 3.7+.
Usar ``pip`` para instalar la ultima version

.. code-block:: console

   $ pip install --upgrade python-gitlab

La versión de desarrollo actual está disponible tanto en `GitHub.com

<https://github.com/python-gitlab/python-gitlab>`__ and `GitLab.com
<https://gitlab.com/python-gitlab/python-gitlab>`__, and can be
installed directly from the git repository:

.. code-block:: console

   $ pip install git+https://github.com/python-gitlab/python-gitlab.git

From GitLab:

.. code-block:: console

   $ pip install git+https://gitlab.com/python-gitlab/python-gitlab.git


Using the docker image
----------------------

You can run the Docker image directly from the GitLab registry:

.. code-block:: console

   $ docker run -it --rm registry.gitlab.com/python-gitlab/python-gitlab:latest <command> ...

For example, to get a project on GitLab.com (without authentication):

.. code-block:: console

   $ docker run -it --rm registry.gitlab.com/python-gitlab/python-gitlab:latest project get --id gitlab-org/gitlab

You can also mount your own config file:

.. code-block:: console

   $ docker run -it --rm -v /path/to/python-gitlab.cfg:/etc/python-gitlab.cfg registry.gitlab.com/python-gitlab/python-gitlab:latest <command> ...

Building the image
~~~~~~~~~~~~~~~~~~

To build your own image from this repository, run:

.. code-block:: console

   $ docker build -t python-gitlab:latest .

Run your own image:

.. code-block:: console

   $ docker run -it --rm -v python-gitlab:latest <command> ...

Bug reports
-----------

Please report bugs and feature requests at
https://github.com/python-gitlab/python-gitlab/issues.

Gitter Community Chat
---------------------

We have a `gitter <https://gitter.im/python-gitlab/Lobby>`_ community chat
available at https://gitter.im/python-gitlab/Lobby, which you can also
directly access via the Open Chat button below.

If you have a simple question, the community might be able to help already,
without you opening an issue. If you regularly use python-gitlab, we also
encourage you to join and participate. You might discover new ideas and
use cases yourself!

Documentation
-------------

The full documentation for CLI and API is available on `readthedocs
<http://python-gitlab.readthedocs.org/en/stable/>`_.

Build the docs
~~~~~~~~~~~~~~

We use ``tox`` to manage our environment and build the documentation::

    pip install tox
    tox -e docs

Contributing
------------

For guidelines for contributing to ``python-gitlab``, refer to `CONTRIBUTING.rst <https://github.com/python-gitlab/python-gitlab/blob/main/CONTRIBUTING.rst>`_.
