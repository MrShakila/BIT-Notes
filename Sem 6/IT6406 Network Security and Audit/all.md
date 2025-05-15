# Computer and Network Security Concepts: IT6406 Network Security and Audit

## Computer Security Concepts

### Defining Computer Security

- Computer security is the protection of automated information systems to maintain integrity, availability, and confidentiality of resources (hardware, software, firmware, data, and telecommunications).

- This protection aims to meet applicable objectives.

### Key Security Principles

- Confidentiality:  Protecting information from unauthorized access and disclosure, including personal privacy and proprietary data.

- Integrity: Preventing unauthorized modification or destruction of information, ensuring authenticity and non-repudiation.

- Availability: Guaranteeing timely and reliable access to and use of information.

- Authenticity: Verifying the genuineness and trustworthiness of information, ensuring confidence in the validity of transmissions and originators.

- Accountability: Tracing actions of an entity uniquely back to that entity.

## The OSI Security Architecture

### Overview of the OSI Security Architecture

- The OSI security architecture provides a systematic way to define security requirements and characterize approaches to meet them.

- The International Telecommunication Union (ITU) recommends the X.800 Security Architecture for OSI.

- Many vendors have developed security features based on this standard.

### Key Components of the OSI Security Architecture

- Security attacks: Actions that compromise the security of information.

- Security mechanisms: Processes or devices designed to detect, prevent, or recover from security attacks.

- Security services: Processing or communication services enhancing the security of data processing systems and information transfers, using security mechanisms.

## Security Attacks

### Classifying Security Attacks

- Security attacks are categorized as passive or active.

- Passive attacks involve learning or using information without affecting system resources (e.g., eavesdropping).

- Active attacks attempt to alter system resources or affect their operation (e.g., modification, masquerade, replay, denial of service).

### Passive Attacks

- Passive attacks are like eavesdropping or monitoring transmissions.

- The goal is to obtain transmitted information.

- Two types: release of message contents and traffic analysis.

### Active Attacks

- Active attacks involve modification of data streams, creation of false streams, masquerading, replaying data, modifying messages, and denial-of-service attacks.

## Security Services

### Defining Security Services

- Security services are processing or communication services providing specific protection to system resources.

- X.800 divides these services into five categories.

### Types of Security Services

- Authentication: Verifying the authenticity of a communication.

- Access Control: Limiting and controlling access to host systems and applications.

- Data Confidentiality: Protecting transmitted data from passive attacks.

- Data Integrity: Ensuring messages are received as sent, without duplication, insertion, modification, reordering, or replays.

- Nonrepudiation: Preventing senders or receivers from denying a transmitted message.

## Security Mechanisms

### Categorizing Security Mechanisms

- Security mechanisms are categorized as specific or pervasive.

- Specific mechanisms are incorporated into protocol layers to provide OSI security services.

- Pervasive mechanisms are not specific to any OSI security service or protocol layer.

### Specific Security Mechanisms

- Encipherment: Transforming data into an unintelligible form using mathematical algorithms.

- Digital Signature: Cryptographic transformation proving data source and integrity.

- Access Control: Mechanisms enforcing access rights.

- Data Integrity: Mechanisms assuring data unit or stream integrity.

- Authentication Exchange: Ensuring entity identity through information exchange.

- Traffic Padding: Inserting bits to frustrate traffic analysis.

- Routing Control: Selecting physically secure routes.

- Notarization: Using a trusted third party to assure data exchange properties.

### Pervasive Security Mechanisms

- Trusted Functionality: Functionality perceived as correct based on security policy criteria.

- Security Label: Marking designating resource security attributes.

- Event Detection: Detecting security-relevant events.

- Security Audit Trail: Data for independent security audits.

- Security Recovery: Handling requests from mechanisms and taking recovery actions.

## Fundamental Security Design Principles

### Importance of Design Principles

- There are no foolproof techniques to completely exclude security flaws.

- Widely agreed design principles guide the development of protection mechanisms.

### Fundamental Security Design Principles

- Economy of mechanism: Simple and small security measures.

- Fail-safe defaults: Access decisions based on permission, not exclusion.

- Complete mediation: Every access checked against access control.

- Open design: Open, not secret, security mechanism design.

- Separation of privilege: Multiple privileges needed for access.

- Least privilege: Using only necessary privileges.

- Least common mechanism: Minimizing shared functions.

- Psychological acceptability: Mechanisms not interfering with user work.

- Isolation: Isolating public access systems from critical resources.

- Encapsulation: Isolation based on object-oriented functionality.

- Modularity: Separate, protected modules and modular architecture.

- Layering: Multiple, overlapping protection approaches.

- Least astonishment: User interface responding in expected ways.

## Attack Surfaces and Attack Trees

### Defining Attack Surfaces

- An attack surface consists of reachable and exploitable vulnerabilities in a system.

- Examples include open ports, services inside firewalls, code processing data, interfaces, and vulnerable employees.

### Categorizing Attack Surfaces

- Network attack surface: Vulnerabilities over networks (denial-of-service, disruption of links, intruder attacks).

- Software attack surface: Vulnerabilities in application, utility, or operating system code (web server software).

- Human attack surface: Vulnerabilities created by personnel (social engineering, human error, trusted insiders).

### Understanding Attack Trees

- An attack tree is a branching, hierarchical data structure representing potential techniques for exploiting vulnerabilities.

- The root node is the security incident goal.

- Subnodes represent subgoals, with leaf nodes representing attack initiation methods.

- Nodes are AND-nodes or OR-nodes.

- Attack trees effectively exploit information on attack patterns.

## A Model for Network Security

### The Basic Model

- A general model outlines four basic tasks in designing a security service:

	- Designing a security algorithm.

	- Generating secret information for the algorithm.

	- Developing methods for distributing and sharing secret information.

	- Specifying a protocol for principals to use the algorithm and secret information.

## Standards

### Standardization in Security

- Many security techniques and applications are standardized.

- Various organizations promote these standards.

### Key Organizations

- National Institute of Standards and Technology (NIST): A U.S. federal agency dealing with measurement science, standards, and technology.

- Internet Society (ISOC): A professional membership society responsible for Internet infrastructure standards.

- International Telecommunication Union (ITU): An international organization coordinating global telecom networks.

- International Organization for Standardization (ISO): A worldwide federation of national standards bodies.

# Transport Layer Security and Related Protocols

## Web Security Considerations

### Web Security Threats

- Integrity threats include data modification, Trojan horse browsers, and message traffic manipulation.  Consequences include information loss and system vulnerabilities. Countermeasures involve cryptographic checksums.

- Confidentiality threats involve eavesdropping and data theft.  Consequences include information and privacy loss. Countermeasures include encryption and web proxies.

- Denial-of-service threats involve disrupting service through various attacks. Consequences are disruptive and prevent users from working.  Prevention is difficult.

- Authentication threats include impersonation and data forgery. Consequences include misrepresentation of users and the acceptance of false information. Countermeasures involve cryptographic techniques.

### Web Traffic Security Approaches

- Network level security uses IP/IPSec to secure protocols like HTTP, FTP, and SMTP over TCP/IP.

- Transport level security uses SSL or TLS over TCP/IP to secure the same protocols.

- Application level security uses Kerberos and S/MIME to secure HTTP and SMTP over TCP/IP and UDP/IP.

## Transport Layer Security (TLS)

### TLS Overview and Architecture

- TLS version 1.2 (RFC 5246) is a general-purpose service implemented as a set of protocols relying on TCP.  It's often transparent to applications.

- TLS is not a single protocol but consists of two layers above TCP: the record protocol and higher-level protocols (handshake, change cipher spec, alert, heartbeat).

- Two key concepts are TLS sessions (associations between client and server) and TLS connections (transient peer-to-peer relationships within a session).

### TLS Session and Connection

- A TLS session is an association between a client and a server, created by the Handshake Protocol.  It defines cryptographic parameters shared across multiple connections.

- A TLS connection is a peer-to-peer relationship; each connection is associated with one session.  Multiple connections can exist within a single session.

### TLS Record Protocol

- The TLS Record Protocol provides confidentiality (using a shared secret key for encryption) and message integrity (using a shared secret key to generate a Message Authentication Code, MAC).

- The protocol operates by fragmenting application data, compressing it, adding a MAC, encrypting it, and appending a header.

### TLS Protocols: Change Cipher Spec, Alert, and Handshake

- The Change Cipher Spec Protocol uses a single message to update the cipher suite for a connection.

- The Alert Protocol conveys TLS-related alerts (warning or fatal) to the peer entity.  Messages are compressed and encrypted.

- The Handshake Protocol authenticates the client and server, negotiates encryption and MAC algorithms, and establishes cryptographic keys.  It occurs before application data transmission.

### Handshake Protocol Details

- The Handshake Protocol involves a series of messages exchanged between client and server.  Message types include hello_request, client_hello, server_hello, certificate, server_key_exchange, certificate_request, server_done, certificate_verify, client_key_exchange, and finished.

- The exchange has four phases: establishing security capabilities, server authentication and key exchange, client authentication and key exchange, and finishing.

### Handshake Protocol Phases

- Phase I (Establish Security Capabilities):  Establishes security parameters (protocol version, session ID, cipher suite, compression method, random numbers).

- Phase II (Server Authentication and Key Exchange): The server may send its certificate, key exchange parameters, and request a client certificate.

- Phase III (Client Authentication and Key Exchange): The client sends its certificate (if requested), key exchange parameters, and may send certificate verification.

- Phase IV (Finish): The client changes the cipher suite and sends a finished message; the server does the same.

### Handshake Protocol Cryptographic Computations

- The Handshake Protocol involves cryptographic computations: creating a shared master secret via key exchange (RSA or Diffie-Hellman), and generating cryptographic parameters from the master secret using a pseudo-random function.

### Heartbeat Protocol

- The Heartbeat Protocol runs on top of the TLS Record Protocol. It sends periodic signals to ensure the connection is alive and prevent closure by firewalls that don't tolerate idle connections.

### SSL/TLS Attacks

- Attacks can target the handshake protocol, record and application data protocols, and the Public Key Infrastructure (PKI).

### TLSv1.3

- TLSv1.3 removes support for compression, ciphers without authenticated encryption, static RSA and DH key exchange, 32-bit timestamps, renegotiation, the Change Cipher Spec Protocol, RC4, and MD5/SHA-224 hashes with signatures.

- It uses Diffie-Hellman or Elliptic Curve Diffie-Hellman for key exchange and allows for a "one round trip time" handshake.

## HTTPS

### HTTPS combines HTTP and SSL/TLS to provide secure communication between web browsers and servers.

### When HTTPS is used, the URL, document contents, browser form contents, cookies, and HTTP header contents are encrypted.

## Secure Shell (SSH)

### SSH Overview and Protocol Stack

- SSH is a protocol for secure network communications. It's designed to be simple and inexpensive to implement.

- The SSH protocol stack consists of three protocols running on top of TCP: the Transport Layer Protocol, the User Authentication Protocol, and the Connection Protocol.

### SSH Transport Layer Protocol

- Server authentication occurs at the transport layer, based on the server possessing a public/private key pair.

- Two trust models exist: a client-side database associating host names with public keys, or certification by a trusted Certificate Authority (CA).

### SSH User Authentication Protocol

- This protocol authenticates the client to the server.

- The message exchange involves several steps: client request, server validation, server response with authentication methods, client selection of a method, and authentication success or failure.

### SSH Authentication Methods

- Authentication methods include public key, password, and host-based authentication.

### SSH Connection Protocol

- The Connection Protocol runs on top of the SSH Transport Layer Protocol and uses a secure authentication connection (a tunnel) to multiplex logical channels.

- Four channel types are recognized: session, X11, forwarded-tcpip, and direct-tcpip.

### SSH Connection Protocol Message Exchange

- The Connection Protocol uses messages like SSH_MSG_CHANNEL_OPEN, SSH_MSG_CHANNEL_OPEN_CONFIRMATION, and SSH_MSG_CHANNEL_DATA to manage channel opening, data transfer, and closing.

### SSH Port Forwarding

- SSH port forwarding converts insecure TCP connections into secure SSH connections (SSH tunneling).

- SSH supports local and remote port forwarding.

# User Authentication and Network Access Control

## Remote User Authentication Principles

### Identification and Verification

- User authentication is fundamental for access control and accountability.

- The process involves two steps: identification (presenting an identifier) and verification (corroborating the binding between the entity and the identifier).

- A user login scenario illustrates these steps.

### Means of Authentication

- Something the individual knows (passwords, PINs, answers to security questions).

- Something the individual possesses (cryptographic keys, smart cards, tokens).

- Something the individual is (static biometrics like fingerprints, retina scans, facial recognition).

- Something the individual does (dynamic biometrics like typing patterns or voice recognition).

### Mutual Authentication

- Mutual authentication protocols allow communicating parties to verify each other's identity and exchange session keys.

- Key issues are confidentiality and timeliness.

- Replay attacks are a significant concern, requiring mechanisms like timestamps and challenge/response to mitigate them.  Examples of replay attacks are provided.  Methods for preventing replay attacks are discussed.

### One-Way Authentication

- In one-way authentication, the sender and receiver don't need to be online simultaneously.

- The email header must be in clear text for store-and-forward protocols to function.

- The mail-handling protocol doesn't require access to the message's plaintext.

- Encrypted emails enable one-way authentication.

## Remote User Authentication Using Symmetric Encryption

### Mutual Authentication

- A two-level hierarchy of symmetric encryption keys provides confidentiality in distributed environments.

- The Needham-Schroeder protocol, while using a trusted Key Distribution Center (KDC), is vulnerable to replay attacks.  The protocol is described with examples.

- Denning's modification adds timestamps to address replay vulnerabilities, but it remains susceptible to suppress-replay attacks if clocks aren't synchronized.  The modified protocol is described with examples.

- A more robust solution is presented to address these weaknesses.  The protocol is described with examples.

### One-Way Authentication

- A limitation is that the sender cannot ensure the recipient is online.

- The protocol doesn't inherently protect against replays; timestamps can help mitigate this.  The protocol is described with examples.

## Kerberos

### A Simple Authentication Dialogue

- Kerberos addresses the problem of users accessing services on servers in an open distributed environment where workstations cannot be fully trusted.

- In an unprotected environment, any client can request service from any server, leading to impersonation risks.

- A centralized authentication server (AS) knowing all user/service passwords is proposed, but this has security and scalability issues.

### A More Secure Authentication Dialogue

- A more secure approach uses an authentication server (AS) and a ticket-granting server (TGS) to minimize password entry and enhance security.

- Replay attacks and lifetime issues remain concerns.

- The system needs to verify that the person using a ticket is the same person to whom it was issued.

- Server authentication to users might also be necessary.

### The Version 4 Authentication Dialogue

- The version 4 dialogue is described in detail, outlining the steps involved in obtaining ticket-granting and service-granting tickets, and client/server authentication.  The protocol is described with diagrams and examples.

### Kerberos Realms and Multiple Kerberi

- The Kerberos server must store user IDs and hashed passwords of all users.

- The Kerberos server shares secret keys with each server.

- Interoperating realms share secret keys between their Kerberos servers.

### Differences Between Version 4 and 5

- Kerberos version 4 has environmental shortcomings (encryption system dependence, internet protocol dependence, message byte ordering, ticket lifetime, authentication forwarding, inter-realm authentication).

- Version 5 addresses these deficiencies with double encryption, PCBC encryption, improved session key management, and enhanced password protection.

### The Version 5 Authentication Dialogue

- The version 5 authentication dialogue is described, detailing the improvements over version 4 in obtaining ticket-granting and service-granting tickets, and client/server authentication.  The protocol is described with examples.

## Remote User Authentication Using Asymmetric Encryption

### Mutual Authentication

- This method uses asymmetric encryption for mutual authentication.  The protocol is described with examples.

### One-Way Authentication

- If confidentiality is paramount, a more efficient approach is presented.

- If authentication is the main concern, a digital signature suffices.

## Federated Identity Management

### Identity Management

- Identity management is a centralized, automated approach to provide enterprise-wide access to resources.

- Single sign-on (SSO) is a central concept.

### Identity Federation

- Identity federation extends identity management across multiple security domains.

- It involves agreements, standards, and technologies enabling portability of identities, attributes, and entitlements across enterprises and applications.

- Federated identity management uses standards for secure identity exchange across domains or heterogeneous systems.

## Network Access Control

### Elements of a Network Access Control System

- The system consists of an access requestor (AR), a policy server, and a network access server (NAS).

## Extensible Authentication Protocol

### Authentication Methods

- EAP-TLS (EAP Transport Layer Security)

- EAP-TTLS (EAP Tunneled TLS)

- EAP-GPSK (EAP Generalized Pre-Shared Key)

- EAP-IKEv2

### Network Access Enforcement Methods

- IEEE 802.1X

- Virtual local area networks (VLANs)

- Firewall

- DHCP management

### EAP Protocol Exchanges

- The exchange process between EAP peer, EAP authenticator, and authentication server (RADIUS) is illustrated.

### EAP Message Flow in Pass Through Mode

- The message flow in pass-through mode is illustrated, showing the sequence of EAP requests and responses.

## IEEE 802.1X Port-Based Network Access Control

### The process is illustrated, showing the EAPOL messages exchanged between the EAP peer, EAP authenticator, and authentication server (RADIUS).

# Virtual Private Networks (VPNs) and IP Security (IPsec)

## Introduction to Virtual Private Networks

### Requirement of Remote Access and Private Communication

- Remote access allows organizations to access resources remotely, a common need.

- Site-to-site access connects different branches of an organization (intranet) or different organizations (extranet).  Examples include a bank connecting its head office to branches or a bank giving access to a software development company.

### Private Communication Technologies and Evolution

- Dedicated network links, while providing private communication, are not scalable, expensive, inflexible for remote connectivity, and costly to upgrade.

### What is a Virtual Private Network (VPN)?

- A VPN is a logical communication link that carries private traffic over a public network.

- Access is restricted to defined users.

- Communication is private, not necessarily encrypted (e.g., MPLS).

- Communication is abstracted from the physical substrate, remaining unchanged despite physical layer technology changes.

### Practical VPN Applications

- Ubiquitous access to corporate resources (e.g., working while traveling).

- Accessing private corporate services from remote locations (e.g., a corporate financial system).

- Controlled/private access from many locations by different parties (e.g., a software vendor accessing from their site).

- Long-distance connectivity where leased lines are not feasible (e.g., international employees/clients).

- Infrastructure requirements such as extended LANs (e.g., Oracle DB deployments).

### VPN Implementations

- MPLS (Multi-Protocol Label Switching): Not secure. Uses a labeling mechanism for network isolation. Can be implemented as a full mesh but is limited by service provider networks.

- GRE Tunnels (Generic Routing Encapsulation): Not secure. Uses encapsulation for network isolation. Can forward multicast traffic, unlike other VPN protocols.

- PPTP (Point-to-Point Tunneling Protocol): Secure but considered vulnerable. Introduced by Microsoft, supported by many operating systems. Uses MS-CHAP authentication.  Uses GRE for encapsulation; encryption varies by implementation. Point-to-point connectivity, works only on IP networks.

- L2TP (Layer 2 Tunneling Protocol): Provides PPTP functionality but works on networks other than just IP. Does not provide encryption or authentication; requires IPsec for these services. Uses processes similar to PPTP for encapsulation.

- IPSecurity: Secure and de facto protocol for secure VPN implementations.

- TLS (SSL VPN): Secure.

## IP Security Overview

### Applications of IPsec

- Secure branch office connectivity over the internet.

- Secure remote access over the internet.

- Establishing extranet and intranet connectivity with partners.

- Enhancing electronic commerce security.

### Benefits of IPsec

- When implemented in a firewall or router, it provides strong security for all traffic crossing the perimeter without impacting internal traffic.

- It's resistant to bypass if all external traffic must use IPsec and the firewall is the only entry point.

- It operates below the transport layer (TCP, UDP), making it transparent to applications and end-users.

- It can provide security for individual users.

### Routing Applications

- IPsec ensures that router advertisements, neighbor advertisements, and redirect messages come from authorized routers, preventing forged routing updates.

### IPsec Services

- IPsec provides security services at the IP layer by selecting security protocols, algorithms, and cryptographic keys.

- Two protocols provide security:

	- Authentication Header (AH): An authentication protocol.

	- Encapsulating Security Payload (ESP): A combined encryption/authentication protocol.

- RFC 4301 lists the following services: access control, connectionless integrity, data origin authentication, rejection of replayed packets, confidentiality (encryption), and limited traffic flow confidentiality.

### Transport and Tunnel Modes

- Both AH and ESP support transport and tunnel modes.

