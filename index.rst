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
  :caption: Ansible Lab (optional)
  :name: _ansible_lab
  :hidden:

  ansible_install/ansible_install
  ansible_basics/ansible_basics
  ansible_lamp_playbook/ansible_lamp_playbook


  appendix/glossary


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

Networking / Credentials
..........
Cluster IP: 172.16.70.19

PC IP: 172.16.70.20

Username: admin

Pwd: 1qaz2wsx#EDC

Network Details: 172.16.68.0/22

Useable Range: 172.16.70.1 – 172.16.71.222 (DHCP has already been setup)

Gateway: 172.16.68.1/22

.. note::

Windows VM: administrator / nutanix/4u
Oracle VM: oracle / oracle
