# 1. DEFINITIONS 

The following terms and their definitions are of great importance for the correct comprehension of the objectives, context and policies described herein.

IP address allocation follows a hierarchical scheme. Responsibility for the administration of number resources is distributed globally in accordance with the hierarchical structure shown below.

![](https://www.lacnic.net/innovaportal/file/681/1/jerarquia_en.jpg)

## 1.1.IANA (Internet Assigned Number Authority)

IANA is responsible for allocating part of the global IP address space and autonomous system numbers to Regional Registries according to established needs.

## 1.2.Internet Registry (IR)

An Internet Registry (IR) is an organization responsible for allocating IP address space to its members or customers and for registering those allocations. IRs are classified according to their main function and geographic area of coverage as indicated in the hierarchical structure defined in the figure above.

## 1.3.Regional Internet Registry (RIR)

Regional Internet Registries (RIRs) are established and authorized by their respective regional communities, and recognized by the IANA to serve and represent large geographical regions. The primary role of RIRs is to manage and allocate Internet resources within their own respective regions.

## 1.4.National Internet Registry (NIR)

A National Internet Registry (NIR) primarily allocates Internet resources to its members or constituents, which are generally LIRs.

## 1.5.Local Internet Registry (LIR)

A Local Internet Registry (LIR) is an IR that primarily assigns Internet resources to the users of the network services it provides. LIRs are generally ISPs, whose customers are primarily end users and possibly other ISPs.

## 1.6.Internet Service Provider (ISP)

Internet Service Providers mainly assign IP address space to end users of the network services they provide. Their clients may be other ISPs. ISPs do not have geographical restrictions as do NIRs.

## 1.7.End Site or End User (EU)

An end site is defined as an end user (subscriber) that has a legal or commercial relationship (the same or associated entities) with an Internet service provider which involves:

* the service provider assigning address space to the end user
* the service provider offering transit services for the end user towards other sites
* the service provider transporting the end user's traffic
* the service provider announcing an aggregated route prefix which contains the address space assigned by LACNIC to the end user

## 1.8.Allocate

To allocate means to distribute address space to IRs for the purpose of subsequent distribution by them.

## 1.9.Assign

To assign means to delegate address space to an end user, to be exclusively used within the infrastructure operated by said end user, as well as for interconnection purposes.

The assigned address space must only be used by the original recipient of the assignment, as well as for third-party devices provided they are operating within said infrastructure.

Therefore, sub-assignments to third parties outside said infrastructure (for example, the use of end-user assignments for ISPs or similar clients) and providing addresses to third parties in data centers (and others) are not allowed.

## 1.10.The Internet Registry System

The Internet registry system has been established with the aim of enforcing the objectives of exclusivity, preservation, routability and information. This system consists of hierarchically organized Internet registries (IRs). Internet number resources (addresses, ASNs, others) are typically assigned to end users by ISPs or NIRs.<br>
<br>
These resources are previously allocated to NIRs and ISPs by the Regional Internet Registries.<br>
<br>
Under this system, end users are organizations that operate networks that use the resources. Just as LACNIC, NIRs maintain resources for making assignments to end users or allocations to Internet Service Providers. Assigned resources are used to operate networks, whereas allocated resources are kept by Internet Registries for their future assignment to end users.

Note that the resources allocated or assigned by LACNIC or by the NIRs are to be used exclusively by their recipient or by third parties authorized by the recipient, provided that the policies currently in force allow such use. We recommend that such authorizations can be verified using RPKI.

## 1.11.Non-Guaranteed Routability

Neither LACNIC nor the NIRs will guarantee the routability of allocated or assigned addresses.

Resource recipients are responsible for negotiating such routability with their connectivity providers. LACNIC shall provide the corresponding guidance when necessary.

However, allocated or assigned resources must be announced within a maximum of 90 days, except in those cases where the need not to announce the resources is justified.

RIRs must apply operational procedures that reduce the possibility of fragmentation of the address space to minimize the risk of loss of routability.

## 1.12.Multihomed

A site is considered to be multihomed if it receives full-time connectivity from more than one Internet service provider and has one or more routing prefixes announced by at least two of its upstream providers. Independent providers refer to the fact that one does not reach the Internet through the other.

## 1.13.RPKI ASN 0 ROA

LACNIC will create specific Routing Origin Authorizations (ROAs) in the RPKI infrastructure with AS 0 in the Origin ASN field and the list of unallocated or unassigned Internet Number Resources exclusively under LACNIC administration in the Prefixes list such ROAs.

The number of the before mentioned ROAs and any other technical parameter of it will be under LACNIC discretion

Only LACNIC would have authority to create RPKI ROAs for Internet Number Resources not yet allocated or assigned or either recovered or returned, to which LACNIC is the rightful custodian.

Once an Internet Number Resource is allocated or assigned, LACNIC will invalidate ROAs that contain such resources and will issue new ROAs that do not include them, as necessary.

## 1.14.Principles for Proper Administration and Stewardship

The fundamental principle is to distribute unique Internet numbering resources according to the technical and operational needs of the networks currently using, or that will use, these numbering resources, allowing the sustainable growth of the Internet.

The numbering resources under the stewardship of LACNIC must be distributed among organizations legally constituted within its service region [COBERTURA] and mainly *serving networks and services operating in this region. External clients connected directly to main infrastructure located in the region are allowed.

*"Mainly" is understood to mean more than 50%.

"Anycast" services that use numbering resources outside said region are acceptable as long as they are provided by an organization legally constituted within the service region [COBERTURA] and at least one copy of the service is hosted on local infrastructure.

Upon obtaining any type of resources from LACNIC or from the corresponding NIR, any legacy resources held by the recipient will no longer be considered legacy resources.

### 1.14.1.Rational Distribution

Internet numbering resources must be distributed ensuring their uniqueness and considering the technical and operational needs of the networks and infrastructure that use them. Considerations must be made to take into account potential limitations on the availability of each numbering resource at the time of their distribution.

### 1.14.2.Public Information Registry

Providing a public registry of information relating to the numbering resources that have been distributed is a fundamental requirement for the Internet numbering resources distribution system.

Aimed mainly at ensuring the resources' uniqueness while providing usage and contact information in case operational or security problems arise. Also, to allow analyzing the use of these resources.

### 1.14.3.Hierarchical Distribution

The hierarchical distribution of Internet numbering resources seeks to contribute to the Internet routing system's scalability, allowing resources to be grouped and announced as concisely as possible.

In some cases, the goals mentioned above may be in conflict with each other or with the particular interests of the requesting organizations. In these cases, a careful analysis of each particular situation is required so that an appropriate compromise can be reached among the conflicting parties.

## 1.15. Resource Requests

Resource requests to LACNIC or to the corresponding NIRs will be made under the systems in force.

Any request that is considered incomplete will be returned to the applicant with the appropriate instructions so that it can be completed.
