<div align="center">

[**_``Go Back``_**](../README.md)

</div>

# Overview of Computer security

## 1.1. Computer Security Concepts

Computer security involves the protection of computer systems and the data they store from unauthorized access, use, disclosure, disruption, modification, or destruction. It encompasses a variety of measures designed to safeguard the integrity, availability, and confidentiality of computer systems and the information they process.

## 1.2. Computer Security, Information Security, Network Security

### Computer Security
Focuses on protecting the computer systems and their components (hardware, software, firmware) from threats and vulnerabilities.

**Components:**

- ``Hardware Security``: Protection against physical damage or tampering (e.g., using locks, surveillance).
- ``Software Security``: Protection against malicious software and ensuring software integrity (e.g., anti-virus, patches).
- ``Firmware Security``: Ensuring the integrity and security of firmware (e.g., secure boot, firmware updates).

**Examples of Measures:**

- ``Access Controls``: Restricting who can use or access the computer system.
- ``Antivirus Software``: Detecting and removing malware.
- ``Operating System Hardening``: Configuring the OS to minimize vulnerabilities.

### Information Security
Ensures the protection of data, both in transit and at rest, from unauthorized access and misuse.

**Core Aspects:**

- ``Data Confidentiality``: Ensuring data is only accessible to those who are authorized.
- ``Data Integrity``: Ensuring data is accurate and unaltered.
- ``Data Availability``: Ensuring data is accessible when needed by authorized users.

**Examples of Measures:**

- ``Encryption``: Encoding data so only authorized parties can read it.
- ``Data Masking``: Hiding sensitive data to prevent unauthorized access.
- ``Access Controls``: Restricting access to data based on roles and permissions.
- ``Backup Solutions``: Regularly copying data to prevent loss.

### Network Security
Involves securing the data transmitted over networks through protocols, firewalls, and encryption.

**Core Aspects:**

- ``Data Transmission Security``: Ensuring data sent over a network is secure from eavesdropping or tampering.
- ``Network Infrastructure Security``: Protecting the network's hardware and software from attacks.
- ``Access Control``: Managing who can access the network and its resources.

**Examples of Measures:**

- ``Firewalls``: Filtering incoming and outgoing network traffic based on security rules.
- ``Intrusion Detection Systems (IDS)``: Monitoring network traffic for suspicious activity.
- ``Virtual Private Networks (VPN)``: Creating secure connections over public networks.
- ``Secure Socket Layer (SSL) / Transport Layer Security (TLS)``: Encrypting data in transit to ensure secure communication.

## 1.3. Threats, Attacks, and Assets

### Threats
Threats are potential dangers that could exploit a vulnerability to breach security.

**Examples:**

- ``Malware``: Malicious software designed to damage or disrupt systems (e.g., viruses, worms, ransomware).
- ``Phishing``: Fraudulent attempts to obtain sensitive information by disguising as a trustworthy entity (e.g., fake emails or websites).
- ``Insider Threats``: Risks posed by individuals within the organization (e.g., employees, contractors) who may intentionally or unintentionally harm the organization.

### Attacks
Actions taken to exploit vulnerabilities are called Attacks.

**Types:**

- ``Active Attacks``: Direct actions to alter system resources or affect their operation. Examples: ``Data modification``, ``Denial of Service (DoS)``, ``Man-in-the-Middle (MitM)``.
- ``Passive Attacks``: Monitoring or eavesdropping on communications without affecting system resources. Examples: ``Eavesdropping on network traffic``, ``traffic analysis``.

### Assets
Assets are resources of value that need protection.

**Examples:**

- ``Data``: Sensitive information such as personal data, financial records, intellectual property.
- ``Hardware``: Physical devices such as servers, computers, networking equipment.
- ``Software``: Applications and operating systems essential for business operations.

## 1.4. Security Requirements

- ``Confidentiality``: Ensuring that information is not disclosed to unauthorized individuals.
- ``Integrity``: Maintaining the accuracy and completeness of data.
- ``Availability``: Ensuring that authorized users have access to information and resources when needed.
- ``Authentication``: Verifying the identity of users and devices.
- ``Authorization``: Granting permissions based on user roles and responsibilities.
- ``Non-repudiation``: Ensuring that actions or transactions cannot be denied after they have been performed.

