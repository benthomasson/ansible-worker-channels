=============================
Ansible Worker Channels
=============================

.. image:: https://badge.fury.io/py/ansible-worker-channels.svg
    :target: https://badge.fury.io/py/ansible-worker-channels

.. image:: https://travis-ci.org/benthomasson/ansible-worker-channels.svg?branch=master
    :target: https://travis-ci.org/benthomasson/ansible-worker-channels

.. image:: https://codecov.io/gh/benthomasson/ansible-worker-channels/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/benthomasson/ansible-worker-channels

Ansible Runner with Django Channels v2 integration

Documentation
-------------

The full documentation is at https://ansible-worker-channels.readthedocs.io.

Quickstart
----------

Install Ansible Worker Channels::

    pip install ansible-worker-channels

Add it to your `INSTALLED_APPS`:

.. code-block:: python

    INSTALLED_APPS = (
        ...
        'ansible_worker_channels.apps.AnsibleWorkerChannelsConfig',
        ...
    )

Add Ansible Worker Channels's URL patterns:

.. code-block:: python

    from ansible_worker_channels import urls as ansible_worker_channels_urls


    urlpatterns = [
        ...
        url(r'^', include(ansible_worker_channels_urls)),
        ...
    ]

Features
--------

* TODO

Running Tests
-------------

Does the code actually work?

::

    source <YOURVIRTUALENV>/bin/activate
    (myenv) $ pip install tox
    (myenv) $ tox

Credits
-------

Tools used in rendering this package:

*  Cookiecutter_
*  `cookiecutter-djangopackage`_

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage
