.. _compatibility:

************************
|morphver| Compatibility
************************

When installing and upgrading to |morpheus| |morphver|, refer to the following to ensure compatibility.

|morpheus| Application OS
=========================

The Morpheus Applications can be installed on the following Operating System versions:

+--------+--------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| OS     | Version(s)   | Notes                                                                                                                                                                                             |
+========+==============+===================================================================================================================================================================================================+
| CentOS | 7+           | CentOS 7.7 installs FreeRDP 2.0 which is not compatible with Guacamole. To resolve, see https://support.morpheusdata.com/s/article/The-Morpheus-console-RDP-window-is-empty-white                 |
+--------+--------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Ubuntu | 16.04, 18.04 |                                                                                                                                                                                                   |
+--------+--------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Debian | 8,9          |                                                                                                                                                                                                   |
+--------+--------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| RHEL   | 7+           |                                                                                                                                                                                                   |
+--------+--------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Services
========

When externalizing MySQL, Elasticsearch and/or RabbitMQ services, the following versions are compatible with Morpheus |morphver|:

.. important:: Elasticsearch 7.x is required for v4.1.2. Refer to :ref:`upgrading` for more information.

+---------------------------------------+----------------------+---------------------------------+
| **Service**                           |**Compatible Branch** | **|morphver| Installer Version**|
+---------------------------------------+----------------------+---------------------------------+
| MySQL                                 | 5.7                  | 5.7.27                          |
+---------------------------------------+----------------------+---------------------------------+
| Percona                               | 5.7, WSREP 31        | n/a                             |
+---------------------------------------+----------------------+---------------------------------+
| Elasticsearch                         | 7.x                  | 7.4.2                           |
+---------------------------------------+----------------------+---------------------------------+
| RabbitMQ                              | 3.5-3.7              | 3.7.16                          |
+---------------------------------------+----------------------+---------------------------------+
| Redis                                 | REMOVED              | REMOVED                         |
+---------------------------------------+----------------------+---------------------------------+

Integrations
============

.. note:: Current iterations of Amazon AWS, Microsoft Azure, Google Cloud Platform, Digital Ocean, HPE OneView, OpenTelekom Cloud, IBM Bluemix, Softlayer and UpCloud are all supported.

+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Integration       | Supported Version(s)                                     | Known incompatibilities                                                                                                               |
+===================+==========================================================+=======================================================================================================================================+
| Ansible           | 2.7.6                                                    |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Ansible Tower     | 3.3.0                                                    |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| App Dynamics      | 4.5.1                                                    |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Azure Stack       | GA                                                       |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Cisco ACI         | 3.10                                                     |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Commvault         | v11 sp 12                                                |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Docker            | v19.03.4, API version 1.40                               |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Docker            | 1.12.6                                                   |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Jenkins           | < 2.176.1                                                |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Kubernetes        | 1.11                                                     |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Kubernetes        | Major:"1", Minor:"14", GitVersion:"v1.14.1"              |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Microsoft Hyper-V | 2012R2, 2016, 2019                                       |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Nutanix AHV       | 5.0 - 5.10                                               | In 5.5 - 5.7 if Prism Central is enabled, no actions that create images in Prism will function due to Prism Central Image Management. |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Openstack         | Juno, Kilo, Liberty, Mitaka, Newton, Ocata, Pike, Queens |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Rubrik            | 4.2                                                      |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| ServiceNow        | Istanbul, Jakarta, Kingston, London                      |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Splunk            | 7.10                                                     |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Terraform         | v0.11.3                                                  | Not Compatible with v0.12.x (Support Planned)                                                                                         |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| vCloud Director   | 8.20, 9.1, 9.5                                           |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Veeam             | 9.5u3, 9.5u4                                             |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| VMware ESXi       | 5.5, 6.0, 6.5, 6.7                                       |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| VMware Fusion     | 8, 9, 10+                                                |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| VMware NSX        | -V                                                       | NSX -T Support Planned                                                                                                                |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| VMware vCenter    | 5.5, 6.0, 6.5, 6.7                                       |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| XenServer         | 7.0                                                      |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+

.. note:: Non-listed versions may be compatible but are not verified.

If you have any specific requirements please contact support@morpheusdata.com