- Transport mode is used for end-to-end communication between two hosts. ESP encrypts the IP payload (but not the header); AH authenticates the payload and selected header portions.

- Tunnel mode protects site-to-site/network-to-network communication. ESP encrypts the entire inner IP packet; AH authenticates the entire inner packet and selected portions of the outer header.

## IP Security Policy

### Security Associations

- A security association is a one-way logical connection providing security services. Two are needed for two-way secure exchange.  It's uniquely identified by the Security Parameters Index (SPI), IP destination address, and security protocol identifier.

### IPsec Architecture

- The architecture diagram shows the interaction between the Security Policy Database (SPD), Security Association Database (SAD), IKEv2 (key exchange), and IPsecv3.

### Security Association Database

- Defines parameters associated with each security association (SA).  Parameters include: Security Parameter Index, Sequence Number Counter, Sequence Counter Overflow, Anti-Replay Window, AH Information, ESP Information, Lifetime of the SA, IPsec Protocol Mode, and Path MTU.

### Security Policy Database

- Relates IP traffic to specific SAs (or bypasses IPsec).  Selectors determining an SPD entry include: Remote IP Address, Local IP Address, Next Layer Protocol, Name, and Local and Remote Ports.

### IP Traffic Processing

- Diagrams illustrate the processing of outbound and inbound packets, showing how the SPD and SAD are used to determine whether to process packets using AH/ESP or bypass IPsec.

## Encapsulating Security Payload (ESP)

### ESP provides confidentiality, data origin authentication, connectionless integrity, anti-replay service, and traffic flow confidentiality.

### ESP Format, Encryption and Authentication Algorithms, Padding, and Anti-Replay Service

- These are key components of the ESP protocol.  Diagrams illustrate packet structure before and after applying ESP in transport and tunnel modes.

## Internet Key Exchange

### Key management involves determining and distributing secret keys.

### IPsec supports manual and automated key management.

### The default automated protocol is ISAKMP/Oakley, consisting of the Oakley Key Determination Protocol and the Internet Security Association and Key Management Protocol (ISAKMP).

## Cryptographic Suites

### A cryptographic suite defines a set of cryptographic algorithms, parameters, and key sizes.  The presentation shows examples of VPN-A and VPN-B suites, specifying algorithms used for ESP encryption, ESP integrity, IKE encryption, IKE PRF, IKE integrity, and IKE DH group.

# Network Perimeter Security: Intrusion Detection and Prevention

## Understanding Intruders

### Intruder Classification and Behavior

- Intruders are often referred to as hackers or crackers.

- Three main classes of intruders exist: masqueraders, misfeasors, and clandestine users.

- Each intruder class exhibits distinct behavior patterns, including those of hackers, criminal enterprises, and internal threats.  Examples of these patterns are detailed, outlining specific techniques used by each type of intruder.

### Intrusion Techniques

- The primary objective of an intruder is to gain unauthorized system access or escalate privileges.

- Initial attacks often exploit system or software vulnerabilities to create backdoors.

- Intruders may also attempt to acquire passwords using various methods, such as trying default passwords, short passwords, dictionary words, or information gathered about users.  Other techniques include using Trojan horses or tapping communication lines.

## Intrusion Detection Systems

### Importance and Approaches

- Timely intrusion detection allows for swift identification and removal of intruders before significant damage occurs.

- Effective intrusion detection systems act as deterrents, preventing future intrusions.

- Intrusion detection facilitates the collection of valuable information about intrusion techniques, strengthening prevention measures.

- Approaches to intrusion detection include statistical anomaly detection (threshold and profile-based) and rule-based detection (anomaly detection and penetration identification).

### Audit Records and Statistical Anomaly Detection

- Audit records serve as a fundamental tool for intrusion detection.  Two main approaches are used: native audit records and detection-specific audit records.  Each audit record contains specific fields (subject, action, object, exception-condition, resource-usage, and timestamp).

- Statistical anomaly detection uses threshold analysis and profile-based systems.  Threshold analysis alone is often ineffective against sophisticated attacks.  Profile-based systems characterize past user behavior to detect significant deviations.  This approach relies on analyzing audit records.  Metrics used include counters, gauges, interval timers, and resource utilization.  Tests such as mean and standard deviation, Markov processes, time series analysis, and operational analysis are used to determine if current activity falls within acceptable limits.

### Rule-Based Intrusion Detection and the Base-Rate Fallacy

- Rule-based techniques detect intrusions by observing system events and applying rules to determine suspicious activity.  Examples of such rules are provided.

- The base-rate fallacy highlights the importance of balancing intrusion detection effectiveness with an acceptable false alarm rate.  High false alarm rates lead to system managers ignoring alerts or wasting time analyzing false positives.

### Distributed Intrusion Detection and Honeypots

- Distributed intrusion detection systems face design challenges, including handling diverse audit record formats and ensuring data integrity and confidentiality during transmission.  Centralized and decentralized architectures are possible.

- Honeypots are decoy systems designed to lure attackers away from critical systems, collect information about their activity, and prolong their engagement to allow for response.  They contain fabricated information that legitimate users wouldn't access.

## Intrusion Prevention Systems

### While intrusion detection systems can be passive, intrusion prevention systems should be active inline systems.

### In addition to intrusion detection functions, intrusion prevention systems actively prevent attacks by dropping malicious packets, blacklisting malicious sources, resetting malicious network connections, and configuring firewalls to prevent future attacks.

## Firewalls

### Need for Firewalls and Design Goals

- Organizations require internet connectivity for operations and service provision but this exposes them to external threats.

- Firewalls control network access, ensuring that all traffic passes through them, blocking unauthorized access.

- Firewalls only allow authorized traffic, as defined by security policies.

- Firewalls themselves must be resistant to penetration, often requiring hardened systems and secured operating systems.

### Firewall Types and Basing

- Firewall types include packet filtering firewalls, stateful inspection firewalls, application-level gateways, and circuit-level gateways.  Each type is described in detail.

- Firewall basing options include bastion hosts (critical strong points in network security), host-based firewalls (software modules securing individual hosts), and personal firewalls (controlling traffic between personal computers and networks).

### Firewall Location and Configurations

- DMZ networks use external firewalls at the network edge and internal firewalls to protect the internal network.

- Virtual Private Networks (VPNs) use encryption and special protocols to secure communication over insecure networks.

- Distributed firewalls combine stand-alone firewall devices and host-based firewalls under central administrative control.

## Unified Threat Management (UTM)

### UTM provides multiple security features and services on a single device or service.

### It protects against various security threats.

### It is also known as Next-Generation Firewalls.

### UTM includes features such as anti-virus, anti-spam, content filtering, and web filtering.

### Data Leakage Prevention (DLP) and Deep Packet Inspection (DPI)

- DLP detects and prevents data breaches and leakages.

- DPI uses known intrusion signatures to detect abnormal network traffic in hardware or software systems.

# Email and Domain Name System Security

## Email Security

### Internet Mail Architecture

- Email components include the Message User Agent (MUA), Mail Submission Agent (MSA), Message Transfer Agent (MTA), Mail Delivery Agent (MDA), and Message Store (MS).

