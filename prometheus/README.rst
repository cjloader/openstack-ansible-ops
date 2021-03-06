Install Prometheus
##################
:tags: openstack, ansible

About this repository
---------------------

This set of playbooks will deploy Prometheus. If this is being deployed as part of
an OpenStack all of the inventory needs will be provided for.

**These playbooks require Ansible 2.4+.**

Deployment Process
------------------

Clone the repo

.. code-block:: bash

    cd /opt
    git clone https://github.com/openstack/openstack-ansible-ops

Downloading role dependencies

.. code-block:: bash

    cd /opt/openstack-ansible-ops/prometheus
    ansible-galaxy install -r ansible-role-requirements.yml


Install node_exporter

.. code-block:: bash

    cd /opt/openstack-ansible-ops/prometheus
    openstack-ansible installNodeExporter.yml
