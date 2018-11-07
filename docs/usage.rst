=====
Usage
=====

To use Ansible Worker Channels in a project, add it to your `INSTALLED_APPS`:

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
