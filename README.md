# Lab Services Open Source Projects

Curated list of open source projects which are either created by [IBM Lab Services](https://www.ibm.com/it-infrastructure/services/lab-services) consultants, or to which Lab Services consultants contribute to. [Please bring your own!](CONTRIBUTING.md)


## Projects

### IBM Spectrum Scale (GPFS) - Ansible Role
* Lab Services contacts:
  * Achim Christ <achim.christ@de.ibm.com>
  * Ole Kristian Myklebust <ole.kristian.myklebust@no.ibm.com>
* Programming language: Ansible (YAML)
* Platform: RHEL 7
* Links:
  - [Ansible Galaxy](https://galaxy.ansible.com/acch/spectrum_scale)
  - [GitHub](https://github.com/acch/ansible-scale)
  - [Spectrum Scale GUI Role](https://github.com/acch/ansible-scale-gui)

- **Description:**
  Highly-customizable Ansible role for installing and configuring IBM Spectrum Scale (GPFS).

- **User story:**
  A client who already invested heavily in infrastructure automation based on Red Hat Ansible was conducting  a proof of concept (PoC) with IBM Spectrum Scale (GPFS). Automating deployment of all infrastructure components was a key requirement for the client, which is why Lab Services was engaged to develop necessary playbooks for Spectrum Scale. The client agreed to publishing those playbooks as open source, hence the code could be re-used during other client engagements and is actively being maintained and enhanced based on client requirements.


### IBM Spectrum Virtualize IP-Quorum - Ansible Role
* Lab Services contacts:
  * Ole Kristian Myklebust <ole.kristian.myklebust@no.ibm.com>
* Programming language: Ansible (YAML)
* Platform: RHEL 7
* Links:
  - [Ansible Galaxy](https://galaxy.ansible.com/olemyk/ansible_ipquorum)
  - [GitHub](https://github.com/olemyk/ansible-ipquorum)
  - [Blog/Medium](https://medium.com/@ole.kr.myklebust/automated-ip-quorum-installation-with-ansible-269311b3c23d)

- **Description:**
  Ansible role for installing and configuring IP-Quorum Service for Spectrum Virtualize (SAN: SVC, FlashSystem, Storwize, v9000)
  IP-Quorum application is used to resolve failure scenarios where half the control canisters/nodes on the cluster become unavailable.

- **User story:**
  The IP-quorum application is a Java application that runs on a separate host. IP-Quorum application is not an service and the host needs Java installed to run.
  Many times the customer asked how could we run this as a service, we created then a service that made it possible to run the service but the whole installation is with several manual steps.
  So with that i wanted to simplify and automate the installation of IP-Quorum, and with this Ansible role it will install Java, create ip-quorum service, copies in IP-Quorum Java application localy or remotly from Spectrum Virtualize cluster and more.


### IBM Spectrum Control - Ansible Role
* Lab Services contacts:
  - Ole Kristian Myklebust <ole.kristian.myklebust@no.ibm.com>
* Programming language: Ansible (YAML)
* Platform: RHEL 7
* Links:
  - [Ansible Galaxy](https://galaxy.ansible.com/olemyk/ansible_spectrum_control/)
  - [GitHub](https://github.com/olemyk/ansible-spectrum-control)
  - [Blog/Medium](https://medium.com/@ole.kr.myklebust/automated-ibm-spectrum-control-installation-with-ansible-2593d9e93691)

- **Description:**
  Ansible role for installing and configuring IBM Spectrum Control on Linux.
  IBM Spectrum Control provides monitoring, automation and analytics for multiple-vendor storage environments.

- **User Story:**
  The Spectrum Control installation can be sometimes time-consuming, boring and upgrades are getting more frequent. So with that i wanted to simplify and automate the installation of IBM Spectrum Control and IBM DB2.


### IBM DB2 - Ansible Role
* Lab Services contacts:
  - Ole Kristian Myklebust <ole.kristian.myklebust@no.ibm.com>
* Programming language: Ansible (YAML)
* Platform: RHEL 7
* Links:
  - [Ansible Galaxy](https://galaxy.ansible.com/olemyk/ansible_role_db2/)
  - [GitHub](https://github.com/olemyk/ansible-role-db2)

- **Description:**
  Ansible role to install IBM DB2 on linux, this project have been forked and updated to work with newer DB2 version and IBM Spectrum Control.


## License

This project is licensed under the terms of the [Creative Commons Zero (CC0 1.0)](LICENSE) license.

[![CC0](https://i.creativecommons.org/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)


### BaaSapi - GUI for hyperledger fabric network
* Lab Services contacts:
  - Liyong Li <liyong.li@ibm.com>
* Programming language: Golang (API) and VUEjs (frontend)
* Platform: Linux
* Links:
  - [GitHub](https://github.ibm.com/Liyong-Li/baasapi)

- **Description:**
  BaaSapi is a lightweight management UI which allows you to easily manage your hyperledger fabric environments (kubernetes).
  BaaSapi allows you to manage your hyperledger fabric resources (network, organization, nodes, CA, channel, chaincodes and more) !
  
Introduction
https://github.ibm.com/Liyong-Li/baasapi/blob/master/Blockchain_Platform_Solution_v1.0.pdf