## 1.5. Seeurity Design Principles

- ``Least Privilege``: Limiting access rights for users to the bare minimum they need to perform their work.
- ``Defense in Depth``: Implementing multiple layers of security controls to protect assets.
- ``Fail-Safe Defaults``: Defaulting to a secure state in the event of a failure.
- ``Economy of Mechanism``: Keeping the design as simple as possible.
- ``Complete Mediation``: Ensuring all accesses to resources are checked for authorization.
- ``Open Design``: Security should not depend on the secrecy of the design or implementation.
- ``Separation of Privilege``: Using multiple conditions to grant access to sensitive resources.
- ``Least Common Mechanism``: Minimizing the amount of shared mechanisms to reduce risk.
- ``Psychological Acceptability``: Designing security measures that are user-friendly and easy to understand.

## 1.6. Attack Surfaces and Attack Trees

### Attack Surfaces
The total points of entry or potential vulnerabilities through which an unauthorized user can try to enter data to or extract data from an environment.

**Components:**
- ``Network Attack Surface``: Includes vulnerabilities in network protocols, interfaces, and network devices like routers and firewalls.
- ``Software Attack Surface``: Encompasses vulnerabilities within the software applications, operating systems, and services running on a system.
- ``Physical Attack Surface``: Involves physical access points to systems, such as USB ports, workstations, and other hardware components.
- ``Human Attack Surface``: Targets human users through social engineering tactics like phishing and pretexting.

**Examples:**
- ``Network Attack Surface``: Open ports, unpatched vulnerabilities in network services.
- ``Software Attack Surface``: Buffer overflow vulnerabilities in applications, outdated software versions.
- ``Physical Attack Surface``: Unlocked server rooms, unattended workstations.
- ``Human Attack Surface``: Employees who can be tricked into divulging sensitive information.

**Minimizing Attack Surfaces:**
- ``Reduce Unnecessary Services``: Disable unused services and ports.
- ``Patch Management``: Regularly update and patch software to fix known vulnerabilities.
- ``Access Controls``: Implement strict access controls to limit who can access critical systems and data.
- ``User Training``: Educate employees on security best practices and social engineering tactics.

### Attack Trees
A hierarchical model that represents the various ways an attack can occur, showing the different paths that can be taken to achieve a malicious goal.

**Components:**

- ``Root Node``: Represents the ultimate goal of the attacker, such as gaining unauthorized access to a system.
- ``Branches``: Represent the different ways an attacker might try to achieve the goal.
- ``Leaf Nodes``: Represent specific actions or conditions that must be met to achieve a particular branch's goal.

**Purpose:**

- To systematically identify and analyze potential attack vectors.
- To prioritize security measures by identifying the most likely or most damaging attack paths.

**Examples:**

- ``Root Node Goal``: Gain administrative access to a server.
    - ``Branch 1``: Exploit a software vulnerability.
        - ``Leaf Node``: Find a buffer overflow in the web server software.
    - ``Branch 2``: Social engineering attack.
        - ``Leaf Node``: Phish an administrator's credentials.
    - ``Branch 3``: Physical access.
        - ``Leaf Node``: Break into the server room.

**Creating an Attack Tree:**

- ``Identify the Goal``: Define the main objective of the attacker.
- ``Map Out Possible Paths``: Identify all the possible ways the goal can be achieved.
- ``Analyze Paths``: Determine the likelihood and potential impact of each path.
- ``Prioritize Security Measures``: Focus on securing the most vulnerable and critical paths first.

## 1.7. Computer Security Strategy

- ``Risk Assessment``: Identifying and evaluating risks to the organization's information assets.
- ``Security Policy``: Establishing rules and practices to protect assets.
- ``Security Awareness Training``: Educating employees about security practices and policies.
- ``Incident Response``: Developing a plan to respond to security breaches or incidents.
- ``Continuous Monitoring``: Regularly reviewing and updating security measures to address emerging threats.
- ``Compliance``: Ensuring that the organization adheres to relevant laws, regulations, and standards.