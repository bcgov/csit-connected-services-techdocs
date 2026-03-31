---
title: Privacy and security 
---
# Getting started with Connected Services

## Privacy and security 

_Connected Services_ is built on a secure, policy-driven trust foundation. 

Data remains with the ministry that owns it. Connected Services does not centralize or store program data. Instead, it enables secure, auditable exchange between trusted systems. 

Privacy and security controls are embedded into the technical design, not added afterward. 

### Secure exchange by design 

All data exchange within Connected Services occurs through _Secure Data Exchange_ (SDX), which enforces: 

- Authentication of participating systems 
- Verification that requests are unaltered 
- Real-time access control 
- Timestamped logging of transactions 

These controls ensure that only authorized, policy-compliant requests are fulfilled. 

For technical details on how SDX implements these controls, including request verification and Edge Server architecture, see [Secure Data Exchange (SDX)](secure-data-exchange.md). 

### Data ownership and control 

Connected Services does not take ownership of ministry data. 

- Ministries remain custodians of their data 
- Access decisions are enforced based on predefined policies 
- Data is exchanged directly between approved participants 
- No centralized data repository is created 

This model supports interoperability while preserving program accountability. 

### Identity and access enforcement 

Access is controlled at request time using short-lived, scoped tokens. 

Each request must: 

- Be authenticated 
- Meet defined access policies 
- Be validated before any data is exchanged 

Access enforcement is automated and consistent across participants. 

### Logging, audit, and transparency 

All transactions are logged automatically. 

- Requests are timestamped 
- Actions are auditable 
- Records support compliance and oversight 
- Logging enables accountability without exposing underlying data 

This design supports transparency while minimizing data exposure. 

### Scaling securely 

As Connected Services expands, the same trust and security foundation applies. 

- New partners onboard under shared trust rules 
- Policies are enforced consistently 
- Security controls do not need to be rebuilt for each integration 

This supports scalable, secure interoperability across ministries. 

### How decisions are defined 

Privacy and security controls enforce rules — but those rules are established through governance and policy direction. 

To understand how oversight, accountability, and decision-making structures shape Connected Services, review [Governance and policy](governance-and-policy.md). 