- The MTA relays messages between mail servers using SMTP.

- The MUA interacts with the user and the MSA submits messages to the MTA.  The MDA delivers messages to the MS.

### Email Formats

- Email message structure, as defined in RFC 5322, consists of header lines and a text body separated by a blank line.  Headers contain keywords like From, To, Subject, and Date.

- Multipurpose Internet Mail Extension (MIME) extends RFC 5322 to address limitations in SMTP, handling various content types.

- MIME header fields include MIME-Version, Content-Type, Content-Transfer-Encoding, Content-ID, and Content-Description.

### Email Threats and Comprehensive Email Security

- Email security threats are classified as authenticity-related, integrity-related, confidentiality-related, and availability-related.

- Standardized protocols addressing these threats include STARTTLS, S/MIME, DNSSEC, DANE, SPF, DKIM, and DMARC.

### S/MIME

- Secure/Multipurpose Internet Mail Extension (S/MIME) enhances the MIME standard with security features.

- It uses RSA technology for authentication and AES-128 with CBC for confidentiality.

- S/MIME provides compression and ensures email compatibility across various systems by converting 8-bit binary streams to printable ASCII.

- S/MIME message content types include Data, SignedData, EnvelopedData, and CompressedData.

### Pretty Good Privacy (PGP)

- PGP is an email security protocol with similar functionality to S/MIME.

- OpenPGP is a standardized version of PGP.

- Key certification differs: S/MIME uses X.509 certificates from Certificate Authorities, while OpenPGP uses a web-of-trust model where users generate their own keys.

- OpenPGP does not include the sender's public key with each message.

## Domain Name System Security

### DNSSEC

- The Domain Name System (DNS) maps domain names to IP addresses.

- DNS Security Extensions (DNSSEC) secures data exchange in DNS using digital signatures.

- DNSSEC protects against forged or altered DNS resource records, providing data origin authentication and data integrity verification.

### DNS-Based Authentication of Named Entities (DANE)

- DANE addresses the risk of compromised Certificate Authorities (CAs) issuing false certificates.

- It replaces reliance on CA security with reliance on DNSSEC security.

- DANE defines the TLSA DNS record type for securely authenticating SSL/TLS certificates.

- DANE can enhance email security when used with SMTP over TLS.

### Sender Policy Framework (SPF)

- SPF standardizes how sending domains identify and assert their mail senders.

- It prevents unauthorized hosts from using a domain name in email headers.

- SPF provides a protocol for Administrative Management Domains (ADMDs) to authorize hosts.

- SPF makes it difficult for senders to spoof their domain.

### DomainKeys Identified Mail (DKIM)

- DKIM cryptographically signs email messages, allowing domains to claim responsibility.

- DKIM authentication is transparent to the end user.

- The sender's private key signs the message, and the receiver's Mail Delivery Agent (MDA) verifies it using the public key retrieved via DNS.

### Domain-Based Message Authentication, Reporting, and Conformance (DMARC)

- DMARC allows senders to specify policies for handling their mail, the types of reports receivers can send, and the reporting frequency.

- It uses SPF, DKIM, and identifier alignment to verify email authenticity.

- DMARC reporting provides feedback on SPF, DKIM, identifier alignment, and message disposition policies.

- Reports include the sender's DMARC policy, message disposition, SPF and DKIM results, results classified by sender subdomain, and the sending/receiving domain pair.

# Wireless Network Security: An Overview

## Wireless Security

### Factors Contributing to Higher Security Risks in Wireless Networks

- Wireless networks are more susceptible to security breaches compared to wired networks due to several factors.

- The open nature of the wireless channel makes it easier for unauthorized access.

- The mobility of wireless devices increases the risk of exposure to insecure networks.

- Shared resources in wireless networks can be vulnerable to attacks.

- The accessibility of wireless networks makes them attractive targets for malicious actors.

### Wireless Network Threats

- Accidental association with unauthorized networks poses a security risk.

- Malicious associations with rogue access points can compromise network security.

- Ad hoc networks, lacking central management, are vulnerable to various attacks.

- Nontraditional networks, often lacking robust security measures, increase the attack surface.

- Identity theft through MAC spoofing is a significant threat.

- Man-in-the-middle attacks intercept and manipulate communication.

- Denial-of-service (DoS) attacks disrupt network availability.

- Network injection attacks introduce malicious code into the network.

### Wireless Security Measures

- Securing wireless transmission is crucial to prevent eavesdropping and data breaches.

- Signal-hiding techniques reduce the range and visibility of wireless signals.

- Encryption protects data transmitted over the wireless network.

- Securing wireless access points involves configuring strong passwords and encryption protocols.

- Securing wireless networks requires a multi-layered approach, including encryption, antivirus software, firewalls, and access control.

## Mobile Device Security

### Security Threats Related to Mobile Devices

- Lack of physical security control increases the risk of theft and unauthorized access.

- Using untrusted mobile devices introduces vulnerabilities to malware and data breaches.

- Connecting to untrusted networks exposes devices to attacks and data theft.

- Using applications from unknown sources can lead to malware infections and data compromise.

- Accessing untrusted content can expose devices to malware and phishing attacks.

- Using location services without proper security measures can compromise user privacy.

### Mobile Device Security Strategies

- Device security measures include enabling auto-lock, password or PIN protection, and disabling auto-complete features.

- Enabling remote wipe allows for the secure deletion of data in case of loss or theft.

- Keeping the operating system and software up-to-date is essential for patching security vulnerabilities.

- Sensitive data should be encrypted or prohibited from storage on the device.

- Traffic security, through encryption and authentication, protects data in transit.

- Barrier security measures protect the network from unauthorized access.

## IEEE 802.11 Wireless LAN Overview

### IEEE 802 Protocol Architecture

- The IEEE 802 standard defines the architecture for wireless local area networks (WLANs).

- The physical layer specifies frequency bands and antenna characteristics.

- The media access control (MAC) layer handles data transmission and reception.  It assembles data into frames with addresses and error-detection fields during transmission and disassembles frames, performing address recognition and error detection upon reception.

### IEEE 802.11 Network Components and Architectural Model

- The IEEE 802.11 architecture consists of several components, including access points (APs) and stations (STAs).

- Access points act as central points for wireless communication within a basic service set (BSS).

- Multiple BSSs can be interconnected through a distribution system.

### IEEE 802.11 Services

- The IEEE 802.11 standard defines various services, including association, authentication, de-authentication, disassociation, distribution, integration, MSDU delivery, privacy, and re-association.  These services ensure secure and reliable communication within the WLAN.

## IEEE 802.11i Wireless LAN Security

### Security Protocols in IEEE 802

- Several security protocols are available within the IEEE 802 standard to protect wireless networks.

- Wired Equivalent Privacy (WEP) is an older protocol with known vulnerabilities.

- Wi-Fi Protected Access (WPA) is an improved protocol offering enhanced security.

- Robust Security Network (RSN) is the most secure protocol, providing strong authentication and encryption.

