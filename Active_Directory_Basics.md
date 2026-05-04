# TryHackMe | Active Directory Basics Notes

## 1. Introduction to Active Directory (AD)
Active Directory is a directory service developed by Microsoft for Windows domain networks. It serves as a centralized database for managing permissions and access to networked resources.

### Key Functions:
* **Authentication:** Verifying the identity of a user (e.g., login).
* **Authorization:** Granting permission to access specific resources (e.g., folders, printers).

## 2. AD Hierarchical Structure
AD uses a logical structure to organize objects:
* **Forest:** The highest level of container; a collection of one or more domain trees.
* **Tree:** A group of domains that share a contiguous DNS namespace.
* **Domain:** The core unit of AD; a logical group of network objects (users, computers) sharing the same database.
* **Organizational Units (OUs):** Containers within a domain used to organize objects and apply Group Policies (GPOs).

## 3. AD Components & Terminology
* **Domain Controller (DC):** The server that hosts the AD database and handles authentication requests.
* **AD Data Store (NTDS.dit):** The physical database file where all AD information is stored (`%SystemRoot%\NTDS\ntds.dit`).
* **Global Catalog:** A service that allows users to find objects in any domain within the forest.
* **DNS:** Essential for AD; it allows clients to locate Domain Controllers.

## 4. Physical Structure
While the logical structure focuses on organization, the physical structure focuses on network performance:
* **Sites:** Represent the physical topology of the network (e.g., different office buildings).
* **Subnets:** IP ranges associated with specific sites to optimize replication traffic.

## 5. Group Policy Objects (GPOs)
GPOs are used by administrators to define settings for users and computers across the domain.
* **Common Uses:** Setting desktop wallpapers, enforcing password complexity, or disabling USB ports.
* **Inheritance:** Settings flow from the Domain level down to OUs unless explicitly blocked.

## 6. Trusts
Trusts allow users in one domain to access resources in another.
* **Transitive:** If A trusts B and B trusts C, then A trusts C.
* **Directional:** Can be one-way or two-way.

## 7. Protocol Overview
* **LDAP (Lightweight Directory Access Protocol):** Used to query and modify the AD database.
* **Kerberos:** The primary authentication protocol for AD.
* **NTLM:** A legacy authentication protocol (still used in some environments).
