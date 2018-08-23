.. title:: Welcome to Nutanix Partner Enablement Factory (Elite Training)

.. toctree::
  :maxdepth: 2
  :caption: Technology Overview
  :name: _technology_overview
  :hidden:

  what_is_nutanix/what_is_nutanix
  nutanix_terminology/nutanix_terminology


.. toctree::
  :maxdepth: 2
  :caption: Getting Started with SQL
  :name: _startsql
  :hidden:

  sql_lab/sql_lab

.. toctree::
  :maxdepth: 2
  :caption: SQL Hands on Labs
  :name: _labs
  :hidden:

  SQLLAB01/sqllab01
  SQLLAB02/sqllab02


.. toctree::
  :maxdepth: 2
  :caption: SQL Design Lab
  :name: _DESIGNLAN01
  :hidden:

  DESIGNLAB01/designlab1


.. toctree::
    :maxdepth: 2
    :caption: Oracle Hands on Labs
    :name: _labs
    :hidden:

    examplelab1/examplelab1
    examplelab2/examplelab2


.. toctree::
      :maxdepth: 2
      :caption: Oracle Design Lab
      :name: _oracledesignlab1
      :hidden:

      oracledesignlab1/oracledesignlab1


.. toctree::
  :maxdepth: 2
  :caption: Nutanix Calm Lab
  :name: _nutanix_calm_lab
  :hidden:

  calm_enable/calm_enable
  calm_mysql_blueprint/calm_mysql_blueprint
  calm_lamp_blueprint/calm_lamp_blueprint
  calm_marketplace/calm_marketplace

.. toctree::
  :maxdepth: 2
  :caption: Optional Labs
  :name: _optional_labs
  :hidden:


.. toctree::
  :maxdepth: 2
  :caption: Flow Lab
  :name: _flow_lab
  :hidden:

  flow_enable/flow_enable
  flow_quarantine_vm/flow_quarantine_vm
  flow_isolate_environments/flow_isolate_environments
  flow_secure_app/flow_secure_app
  flow_visualization/flow_visualization

.. toctree::
  :maxdepth: 2
  :caption: Appendix
  :name: _appendix
  :hidden:


.. toctree::
  :maxdepth: 2
  :caption: Ansible Lab (optional)\
  :name: _ansible_lab
  :hidden:

  ansible_install/ansible_install
  ansible_basics/ansible_basics
  ansible_lamp_playbook/ansible_lamp_playbook


  appendix/glossary
  appendix/basics

.. _getting_started:

---------------
Welcome to Nutanix NPEF Elite training 2018!
---------------

Welcome to the Nutanix Partner Enablement Factory! This workbook accompanies an instructor-led session that introduces Nutanix Calm and many common management tasks. Each section has a lesson and an exercise to give you hands-on practice. The instructor explains the exercises and answers any additional questions that you may have.

At the end of the workshop, attendees should understand the basic concepts and technologies that make up Nutanix Calm and should be well prepared to demo and talk about Calm.

What's New
++++++++++++++++++++++++++++++++++++++++++++++++++

- Workshop updated for the following software versions:
    - AOS 5.6
    - PC 5.7.1

- Optional Lab Updates:
    - Ansible

Agenda
++++++

- Introductions
- Technology Overview
- SQL Lab (Day1)
- Oracle Lab (Day1)
- Nutanix Calm Lab (Day2)
- Flow Lab (Day2)
- Optional Labs
  - Ansible Lab

Introductions
+++++++++++++

- Name
- Familiarity with Nutanix

Initial Setup
+++++++++++++

- Take note of the *Passwords* being used.
- Login to the Prism Central with the IP address provided by instructor.

Environment Details
+++++++++++++++++++

Nutanix Workshops are intended to be run in the Nutanix Hosted POC or in a demo cluster provided by the facilitator.

Your cluster will be provisioned with all necessary images, networks, and VMs required to complete the exercises.

You will be provided with the necessary file server that has the images that could not be found in the cluster.

Networking
..........

Hosted POC clusters follow a standard naming convention:

- **Cluster Name** - POC\ *XYZ*
- **Subnet** - 10.**21**.\ *XYZ*\ .0
- **Cluster IP** - 10.**21**.\ *XYZ*\ .37

If provisioned from the marketing pool:

- **Cluster Name** - MKT\ *XYZ*
- **Subnet** - 10.**20**.\ *XYZ*\ .0
- **Cluster IP** - 10.**20**.\ *XYZ*\ .37

For example:

- **Cluster Name** - POC055
- **Subnet** - 10.21.55.0
- **Cluster IP** - 10.21.55.37

Throughout the Workshop there are multiple instances where you will need to substitute *XYZ* with the correct octet for your subnet, for example:

.. list-table::
  :widths: 25 75
  :header-rows: 1

  * - IP Address
    - Description
  * - 10.21.\ *XYZ*\ .37
    - Nutanix Cluster Virtual IP
  * - 10.21.\ *XYZ*\ .39
    - **PC** VM IP, Prism Central
  * - 10.21.\ *XYZ*\ .40
    - **DC** VM IP, NTNXLAB.local Domain Controller

Each cluster is configured with 2 VLANs which can be used for VMs:

.. list-table::
  :widths: 25 25 10 40
  :header-rows: 1

  * - Network Name
    - Address
    - VLAN
    - DHCP Scope
  * - Primary
    - 10.21.\ *XYZ*\ .1/25
    - 0
    - 10.21.\ *XYZ*\ .50-10.21.\ *XYZ*\ .124
  * - Secondary
    - 10.21.\ *XYZ*\ .129/25
    - *XYZ1*
    - 10.21.\ *XYZ*\ .132-10.21.\ *XYZ*\ .253

Credentials
...........

.. note::

  All users will be accessing to the same cluster with the below credentials. If otherwise mentioned by instructor.

.. list-table::
  :widths: 25 35 40
  :header-rows: 1

  * - Credential
    - Username
    - Password
  * - Wifi Login
    - nutanix (SSID)
    - nutanix/4u
  * - Prism Element
    - admin
    - Nutanix/4u!@34
  * - Prism Central
    - admin
    - Nutanix/4u!@34
  * - Controller VM
    - nutanix
    - nutanix/4u
  * - Prism Central VM
    - nutanix
    - nutanix/4u

Each cluster has a dedicated domain controller VM, **DC**, responsible for providing AD services for the **NTNXLAB.local** domain. The domain is populated with the following Users and Groups:

.. list-table::
  :widths: 25 35 40
  :header-rows: 1

  * - Group
    - Username(s)
    - Password
  * - Administrators
    - Administrator
    - nutanix/4u
  * - SSP Admins
    - adminuser01
    - nutanix/4u
  * - SSP Developers
    - devuser01
    - nutanix/4u
  * - SSP Power Users
    - poweruser01
    - nutanix/4u
  * - SSP Basic Users
    - basicuser01
    - nutanix/4u