### 802.11i RSN Security Specification

- The 802.11i RSN security specification defines key services for secure wireless communication.

- Authentication verifies the identity of wireless devices.

- Access control restricts access to the network based on authentication.

- Privacy with message integrity ensures data confidentiality and prevents unauthorized modification.

### IEEE 802.11i Phases of Operation

- The IEEE 802.11i standard defines several phases of operation to establish and maintain a secure connection.

- Discovery involves access points advertising their security policies using Beacons and Probe Responses.

- Authentication involves wireless stations and the authentication server verifying their identities.

- Key generation and distribution involves negotiating cryptographic keys between wireless stations and access points.

- Protected data transfer ensures secure exchange of data frames through the access point.

- Connection termination securely ends the connection and restores the network to its original state.

# Cloud Security Fundamentals

## Cloud Computing Overview

### Defining Cloud Computing

- Many organizations are shifting IT operations to internet-connected infrastructure (cloud computing).

- NIST defines cloud computing as a model enabling ubiquitous, convenient, on-demand network access to a shared pool of configurable computing resources.  These resources (networks, servers, storage, applications, and services) are rapidly provisioned and released with minimal management effort.

- Essential characteristics include broad network access, rapid elasticity, measured service, on-demand self-service, and resource pooling.

### Cloud Computing Service Models (NIST)

- Software as a Service (SaaS): Consumers use the provider's applications running on a cloud infrastructure, accessible through a thin client interface.  This simplifies software installation, maintenance, and upgrades.

- Platform as a Service (PaaS): Consumers deploy applications onto the cloud infrastructure using programming languages and tools supported by the provider.  PaaS often provides middleware services like databases.

- Infrastructure as a Service (IaaS): Consumers provision processing, storage, networks, and other fundamental computing resources to deploy and run arbitrary software.  This allows combining basic computing services to build adaptable systems.

### Cloud Computing Deployment Models (NIST)

- Public cloud: Infrastructure is available to the general public or a large industry group, owned by an organization selling cloud services. The provider is responsible for infrastructure and data control.

- Private cloud: Infrastructure is operated solely for an organization, managed by the organization or a third party, and may be on or off-premise. The provider is responsible only for the infrastructure.

- Community cloud: Infrastructure is shared by several organizations with shared concerns (mission, security, policy, compliance). It may be managed by the organizations or a third party.

- Hybrid cloud: A composition of two or more clouds (private, community, or public) bound by standardized or proprietary technology enabling data and application portability.

## Cloud Security Risks and Countermeasures

### Cloud-Specific Security Threats

- Abuse and nefarious use of cloud computing (easy registration and free trials enable attacks).

- Insecure interfaces and APIs (security and availability depend on basic API security).

- Malicious insiders (organizations relinquish direct control, increasing trust in the cloud provider).

- Shared technology issues (underlying infrastructure components not designed for strong isolation in a multi-tenant architecture).

- Data loss or leakage (most devastating impact of a security breach).

- Account or service hijacking (stolen credentials enable access to critical areas).

- Unknown risk profile (clients pass control to the cloud provider on many security issues).

### Countermeasures for Cloud Security Threats

- Abuse and nefarious use: stricter registration, enhanced fraud monitoring, network traffic introspection, monitoring public blacklists.

- Insecure interfaces and APIs: analyze security models, implement strong authentication and access controls with encryption, understand dependency chains.

- Malicious insiders: enforce strict supply chain management, comprehensive supplier assessment, specify human resource requirements, require transparency and compliance reporting, determine breach notification processes.

- Shared technology issues: implement security best practices, monitor for unauthorized changes, promote strong authentication and access control, enforce SLAs for patching and vulnerability remediation, conduct vulnerability scanning and configuration audits.

- Data loss or leakage: implement strong API access control, encrypt data in transit, analyze data protection at design and run time, implement strong key generation, storage, management, and destruction practices.

- Account or service hijacking: prohibit credential sharing, leverage two-factor authentication, employ proactive monitoring, understand security policies and SLAs.

- Unknown risk profile: disclose applicable logs and data, disclose infrastructure details, monitor and alert on necessary information.

## Data Protection in the Cloud

### Data Compromise Methods and Increased Risk

- Data can be compromised through deletion, alteration, unlinking, loss of encoding keys, or unauthorized access.

- The threat of data compromise increases in the cloud due to the number and interactions between risks and challenges unique to the cloud environment.

### Data Protection Strategies

- Data must be secured at rest, in transit, and in use, with controlled access.

- Encryption protects data in transit, but involves key management responsibilities.

- Access control techniques can be enforced, but the cloud provider is involved.

- For data at rest, encrypting the database and storing only encrypted data (with the provider having no access to the key) is ideal.  Corruption and denial-of-service attacks remain a risk.

## Cloud Security as a Service (SecaaS)

### SecaaS Overview and Services

- SecaaS is a package of security services offered by a service provider, offloading security responsibility from the enterprise.

- Typical services include authentication, antivirus, antimalware, intrusion detection, and security event management.

- In cloud computing, SecaaS is a segment of a cloud provider's SaaS offering.

### SecaaS Categories

- Identity and access management (IAM): manages access to resources by verifying identity and granting appropriate access levels. Includes provisioning and deprovisioning.

- Data loss prevention (DLP): monitors, protects, and verifies data security at rest, in motion, and in use.  Can be implemented by the client or the cloud service provider.

- Web security: real-time protection via on-premise software or cloud-based proxying, adding a layer of protection against malware.  May include usage policy enforcement, data backup, traffic control, and web access control.

- Email security: controls inbound and outbound email, protecting against phishing and malicious attachments, enforcing corporate policies. May incorporate digital signatures and encryption.

- Security assessments: third-party audits of cloud services.  The cloud service provider can provide tools and access points.

- Intrusion management: encompasses intrusion detection, prevention, and response using intrusion detection systems (IDSs) and intrusion prevention systems (IPSs).

- Security information and event management (SIEM): aggregates log and event data to provide real-time reporting and alerting.

- Encryption: a pervasive service for data at rest, email traffic, network management information, and identity information.  Involves key management, VPN services, application encryption, and data access control.

- Business continuity and disaster recovery: ensures operational resiliency with backup at multiple locations, failover, and disaster recovery facilities.  Includes flexible infrastructure, redundancy, monitored operations, geographically distributed data centers, and network survivability.

- Network security: allocates access, distributes, monitors, and protects underlying resource services. Includes perimeter and server firewalls and denial-of-service protection.

## Addressing Cloud Computing Security Concerns

### Cloud Security's Ongoing Importance

- Cloud computing security remains crucial as more businesses incorporate cloud services.

- Security failures can negatively impact business interest, prompting providers to improve security mechanisms.

### NIST Security Controls

- NIST recommends various security controls relevant to cloud computing environments, categorized as technical, operational, and management controls.  These include access control, audit and accountability, identification and authentication, system and communication protection, awareness and training, configuration and management, contingency planning, incident response, maintenance, media protection, physical and environmental protection, personnel security system and information integrity, certification, accreditation, security assessment, planning risk assessment, and system and services acquisition.

