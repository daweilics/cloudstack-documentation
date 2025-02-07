.. Licensed to the Apache Software Foundation (ASF) under one
   or more contributor license agreements.  See the NOTICE file
   distributed with this work for additional information#
   regarding copyright ownership.  The ASF licenses this file
   to you under the Apache License, Version 2.0 (the
   "License"); you may not use this file except in compliance
   with the License.  You may obtain a copy of the License at
   http://www.apache.org/licenses/LICENSE-2.0
   Unless required by applicable law or agreed to in writing,
   software distributed under the License is distributed on an
   "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
   KIND, either express or implied.  See the License for the
   specific language governing permissions and limitations
   under the License.

Compatibility Matrix
====================

Supported OS Versions for Management Server
-------------------------------------------

This section lists the operating systems that are supported for running
CloudStack Management Server.

-  Ubuntu 18.04 LTS, 20.04 LTS
-  CentOS versions 7, 8 (note: CentOS 8 will EOL in Dec 2021)
-  Rocky Linux 8
-  RHEL versions 7, 8
-  openSUSE Leap 15
-  SUSE Linux Enterprise Server 15

   .. note:: There is a known issue with ipmitool with RHEL8 / SUSE, so certain functionality such as out of band management might not work

Software Requirements
~~~~~~~~~~~~~~~~~~~~~

-  Java JRE 11
-  MySQL 5.6, 5.7, 8.0

Supported Hypervisor Versions
-----------------------------

CloudStack supports three hypervisor families, XenServer with XAPI, KVM,
and VMware with vSphere.

-  Ubuntu 18.04 LTS, 20.04 LTS with KVM
-  CentOS 7, 8 with KVM (note: CentOS 8 will EOL in Dec 2021)
-  Rocky Linux 8 with KVM
-  Red Hat Enterprise Linux 7, 8 with KVM
-  Rocky Linux 8 with KVM
-  openSUSE Leap 15
-  SUSE Linux Enterprise Server 15
-  XenServer versions 7.1, 7.2, 7.4, 7.5, 8.0 with latest hotfixes, XCP-ng 7.4, 7.6, 8.0, 8.1, 8.2

   .. note:: It is now required to enable HA on the XenServer pool in order to recover from a pool-master failure. Please refer to the `XenServer documentation <https://docs.citrix.com/en-us/xencenter/7-1/pools-ha-enable.html>`_.

-  VMware versions 6.5, 6.7 and 7.0

   .. note:: There is a known issue in 6.7 U1 (https://kb.vmware.com/s/article/67315) which blocks some CloudStack cloning operations. The use of linked clones is known to be effected.

   .. note:: There is a known issue in 6.7 U3 - 6.7 U3f where a mailformed OVA could crash vCenter services (for more information see `here <https://mail-archives.apache.org/mod_mbox/cloudstack-users/202005.mbox/%3CCAMvtBPNQqbe0XEsHyjFMror7HRvj-c%3DfEe7y12NfCDQSFTYgqQ%40mail.gmail.com%3E>`_). To avoid the issue, make sure to use 6.7 U3g or later.

-  LXC Host Containers on RHEL 7
-  Windows Server 2012 R2 (with Hyper-V Role enabled)
-  Hyper-V 2012 R2
-  Oracle VM 3.0+
-  Bare metal hosts are supported, which have no hypervisor. These hosts
   can run the following operating systems:

   -  Fedora 17
   -  Ubuntu 12.04


Supported External Devices
--------------------------

-  Netscaler VPX and MPX versions 9.3, 10.1e and 10.5
-  Netscaler SDX version 9.3, 10.1e and 10.5
-  SRX (Model srx100b) versions 10.3 to 10.4 R7.5
-  F5 11.X
-  Force 10 Switch version S4810 for Baremetal Advanced Networks


Supported Browsers
------------------

The CloudStack Web-based UI should be compatible with any modern
browser, but it's possible that some browsers will not render portions
of the UI reliably, depending on their support of Web standards. For
best results, one of the following browsers recommended:

-  Firefox version 75 or later

-  Google Chrome version 85 or later

-  Safari 12+

Notice Of Management OSes and Hypervisors to be Deprecated
----------------------------------------------------------

The following hypervisors are no longer be supported in this release due to vendor EOL:

-  XenServer 6.2
-  XenServer 6.5
-  XenServer 7.0
-  vSphere 5.0
-  vSphere 5.1
-  vSphere 5.5
-  vSphere 6.0
-  CentOS/RHEL (KVM) 6.x
-  Ubuntu 14.04
-  Ubuntu 16.04

The following Management Server Operating Systems are no longer supported in this release due to vendor EOL:

-  CentOS 6.x
-  Ubuntu 14.04
-  Ubuntu 16.04

Please see `CloudStack Wiki <https://cwiki.apache.org/confluence/display/CLOUDSTACK/Hypervisor+and+Management+Server+OS+EOL+Dates>`_
for details.
