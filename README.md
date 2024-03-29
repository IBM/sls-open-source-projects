# Lab Services Open Source Projects

Curated list of open source projects which are either created by [IBM Lab Services](https://www.ibm.com/it-infrastructure/services/lab-services) consultants, or to which Lab Services consultants contribute to. [Please bring your own!](CONTRIBUTING.md)

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [Projects](#projects)
  - [IBM Spectrum Scale (GPFS) - Ansible Role](#ibm-spectrum-scale-gpfs---ansible-role)
  - [IBM Spectrum Virtualize IP-Quorum - Ansible Role](#ibm-spectrum-virtualize-ip-quorum---ansible-role)
  - [IBM Spectrum Control - Ansible Role](#ibm-spectrum-control---ansible-role)
  - [IBM DB2 - Ansible Role](#ibm-db2---ansible-role)
  - [IBM Spectrum Virtualize - Ansible Playbooks](#ibm-spectrum-virtualize---ansible-playbooks)
  - [BaaSapi - GUI for Hyperledger Fabric Network](#baasapi---gui-for-hyperledger-fabric-network)
  - [Docker Files for s390x](#docker-files-for-s390x)
  - [IBM Data Privacy Passports - Hands-on Lab](#ibm-data-privacy-passports---hands-on-lab)
  - [Pervasive Encryption - Hands-on Lab](#pervasive-encryption---hands-on-lab)
  - [IBM Spectrum Virtualize Check (SVCheck)](#ibm-spectrum-virtualize-check-svcheck)
  - [IBM Spectrum Scale Policy Scripts](#ibm-spectrum-scale-policy-scripts)
  - [IBM Spectrum Scale Automation](#ibm-spectrum-scale-automation)
  - [IBM Spectrum Archive Enterprise Edition Check (check_spectrumarchive.sh)](#ibm-spectrum-archive-enterprise-edition-check-check_spectrumarchivesh)
  - [iRODS Tiered-Storage Tape](#irods-tiered-storage-tape)
  - [Tape Archive REST API](#tape-archive-rest-api)
  - [Key Lifecycle Manager Tools (klmutils)](#key-lifecycle-manager-tools-klmutils)
  - [IBM Spectrum Scale Bash Command Line Completion](#ibm-spectrum-scale-bash-command-line-completion)
  - [Infrastructure-as-Code for IBM Cloud Object Storage Trial VM](#infrastructure-as-code-for-ibm-cloud-object-storage-trial-vm)
  - [Integration of IBM Spectrum Discover with IBM Spectrum Archive](#integration-of-ibm-spectrum-discover-with-ibm-spectrum-archive)
  - [IBM Copy Services Manager Rexx Collection](#ibm-copy-services-manager-rexx-collection)
- [License](#license)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Projects

### IBM Spectrum Scale (GPFS) - Ansible Role

-   Lab Services contacts:
    -   Achim Christ <mailto:achim.christ@de.ibm.com>
    -   Ole Kristian Myklebust <mailto:ole.kristian.myklebust@no.ibm.com>
-   Programming language: Ansible (YAML)
-   Platform: RHEL 7
-   Links:
    -   [Ansible Galaxy](https://galaxy.ansible.com/acch/spectrum_scale)
    -   [GitHub](https://github.com/acch/ansible-scale)
    -   [Spectrum Scale GUI Role](https://github.com/acch/ansible-scale-gui)
    -   [Spectrum Scale Installation and Configuration](https://github.com/IBM/ibm-spectrum-scale-install-infra)
    -   [Blog/Medium](https://medium.com/possimpible/deploying-spectrum-scale-with-ansible-part1-singel-node-4cd7e48064ec)
    -   [Ansible Scale Demo](https://github.com/IBM/ansible-scale-demo)


-   **Description:**
    Highly-customizable Ansible role for installing and configuring IBM Spectrum Scale (GPFS).

-   **User story:**
    A client who already invested heavily in infrastructure automation based on Red Hat Ansible was conducting  a proof of concept (PoC) with IBM Spectrum Scale (GPFS). Automating deployment of all infrastructure components was a key requirement for the client, which is why Lab Services was engaged to develop necessary playbooks for Spectrum Scale. The client agreed to publishing those playbooks as open source, hence the code could be re-used during other client engagements and is actively being maintained and enhanced based on client requirements.

### IBM Spectrum Virtualize IP-Quorum - Ansible Role

-   Lab Services contacts:
    -   Ole Kristian Myklebust <mailto:ole.kristian.myklebust@no.ibm.com>
-   Programming language: Ansible (YAML)
-   Platform: RHEL 7
-   Links:
    -   [Ansible Galaxy](https://galaxy.ansible.com/olemyk/ansible_ipquorum)
    -   [GitHub](https://github.com/olemyk/ansible-ipquorum)
    -   [Blog/Medium](https://medium.com/@ole.kr.myklebust/automated-ip-quorum-installation-with-ansible-269311b3c23d)


-   **Description:**
    Ansible role for installing and configuring IP-Quorum Service for IBM Spectrum Virtualize (SAN: SVC, FlashSystem, Storwize, v9000).
    IP-Quorum application is used to resolve failure scenarios where half the control canisters/nodes on the cluster become unavailable.

-   **User story:**
    The IP-quorum application is a Java application that runs on a separate host. IP-Quorum application is not an service and the host needs Java installed to run.
    Many times the customer asked how could we run this as a service, we created then a service that made it possible to run the service but the whole installation is with several manual steps.
    So with that i wanted to simplify and automate the installation of IP-Quorum, and with this Ansible role it will install Java, create ip-quorum service, copies in IP-Quorum Java application localy or remotly from IBM Spectrum Virtualize cluster and more.

### IBM Spectrum Control - Ansible Role

-   Lab Services contacts:
    -   Ole Kristian Myklebust <mailto:ole.kristian.myklebust@no.ibm.com>
-   Programming language: Ansible (YAML)
-   Platform: RHEL 7
-   Links:
    -   [Ansible Galaxy](https://galaxy.ansible.com/olemyk/ansible_spectrum_control/)
    -   [GitHub](https://github.com/olemyk/ansible-spectrum-control)
    -   [Blog/Medium](https://medium.com/@ole.kr.myklebust/automated-ibm-spectrum-control-installation-with-ansible-2593d9e93691)


-   **Description:**
    Ansible role for installing and configuring IBM Spectrum Control on Linux.
    IBM Spectrum Control provides monitoring, automation and analytics for multiple-vendor storage environments.

-   **User Story:**
    The IBM Spectrum Control installation can be sometimes time-consuming, boring and upgrades are getting more frequent. So with that I wanted to simplify and automate the installation of IBM Spectrum Control and IBM DB2.

### IBM DB2 - Ansible Role

-   Lab Services contacts:
    -   Ole Kristian Myklebust <mailto:ole.kristian.myklebust@no.ibm.com>
-   Programming language: Ansible (YAML)
-   Platform: RHEL 7
-   Links:
    -   [Ansible Galaxy](https://galaxy.ansible.com/olemyk/ansible_role_db2/)
    -   [GitHub](https://github.com/olemyk/ansible-role-db2)


-   **Description:**
    Ansible role to install IBM DB2 on Linux, this project have been forked and updated to work with newer DB2 version and IBM Spectrum Control.

### IBM Spectrum Virtualize - Ansible Playbooks

-   Lab Services contacts:
    -   Ole Kristian Myklebust <mailto:ole.kristian.myklebust@no.ibm.com>
-   Programming language: Ansible (YAML)
-   Links:
    -   [GitHub](https://github.com/olemyk/ansible-virtualize-playbooks)
    -   [Medium](https://medium.com/@ole.kr.myklebust/managing-your-spectrum-virtualize-with-ansible-part-1-6f3ec173948f)


-   **Description:**
    Ansible playbooks examples for the Ansible Collection - ibm.spectrum_virtualize.

### BaaSapi - GUI for Hyperledger Fabric Network

-   Lab Services contacts:
    -   Liyong Li <mailto:liyong.li@ibm.com>
-   Programming language: Golang (API) and Vue.js (frontend)
-   Platform: Linux
-   Links:
    -   [GitHub](https://github.com/liyong-li/baasapi)
    -   [PDF](https://github.com/liyong-li/baasapi/blob/master/Blockchain_Platform_Solution_v1.0.pdf)


-   **Description:**
    BaaSapi is a lightweight management UI which allows you to easily manage your Hyperledger Fabric environments (supported with Kubernetes).
    BaaSapi allows you to manage your Hyperledger Fabric resources (network, organization, nodes, CA, channel, chaincodes and more)!

### Docker Files for s390x

-   Lab Services contacts:
    -   Guillaume Hoareau <mailto:guillaume_hoareau@fr.ibm.com>
-   Programming language: Dockerfile
-   Platform: Linux on IBM z
-   Links:
    -   [GitHub](https://github.com/linux-on-ibm-z/dockerfile-examples)


-   **Description:**
    A collection of examples to show how Dockerfiles could be created and used on Linux on IBM z, LinuxONE or z/OS CX.

### IBM Data Privacy Passports - Hands-on Lab

-   Lab Services contacts:
    -   Guillaume Hoareau <mailto:guillaume_hoareau@fr.ibm.com>
-   Programming language: Markdown
-   Platform: Linux on IBM z
-   Links:
    -   [GitHub](https://github.com/guikarai/IBMDPP)


-   **Description:**
    Hands-On Lab about IBM Data Privacy Passports to protect the data at the consumption and the extraction point.

### Pervasive Encryption - Hands-on Lab

-   Lab Services contacts:
    -   Guillaume Hoareau <mailto:guillaume_hoareau@fr.ibm.com>
-   Programming language: Markdown
-   Platform: Linux on IBM z
-   Links:
    -   [GitHub](https://github.com/guikarai/PE-LinuxONE-1804LTS)


-   **Description:**
    Hands-On Lab about Pervasive Encryption for LinuxONE and Linux on IBM z. A walkthrough for understanding how to encrypt data at speed and volume, at rest and in motion.

### IBM Spectrum Virtualize Check (SVCheck)

-   Lab Services contacts:
    -   Luis Bolinches <mailto:luis.bolinches@fi.ibm.com>
    -   Mika Heino <mailto:mika.heino@fi.ibm.com>
-   Programming language: Python
-   Platform: Python 3
-   Links:
    -   [GitHub](https://github.com/IBM/SVCheck)


-   **Description:**
    This tools generates Excel file of IBM Spectrum Virtualize system via REST API calls.

### IBM Spectrum Scale Policy Scripts

-   Lab Services contacts:
    -   Nils Haustein <mailto:nils_haustein@de.ibm.com>
-   Programming language: Bash
-   Links:
    -   [GitHub](https://github.com/IBM/spectrum-scale-policy-scripts)
    -   [Whitepaper](https://www.ibm.com/support/pages/node/6355577)


-   **Description:**
    This project includes scripts and policies for IBM Spectrum Scale ILM in combination with IBM Spectrum Archive Enterprise Edition and IBM Spectrum Protect for Space Management.

### IBM Spectrum Scale Automation

-   Lab Services contacts:
    -   Nils Haustein <mailto:nils_haustein@de.ibm.com>
-   Programming language: Bash
-   Links:
    -   [GitHub](https://github.com/IBM/SpectrumScaleAutomation)
    -   [Presentation](http://files.gpfsug.org/presentations/2017/Manchester/03-1_Automation.pdf)
    -   [Whitepaper](https://www.ibm.com/support/pages/node/6355601)


-   **Description:**
    This project describes a framework for automation of IBM Spectrum Scale storage services, such as backup (mmbackup), tiering (mmapplypolicy) and Scale out Backup and Recovery (Sobar).

### IBM Spectrum Archive Enterprise Edition Check (check_spectrumarchive.sh)

-   Lab Services contacts:
    -   Nils Haustein <mailto:nils_haustein@de.ibm.com>
    -   Jan-Frode Myklebust <mailto:jan-frode@no.ibm.com>
-   Programming language: Bash
-   Platform: Nagios / Icinga
-   Links:
    -   [GitHub](https://github.com/IBM/check_spectrumarchive)


-   **Description:**
    This utility performs status checks of IBM Spectrum Archive Enterprise Edition components. It can be integrated with the IBM Spectrum Scale event monitoring framework, or with Nagios, Icinga, or compatible monitoring systems.

### iRODS Tiered-Storage Tape

-   Lab Services contacts:
    -   Nils Haustein <mailto:nils_haustein@de.ibm.com>
-   Programming language: Bash
-   Platform: iRODS
-   Links:
    -   [GitHub](https://github.com/IBM/irods-tieredStorage-tape)


-   **Description:**
    This project includes examples for integrating iRODS software with IBM Spectrum Scale and IBM Spectrum Archive Enterprise Edition.

### Tape Archive REST API

-   Lab Services contacts:
    -   Nils Haustein <mailto:nils_haustein@de.ibm.com>
-   Programming language: JavaScript
-   Platform: Node.js
-   Links:
    -   [GitHub](https://github.com/IBM/tape-archive-api)


-   **Description:**
    The Tape archive REST API facilitates controlling migration and recalls of files managed by IBM Spectrum Archive Enterprise Edition version 1.3.0.3 and above.

### Key Lifecycle Manager Tools (klmutils)

-   Lab Services contacts:
    -   Daniel Wendler <mailto:daniel.wendler@de.ibm.com>
-   Programming language: Python
-   Platform: Python 3
-   Links:
    -   [GitHub](https://github.com/IBM/klmutils)


-   **Description:**
    Utility to query IBM Security Guardium Key Lifecycle Manager (GKLM/SKLM) server status via REST API. Depending on the type of the deployed architecture (Standalone, Multi-Master or Master-Clone) different kind of API endpoints are queried and the responses are evaluated.

### IBM Spectrum Scale Bash Command Line Completion

-   Lab Services contacts:
    -   Maarten Kreuger <mailto:maarten_kreuger@nl.ibm.com>
-   Programming language: Bash
-   Platform: Linux
-   Links:
    -   [GitHub](https://github.com/MaartenKreuger/scale-completion)


-   **Description:**
    Bash command line completion for IBM Spectrum Scale.

### Infrastructure-as-Code for IBM Cloud Object Storage Trial VM

-   Lab Services contacts:
    -   Mathias Defiebre <mailto:mathias.defiebre@de.ibm.com>
    -   Harald Seipp <mailto:SEIPP@de.ibm.com>
-   Programming language: Bash
-   Platform: Linux
-   Links:
    -   [GitHub](https://github.com/hseipp/ibm-cos-vm-iac)


-   **Description:**
    The purpose of this project is to demonstrate how a pure virtual variant of the IBM Cloud Object Storage (COS) System can be built on top a KVM-based Linux virtualization host.

### Integration of IBM Spectrum Discover with IBM Spectrum Archive

-   Lab Services contacts:
    -   Nils Haustein <mailto:nils_haustein@de.ibm.com>
-   Programming language: Bash
-   Platform: Linux
-   Links:
    -   [GitHub](https://github.com/IBM/discover-tape-recall-integration)
    -   [Blog](https://community.ibm.com/community/user/storage/blogs/nils-haustein1/2022/02/10/spectrumdiscover-taperecall-integration)


-   **Description:**
    This set of program examples accommodates workflows for tape optimized recalls of files using the metadata management capabilities of IBM Spectrum Discover.

### IBM Copy Services Manager Rexx Collection

-   Lab Services contacts:
    -   Thomas Luther <mailto:tluther@de.ibm.com>
-   Programming language: REXX
-   Platform: IBM z
-   Links:
    -   [GitHub](https://github.com/IBM/CSM-Rexx-Collection)
    -   [Blog](https://community.ibm.com/community/user/storage/blogs/thomas-luther1/2022/02/21/how-to-use-ibm-copy-services-manager-rest-api-on-z)


-   **Description:**
    The purpose of this project is to provide Rexx examples to utilize IBM Copy Services Manager. Most examples focus on Rexx on IBM z, but some may be used also with other Rexx distributions on various platforms.

## License

This project is licensed under the terms of the [Creative Commons Zero (CC0 1.0)](LICENSE) license.

[![CC0](https://i.creativecommons.org/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