# IT Infrastructure Auditing Concepts

## The Need for Information Systems Security Compliance

### Understanding IT Security Assessments

- Assessing IT security involves managing risk through identifying and categorizing information systems, selecting and implementing appropriate security controls, assessing their effectiveness, authorizing systems based on accepted risks, and continually monitoring controls.  This is a continuous cycle.

- Security controls encompass physical, procedural, and technical mechanisms to safeguard systems. Assessments identify weaknesses, confirm remediation, prioritize mitigation, provide assurance of effective controls, and support future budgetary planning.

- Personnel conducting assessments can be internal or external. NIST provides a framework (Special Publication 800-53A) for effective assessment plans, outlining objectives, methods, and objects.  An example is analyzing unsuccessful logon attempts.

### Understanding IT Security Audits

- An IT security audit independently assesses an organization's policies, controls, and activities.  It's crucial for ensuring compliance and identifying vulnerabilities.

- Audits can cover organizational management, compliance with laws and guidelines, application usage, and technical infrastructure.

- Effective audit programs aim to provide objective reviews, reasonable assurance of effective controls, and recommendations for improvement.  Auditors should be independent of the systems they audit.  Internal auditors are employed by the organization, while external auditors are independent.

### Compliance and the Differences Between Audits and Assessments

- Internal compliance focuses on following an organization's own policies, while external compliance involves adhering to external regulations and guidelines.  Meeting compliance involves interpreting regulations, identifying gaps, devising and executing plans to close those gaps.

- Compliance is closely linked to risk management and governance.

- Audits differ from assessments in their rigor and process. Audits follow a more structured approach and require auditor independence from the systems being audited.  Assessments can be less formal and consider future expectations.  Successful audits often lead to certification.

### Non-Compliance Consequences

- Non-compliance can result in financial, reputational, and operational consequences.

- Costs associated with security breaches include discovery, notification, lost productivity, opportunity costs, regulatory fines, restitution, and additional security/audit requirements.

## Auditing Standards and Frameworks

### The Importance of Frameworks in Auditing

- A framework provides structure and consistency in complex situations.  In IT, it offers a consistent system of controls for departments to follow and a consistent approach for auditors.

### Using Standards in Compliance Auditing

- Different standards (e.g., COSO, COBIT, ISO/IEC 27000, NIST 800-53, Cybersecurity Framework) have varying attributes like depth, breadth, flexibility, reasoning, prioritization, and industry acceptance.

- Successful auditing requires agreement between the auditor and organization on a specific standard.  Key recommendations include selecting a standard that is easily followed, employing it consistently, and choosing a flexible standard.

### Hierarchy of Standards and Compliance

- A hierarchical structure exists, with regulations at the top (e.g., SOX, HIPAA, GLBA), followed by governance frameworks (COSO, COBIT), control objectives (COBIT), and finally controls (ISO/IEC 27002, NIST 800-53).  Each level has associated personnel responsible for its implementation and oversight.

### COSO Framework

- COSO (Committee of Sponsoring Organizations) provides a structure for examining and applying risk-based processes.

- The COSO ERM framework has eight components across four objectives: strategic, operations, reporting, and compliance.

- The framework identifies eight interrelated parts of an organization's management processes: internal environment, objective setting, event identification, risk assessment, risk response, control activities, information and communication, and monitoring.

### COBIT Framework

- COBIT (Control Objectives for Information and Related Technology) aligns IT with business requirements by mapping controls to business needs, classifying IT activities, identifying key resources, and defining a framework for control objectives.

- COBIT 5 principles include meeting stakeholder needs (benefits, risk, and resource optimization), covering the enterprise end-to-end (through governance enablers and scope), applying a single integrated framework, enabling a holistic approach, and separating governance from management.

### ISO/IEC Standards and NIST 800-53

- ISO (International Organization for Standardization) provides standards and guidance on information security.  ISO/IEC 27000 series offers guidance on implementing, designing, and auditing information security management systems (ISMS).

- ISO/IEC 27001 specifies requirements for establishing, implementing, maintaining, and improving ISMS.  ISO/IEC 27002 provides a code of practice for information security management.

- NIST 800-53 provides a comprehensive catalog of security controls grouped into 17 families (access control, awareness training, audit and accountability, etc.).

### Cybersecurity Framework

- The Cybersecurity Framework consists of three components: the Framework Core, the Framework Profile, and the Framework Implementation Tiers.  It includes categories across five functions: identify, protect, detect, respond, and recover.

## Planning an IT Infrastructure Audit

### Defining Scope, Objectives, Goals, and Frequency

- When defining the scope, consider controls and processes across the seven domains of IT infrastructure (user, workstation, LAN, LAN-to-WAN, WAN, remote access, system/application).  Relevant resources include data, applications, technology, facilities, and personnel.

### Identifying Critical Requirements

- Critical requirements include implementing security controls (management, operational, and technical) and protecting privacy data.

### Assessing IT Security

- This involves risk management, threat analysis, vulnerability analysis, and defining an acceptable security baseline.

### Obtaining Information and Resources

- This includes defining the existing IT security policy framework, documenting IT infrastructure configurations, and conducting interviews with key IT personnel.

### Mapping to Seven Domains

- The seven domains of a typical IT infrastructure are user, workstation, LAN, LAN-to-WAN, WAN, remote access, and system/application.

### Identifying and Testing Monitoring Requirements

- Continuous monitoring and evaluation of the control environment helps answer questions about IT performance measurement, management effectiveness, linking IT performance to business goals, and the adequacy of confidentiality, integrity, and availability controls.

### Identifying Critical Security Control Points

- SANS Consensus Audit Guidelines (CAG) published in 2009 provide guidance on critical security control points.

### Building a Project Plan

- This involves assigning appropriate personnel and utilizing tools such as electronic work papers, project management software, flowcharting software, open issue tracking software, and an audit department website.

## Conducting and IT Infrastructure Audit

### Identifying Minimum Acceptable Risk and Baseline Definitions

- Determining an appropriate set of baseline controls involves assessing aspects like IT governance, IT policies, risk assessment processes, physical security, authentication mechanisms, malicious code protection, firewalls, configuration management, automated monitoring, and personnel training.

### Organization-Wide Considerations

- Establishing a baseline based on a control framework should align with the organization's risk appetite.  The seven domains of IT infrastructure are composed of people, processes, and technology.  Risk mitigation strategies include accepting, avoiding, sharing, or controlling the risk.

### Gap Analysis

- Gap analysis compares the current state of controls with the desired state, identifying areas needing action.

### Identifying Documented IT Security Policies

- The organizational security policy framework forms the foundation for information security management.  ISO/IEC 27002 provides a dedicated control objective for security policies.

### Layered Audit Approach

- A layered approach is necessary when systems span multiple domains.  A company's financial system, for example, might involve multiple domains and third-party providers.

### Performing a Security Assessment

- Different approaches exist to identify security weaknesses, including network scans, vulnerability scans, and penetration testing.

