---
title: Secure Data Exchange (SDX) 
---
# Getting started with Connected Services

## Secure Data Exchange (SDX) 

### What it is 

_Secure Data Exchange_ (SDX) serves as the secure exchange layer within Connected Services, enabling the controlled and protected transfer of data between participating organizations. 

The exchange operates behind the scenes to ensure that when a citizen’s information is sent or received, the data remains protected throughout the process - from initial exchange to storage. 

SDX is built around two foundational components: 

- **Security Controls**  
This includes encryption, authentication, and data integrity mechanisms that protect information in transit and verify participating systems. 
- **Governance and Compliance**  
This includes auditing and logging functionality, policy enforcement, non-repudiation, and timestamping to support oversight and accountability. 

Together, these components ensure that sensitive data exchanged through SDX maintains confidential, protected, and compliant with B.C.’s security and regulatory requirements. 

### Who this is for 

SDX is intended for any organization participating in Connected Services that needs to securely exchange sensitive data across organizational boundaries. 

This includes organizations such as LTSA and ICBC, as well as other ministries and partners. 

Participating organizations may act as data providers, data consumers, or both. 

### When to use Secure Data Exchange 

SDX is required when sensitive data (e.g., personal, financial, or health-related information) is being shared across organizational boundaries. 

Use SDX when: 

- Data exchange requires enhanced security controls due to sensitivity of the data 
- Policy-based access enforcement is needed 
- Auditability and non-repudiation are required 

SDX is not required for public or non-sensitive data that does not require cross-boundary security controls. 

### How it works (high-level) 

SDX operates through an onboarding and registration process within the SDX ecosystem. 

At a high level: 

1. The SDX Operator registers their organization. 
2. An Organization Administrator assigns the necessary System Owner role(s). 
3. The System Owner(s) register(s) services and subsystems and is able to browse the service catalog. 
4. An OpenAPI Specification (OAS) file is submitted for API registration. This spec must be in YAML format.  
5. Once onboarded, an Edge Server is then provisioned. 
6. Secure connections are established between participating systems within the SDX ecosystem. 

All exchanges are authenticated, authorized, and logged automatically. 
 
Detailed onboarding steps and technical configuration guidance are available in [SDX Onboarding – TechDocs](/docs/default/component/aps-infra-platform-docs/how-to/sdx-onboarding). <span style="color:red; font-weight:bold">TODO Unstable link!</span> 

### Relationship to privacy and security 

SDX provides the technical implementation of the privacy and security controls described in Privacy and Security. 

Review Privacy and security for information on governance alignment and accountability structures. 

### Where to go next 

- [SDX Onboarding – TechDocs](/docs/default/component/aps-infra-platform-docs/how-to/sdx-onboarding) <span style="color:red; font-weight:bold">TODO Unstable link!</span> 