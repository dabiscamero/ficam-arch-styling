---
layout: default
title: Applications Diagrams
permalink: /applications/
---
| **Description** | A view of general enterprise ICAM applications and systems. |
| **Audience** | ICAM Enterprise Architects and Implementation specialists. |

<img style="max-width:100%;" src="{{site.baseurl}}/img/ApplicationsInterfaceDiagram.png" alt="Image of applications interface diagram."/>
<img style="max-width:100%;" src="{{site.baseurl}}/img/ApplicationsDescriptions.png" alt="Image of applications interface diagram descriptions."/>

The diagram above provides a bird’s eye view of the different ICAM solutions, applications, and software components that work together to run a functional, secure ICAM program. Within each section of the diagram, there is an accompanying description that explains the general purpose of each application or system as well as which business services they support.

The data input into any ICAM application or system should come from an authoritative, or trusted, source. The Agency ICAM Applications Solutions and Systems in the middle of the diagram (Identity Management System, Access Control System, Credential Management System, Certificate Authority, and Governance Tools) use the data from authoritative sources to perform their function. From an ICAM perspective, an agency endpoint is any physical or logical resource that your agency wants to secure and protect. The systems, applications, solutions, and tools depicted in this diagram all work together to make sure that your resources stay protected.

##### Authoritative Sources
Authoritative sources are any trusted sources of data. This data primarily consists of identity attributes.

##### Identity Management System
The identity management system (IDMS) retains identity data that is retrieved from authoritative source(s) within its identity store and allows for the creation, maintenance, resolution, and deactivation of identities. It may also be accessed to complete an individual’s identity proofing. The role manager within the IDMS leverages the policy database and the provisioning and workflow tool to execute entitlement management activities and provision access privileges to identity accounts.

##### Access Control System
The access control system manages and executes parts of both the design time and run time access processes. Policy administration decisions are stored within a policy database and managed through policy management software. These policies are referenced during dynamic access authorization attempts. It also stores access entitlements within a database. The access management tool helps to execute run time authentication and authorization decisions, leveraging the workflow tool to gather pertinent information from the other ICAM systems. The visitor management system and federated access manager are both important components to grant access to external system users.

##### Credential Management System
The credential management system contains management software that processes sponsored requests for credential registration, creates, issues, and maintains credentials, and stores this information within the credential database.

##### Certificate Authority
The certificate authority contains a certificate repository, which stores data on valid certificates that is leveraged during authentication. The certificate revocation list (CRL) and online certificate status protocol (OCSP) are two methods for checking if a certificate has been revoked.

##### Governance Tools
Governance software aids in the back end processes that support ICAM functionalities. The reporting and analytics software completes auditing, logging, and data transformation for the agency’s ICAM ecosystem. Access certification software audits user permissions to assure that they are still accurate, while remediation software implements the required changes to mitigate identified variances.

##### Agency Endpoints
Agency endpoints are any resource that an agency wants to protect, whether physical or a logical system.

##Background & Key Revisions
Several of the existing target state diagrams were combined to create a single, enterprise-wide view of ICAM systems. Descriptions have also been included for each system and the business service that they assist in delivering.

An item of note is that the application names within this diagram have been abstracted and simplified as to remain product and vendor neutral. In practice, vendor solutions may offer an application or a bundled suite of software that delivers solutions across several of the boxes seen here. For example, a vendor might offer an application that provides both policy management and access management functionality.