### Incorporating Security Assessment into the Audit

- ISACA provides auditing standards and guidelines.  Their suggested penetration testing and vulnerability analysis procedures include planning, skills requirements, agreements, scope questions, various types of penetration testing, physical access controls, social engineering testing, wireless and web application testing, and reporting.

### Using Audit Tools

- Computer-assisted audit tools and techniques (CAATTs) increase auditor productivity.  They are used for testing transactions, reviewing procedures, testing controls, conducting vulnerability assessments, and performing penetration testing.

### Automated Audit Reporting

- Automated tools aggregate data, correlate information, and generate reports, simplifying compliance, improving security, and optimizing IT operations.

### Reviewing Configurations and Implementations

- Configuration management directly impacts security and compliance.  It involves a configuration change control board, baseline configuration management, configuration change control, and configuration monitoring and auditing.  Monitoring helps identify unauthorized changes, misconfigurations, vulnerabilities, and unauthorized systems.

### Verifying Security Controls and Countermeasures

- Auditing security controls involves testing using documents, interviews, and observation.  Each control should have an assessment objective, validated using methods like examination, interviews, and testing.  Assessment objects include specification, mechanism, and activity objects.  The effort required to assess controls varies in depth and coverage.

### Identifying Common Problems

- NIST identifies potential challenges such as time and resources, resistance, temporary behavior, immediate response needs, changing technology, and operational impact.

### Validating Security Operations and Accountabilities

- Security operations and administration are responsible for implementing policies to protect confidentiality, integrity, and availability.  Personnel involved in implementation and administration should be authorized.  Safeguards to prevent attacks include security operation policies, assignment of responsibilities, maintenance procedures, segregation of duties, rotation of duties, least privilege, mandatory vacation, screening, and training and awareness.

## Writing the IT Infrastructure Audit Report

### The report should include an executive summary, a summary of findings, IT security assessment results (risks, threats, vulnerabilities), reporting on control implementation, gap analysis, compliance assessment, and compliance recommendations.

# IT Infrastructure Auditing and Remediation

## IT Compliance Audit Scope

### Compliance Basics

- Organizational policies define operational goals.

- IT security policies protect information and systems' confidentiality, integrity, and availability.

- COBIT is a widely used IT control framework.

### Introduction to IT Infrastructure Auditing

- Objectives include examining security policies and procedures.

- Verifying controls supporting policies and their effective implementation and monitoring.

- Seven domains of a typical IT infrastructure: User, Workstation, LAN, LAN-to-WAN, WAN, Remote Access, and System/Application.  A diagram illustrates these domains and their interconnections.

### Maintaining IT Compliance

- Compliance is an ongoing process requiring a programmatic approach using processes and technology.

- This involves regular security control assessments, configuration and control management, change management processes, and annual security environment audits.

## Compliance within Specific Domains

### Compliance within the User Domain

- Includes employees (fully trusted), contractors (partial access), and guests/third parties (limited access).

- Relevant documentation includes HR manuals and Acceptable Use Policies (AUPs) for IT assets, internet, and email.

- Key aspects include separation of duties, privilege levels, confidentiality agreements, background checks, and a RACI matrix defining responsibilities and accountabilities.  Security awareness training is crucial for new employees.

### Compliance within the Workstation Domain

- Common devices include UPS, desktop computers, laptops/tablets/smartphones, printers, modems/access points, hard drives, and removable storage.

- Focuses on maximizing Confidentiality, Integrity, and Availability (CIA) through access rights and controls.

- Workstation vulnerability management is essential.

### Compliance within the LAN Domain

- Components include connection media, networking devices, servers, networking software.

- LAN traffic and performance monitoring and analysis are key, including optimizing configuration settings and adding security controls.

- Access rights and controls are implemented to maximize CIA.

### Compliance within the LAN-to-WAN Domain

- Components include routers, firewalls, proxy servers, demilitarized zones, honeypots, ISP connections, intrusion detection/prevention systems, data loss/leak security appliances, web content filters, and traffic monitoring devices.

- Monitoring and analysis of LAN-to-WAN traffic and performance are crucial.

- FCAPS (Fault, Configuration, Accounting, Performance, Security) management is essential, along with network management tools and maximizing CIA.

### Compliance within the WAN Domain

- Components include WAN service providers, dedicated lines/circuits, MPLS/VPN WANs, layer 2/3 switches, and backup/redundant links.

- WAN traffic and performance monitoring and analysis, configuration and change management, and management tools are vital.

- Access rights and controls are implemented to maximize CIA.

### Compliance within the Remote Access Domain

- Components include remote users, workstations/laptops, remote access controls/tools, authentication servers, and ISP WAN connections.

- Remote access and VPN tunnel monitoring, traffic and performance monitoring and analysis, configuration and change management, and management tools are necessary.

- Best practices include preventive, detective, and corrective measures to maximize CIA.

## Network Auditing and Assessment Tools

### Nmap (Network Mapper) is used for network exploration and security auditing.

### Wireshark is a network packet analyzer used for troubleshooting, examining security problems, verifying applications, and debugging protocol implementations.

## Network Security Issue Remediation and Infrastructure Hardening

### Assets, Vulnerabilities, Threats, and Exploits

- An asset is any data, device, or component supporting information activities needing protection.

- A vulnerability is a flaw allowing unauthorized access, potentially leading to data manipulation or privilege elevation.

- A threat is a potential danger, such as a malicious hacker.

- An exploit takes advantage of a vulnerability to cause unintended behavior.

### Infrastructure and Vulnerability Assessment (VA)

- Infrastructure includes network devices, services, and servers.

- VA is the process of scanning an information system to identify and document weaknesses.  Motivations for conducting VAs include legal/regulatory constraints, business risks (reputation, financial), and maintaining service continuity.

### VA Techniques and Scoping

- Testing approaches include black box, white box, and grey box testing.

- VA techniques include static analysis (analyzing code structure without exploitation), manual testing (using tester knowledge and experience), and automated testing (using specialized tools). Fuzz testing involves inputting invalid or random data to test system robustness.  Automated tools are available for many of these techniques.

- Scoping a VA involves considering time, budget, resources, and information exposure (black, grey, or white box testing).  A diagram illustrates the VA process, including scoping, reconnaissance, scanning, scoring/categorization/reporting, filtering false positives, and vulnerability analysis.

### Reconnaissance, Scanning, and Reporting

- Reconnaissance aims to gather information in a non-intrusive way (social engineering, internet searching, passive network scanning, dumpster diving).

- Scanning uses tools like Nmap (for open ports and services), ZAP (for web application vulnerabilities), and Metasploit (for vulnerability assessment and penetration testing).

- Vulnerability scoring and reporting often uses the Common Vulnerability Scoring System (CVSS).

### Vulnerability/Security Issue Remediation and Hardening

- Remediation involves applying security patches/updates and system hardening.

- Hardening involves making a system robust against attacks, including strengthening permissions, using secure algorithms, removing unnecessary data/apps, stopping unused services, and enabling firewalls.  CIS guides are a valuable resource for hardening.

