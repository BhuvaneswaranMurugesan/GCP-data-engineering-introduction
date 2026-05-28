# Key Security terms and concepts

1.The privileged access:
The privileged access security model grants specific users access to a broader set of resources than ordinary users.

2.Least Privilige:
The least privilege security principle advocates granting users only the access they need to perform their job responsibilities.

3.Zero-trust architecture:
The zero-trust architecture security model assumes that no user or device can be trusted by default.
Every user and device must be authenticated and authorized before accessing resources.

## These next three concepts relate to how an organization can protect itself from cyber threats.

- Security by default => a principle that emphasizes integrating security measures into systems and applications from the initial stages of development.

- Security posture => refers to the overall security status of a cloud environment.
It indicates how well an organization is prepared to defend against cyber attacks by evaluating their security controls, policies, and practices.

- Cyber resilience =>refers to an organization's ability to withstand and recover quickly from cyber attacks.
It involves identifying, assessing, and mitigating risks, responding to incidents effectively, and recovering from disruptions quickly.

## essential security measures to protect cloud resources from unauthorized access.

1.Firewall - A firewall is a network device that regulates traffic based on predefined security rules.
It follows certain rules to decide which traffic is allowed to enter or leave a network.
These rules help keep unauthorized people or harmful things away from important cloud resources, such as servers, databases, and applications.

2.Encryption  - the process of converting data into an unreadable format by using an encryption algorithm.

3.Decryption - however, is the reverse process that uses an encryption key to restore encrypted data back to its original form.
Safeguarding the encryption key is crucial, because it holds the secret algorithm necessary for decrypting the data.

Another way to think about encryption and decryption is writing a message in a secret language that only you and the person you want to send it to can understand.

# Cloud security components

Confidentiality, Integrity, and Availability. (CIA)

These three principles form the foundation of the “CIA Triad”, a widely used model for developing effective security systems.
The CIA triad emphasizes the importance of protecting sensitive information, ensuring data accuracy and trustworthiness, and maintaining uninterrupted access to resources and services.

# Secure Storage

encryption protects your data in different states.

When data is at rest, it's stored on physical devices like computers or servers.
By encrypting data at rest, even if someone gains physical access to the device, they won't be able to decipher the data without the encryption key.

And if you prefer to manage your encryption keys yourself, you can use our Cloud Key Management Service (Cloud KMS) for added control.

Uses AES (Advanced Encription Standards).

# 3A's

1.Authentication
2.Authorization
3.Auditing

# Network Security

- With Google Cloud's BeyondCorp Enterprise, you can implement a zero trust security model.

- Google Cloud provides private access methods via Cloud VPN and Cloud-interconnect
which let you establish secure connections between your on-premises networks and Google Cloud resources.

- Protect your perimeter with Google Cloud's powerful tools.
Google Cloud offers various methods to help secure your perimeter, including firewalls and Virtual Private Cloud.

Google Cloud provides service to protect are,

- VPC
- firewall
- Cloud VPN
- Cloud-interconnect

External web applications and services are often targeted by cyber threats, including DDoS attacks.
DDoS, which stands for distributed denial-of-service, is a cyber attack that uses multiple compromised computer systems to flood.

Security Operations: (Sec-Ops)

- Google Cloud's Security Command Center (SCC) provides a centralized view of your security posture.
- Google Cloud offers Cloud Logging, a service to collect and analyze security logs from your entire Google Cloud environment.

