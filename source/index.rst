FOSS Hosting at the OSU Open Source Lab
=======================================

* Lance Albertson
* Director
* lance@osuosl.org
* @ramereth

About me
--------

* Director OSU Open Source Lab
* Systems Admin Background
* Specialities:

  * Virtualization: Ganeti, Openstack
  * Configuration Management: CFengine, Puppet, Chef
  * Big storage: GlusterFS

* Gentoo Developer (since 2003 but not as active these days)

What I'll Cover
---------------

* Overview of the lab
* Historical Background
* Major services we provide
* Tools we use
* What's next for us

In the Beginning...
-------------------

.. image:: /_static/open-source.jpg
  :align: left
  :width: 50%

* University President sees *"www.orst.edu"* on a sign
* Maintain - DNS/DHCP management
* Seed money from OSU Network Services
* First clients are some of the most well known Open Source projects 

Why do hosting at OSU?
----------------------

  *"Our commitment to the development and application of Open Source is
  consistent with our drive to be the land grant university of the 21st century.
  Through open source activities we are helping underserved populations around
  the world and creating new industries and new products at home."*

  OSU president, Ed Ray

Timing is everything
--------------------

* Post dot-com bust = lots of dark fiber
* Invested $500K into laying 28mi of fiber to I-5
* *"Cheap"* bandwidth
* Internet2 connectivity
* Newly renovated data center

Notable Project Hosting Milestones
----------------------------------

* Gentoo 2003
* Debian 2003
* Kernel.org 2005
* ASF 2005
* Linux Foundation 2008
* OSGeo 2010
* Python Software Foundation 2012
* Robot Operating System (ROS) 2013
* Buildbot/RTEMS 2013

Over the past ten years...
--------------------------

* Grown from hosting a few servers to several hundred
* Made Oregon State the center of FOSS hosting
* 60 OSL Alumni staff and students

  * Google, Facebook, Rackspace, Intel, etc...

* Helped 160 FOSS projects with their hosting

Staff
-----

* 4 full-time employees
* 16-18 undergrad students

  * 6-10 sysadmin
  * 4-6 devs
  * 2-3 media & communication

* Hosting / Development
* Media & PR team
* Director

Students
--------

.. image:: /_static/student-working.jpg
  :align: right
  :width: 50%

* Undergraduate students
* Full root access
* Hired Sophomore year
* Constant turnover (2-3yrs/student)

Systems Meeting
---------------

.. image:: /_static/systems-meeting.jpg
  :align: center
  :width: 95%

NOC
---

.. image:: /_static/noc1.jpg
  :align: center
  :width: 95%

NOC
---

.. image:: /_static/noc2.jpg
  :align: center
  :width: 95%

OSL Funding Model
-----------------

* Donations

  * Large Corporations
  * Projects
  * Individuals

* Hosting Contracts
* Grants
* No state funding
* Larger projects generally pay for hosting

We need your help!
==================

  *Corporate sponsorships Individual donations*

  http://osuosl.org/donate

Data Center Specs
-----------------

.. image:: /_static/datacenter.png
  :align: right
  :width: 50%

* 2770 sqft, 76 Colo racks, 11 IDF racks
* Dual independent power feeds

  * ea 400A / 480V
  * 3-phase
  * Dual UPS
  * Single generator

* 55 ton cooling capacity via 3 Lieberts

Networking
----------

.. image:: /_static/networking.png
  :align: right
  :width: 50%

.. image:: /_static/osuosl-nero-week.png
  :align: right
  :width: 50%

* NERO

  * (Network for Education & Research in Oregon)

* 10 Gbps to NERO
* Cisco 6509 Core
* 2 Gbps to upstream
* IPv6 coming this summer
* 250TB/mo outbound / 60TB/mo inbound (OSU traffic only)

Datacenter Pics
---------------

.. image:: /_static/datacenter1.jpg
  :align: center
  :width: 95%

Datacenter Pics
---------------

.. image:: /_static/datacenter2.jpg
  :align: center
  :width: 95%

Datacenter Pics
---------------

.. image:: /_static/datacenter3.jpg
  :align: center
  :width: 95%

Hosted Machines
---------------

* ~400 servers
* 200+ virtual machines 
* Projects purchase/own servers 

  * 22 racks used by OSL currently
  * Project racks: Drupal, ASF, Gentoo and Linux Foundation

* What are they running?

  * Debian/Ubuntu, CentOS and FreeBSD

ASF & Drupal Racks
------------------

.. image:: /_static/drupal-rack.jpg
  :align: left
  :width: 45%

.. image:: /_static/asf-rack.jpg
  :align: right
  :width: 45%

PSF, NAS-Admin, Gentoo
----------------------

.. image:: /_static/psf-rack.jpg
  :align: left
  :width: 45%

.. image:: /_static/gentoo-rack.jpg
  :align: right
  :width: 45%

Xiph.org
--------

.. image:: /_static/xiph-server.png
  :align: center
  :width: 95%

Services Provided at the OSL
----------------------------

* Co-location hosting
* Smart-hands support
* Virtual machine(s)
* Managed hosting
* FTP Mirror space
* Email forwarding & Mailing list hosting
* DNS hosting
* Software builds & testing (Supercell)

FTP Mirrors
-----------

.. image:: /_static/ftp-osl.png
  :align: right
  :width: 50%

* 3 servers

  * Corvallis, Oregon
  * Chicago, IL
  * New York, NY

* 6 TB capacity
* Split via DNS view
* 230TB per month
* TDS Telecom
* Upgrading to POWER8 machines soon

Virtualization/Cloud platforms
------------------------------

* Ganeti

  * Infrastructure as a Service (IaaS)
  * *"Pet"* virtual machines
  * High available VM platform

* Openstack

  * On-demand temporary VM resources for testing
  * *"Cattle"* virtual machines

Ganeti at OSL
-------------

* Ganeti - Google FOSS project
* Ganeti Web Manager - OSL project
* Linux KVM hypervisor
* Easy to expand & manage
* Primary Production cluster

  * 6 machines / 180 VMs / 30VMs /server

* Project clusters

  * OSGeo, PSF, Debian*

Ganeti Environment
------------------

* Limited local storage (10-30G)
* No Database servers as VMs

  * Bad performance, inefficient use of resources

* Use shared web hosting for simple sites
* Managed and unmanaged
* K.I.S.S. virtualization management

Openstack at the OSL
--------------------

* Internal test cluster

  * Limited testing currently
  * Chef cookbook testing

* POWER8 Openstack Cluster
* Supercell shifting towards OpenStack

Large data storage
------------------

* HA-NFS (currently being rebuilt)
* GlusterFS in limited trials

  * Very flexible depending on use-cases
  * Excellent expandability
  * Performance not the greatest
  * Must tailor each use case

    * Hosting php files is sub-optimal
    * Ideal for Moodle Data and Drupal files

ORVSD (Oregon Virtual School District)
--------------------------------------

* Primarily Moodle & Drupal hosting for K12 districts
* Has been running for 8 school years
* Give teachers something they can use in the classroom tomorrow
* Host 750 web sites
* 180K user accounts
* 2.5TB of content
* 50+ VMs, GlusterFS, MySQL

Supercell
---------

.. image:: /_static/supercell.jpg
  :align: right
  :width: 50%

* Continuous integration testing
* Run-time testing
* Several platforms supported
* On-demand virtualization
* Powered by Ganeti+KVM
* Migrating towards Openstack
* Hardware donation initially by Facebook

POWER7 (ppc64) Development
--------------------------

.. image:: /_static/power7.png
  :align: right
  :width: 50%

* 7 loaned POWER7 machines (8231-E2B)
* Project access to architecture
* OSL Managed
* Projects using the machines:

  * Fedora, Debian, CentOS, PostreSQL, Gentoo, Eclipse, GCC build farm,
    OpenJDK, Linux Foundation, LLVM, Mozilla, V8

POWER8 (ppc64/ppc64le)
-----------------------

* 4 loaned POWER8 machines (8247-22L)
* Uses newer OPAL firmware
* Supports Little Endian on ppc
* KVM on OpenPOWER w/ Openstack
* Enables FOSS projects easy access to IBM's newer platform in a cloud-like
  manner
* Participating in the IBM Challenge

Hosting FAQ
-----------

* Hosting tailored to each project
* Target medium-large *"high impact"* projects
* Typically outgrown their current hosting
* Bad experiences with other hosting
* Let the projects code instead of worrying about their site

Requesting Hosting
------------------

* http://osuosl.org/requesthosting
* Submit request to support@osuosl.org 
* What we look for

  * Widely used project
  * Healthy community
  * Needs fit within our resources

Hosted Projects (just a few shown)
----------------------------------

.. image:: /_static/projects.png
  :align: center
  :width: 95%

More projects
-------------

.. image:: /_static/osl-projects-word-cloud.jpg
  :align: center
  :width: 95%

Growth
------

* 8 years ago...

  * <10 racks
  * ~60 machines / ~30 VMs
  * ~60 projects

* Today

  * 22 racks / ~160 projects
  * ~400 machines / ~200 VMs

* Similar amount of people resources

Current Devops Tools
--------------------

.. csv-table::
  :header: Type, Tool

  Configuration Management, "Chef, migrating away from CFengine"
  Monitoring, "Nagios, munin, cacti, awstats"
  Ticket Tracking, "RT (external), Chili Project (internal), Github"
  Operating System, "CentOS 6, Gentoo Hardened (deprecated)"

Infrastructure changes
----------------------

* Migrating towards all CentOS
* Migrating towards chef
* Reasons

  * Easier to manage with chef
  * Easier to teach to students
  * Faster deployment & better QA
  * Less time maintaining the OS

Events & Outreach
-----------------

* Devops Bootcamp

  * Staff/Student informal sysadmin/developer training
  * Started in 2013, in second year

* Beaver Barcamp

  * Un-conference for students and community
  * Twice a year (mid Apr & Oct) - now annual in the spring

* OSULUG: Install fests, presentations, etc
* OSL Summit: Quarterly workshop for OSL students and staff
* GOSCON 2005-2010

  * Government Open Source Conference

Organization changes
--------------------

* Organizational move into EECS (Fall 2013)

  * Academic home for OSL
  * Education & Research
  * Better fit within OSU (most of our students are in EECS)

* Center for Applied Systems and Software (CASS)

  * Collaborating with Business Solutions Group (BSG)
  * Research focused development/hosting
  * Initially working in the IoT space

Goals for the future
--------------------

* Create a flexible on-demand & automated build and testing environment
* Performance testing infrastructure
* Expand FTP hosting into its own CDN
* Build or implement a PaaS for common hosted applications
* More non-x86 architecture hosting for development & testing

Questions?
----------

* Lance Albertson
* lance@osuosl.org
* @ramereth
* http://osuosl.org
* http://lancealbertson.com
