---
title: Secure Data Exchange (SDX)
---
# Getting started with Connected Services

## Secure Data Exchange (SDX)

### What it is

_Secure Data Exchange_ (SDX) helps organizations safely share sensitive information with each other.

It protects information as it moves from one organization to another and ensures that only approved systems can send and receive it.

SDX protects exchanges by:

- Encrypting information while it is being exchanged
- Confirming that participating systems are approved
- Checking that information has not been changed in transit
- Applying rules that control access and permitted actions
- Keeping records of exchanges for auditing and review
- Recording who participated in an exchange when it happened

Together, these controls help organizations protect sensitive information and support B.C.'s security, privacy, and regulatory requirements.

### Who should use SDX

SDX is for organizations participating in Connected Services that need to share sensitive information with other organizations.

Participants may include B.C. government ministries and partner organizations such as LTSA and ICBC.

An organization can:

- Provide information or services to other approved organizations
- Consume information or services provided by another organization
- Do both

### When you should use SDX

Use SDX when information needs to be shared between organizations and the exchange needs stronger security, access control, or accountability.

SDX may be appropriate when:

- Personal, financial, or other sensitive information is being shared
- Access must be limited to approved organizations or systems
- The exchange must be logged or available for audit
- There must be a reliable record of who participated in the exchange

SDX is generally not needed for public or non-sensitive information that does not require these additional controls.

### How it works

Organizations complete the SDX onboarding process before exchanging information. Onboarding sets up the organization, its systems, roles, and secure connections.

Once onboarded:

- Providers make services available to approved consumers. API providers register their APIs using an OpenAPI Specification (OAS).
- Consumers request access to the services they need.
- SDX applies security, access, and logging controls to exchanges between participating systems.

SDX Edge Servers provide the secure connection used by participating organizations.

For detailed setup instructions, see [SDX onboarding documentation](/docs/default/component/aps-infra-platform-docs/how-to/sdx-org-onboarding/).

### Privacy and security responsibilities

SDX provides technical controls that help organizations meet privacy and security requirements.

Using SDX does not replace an organization's responsibility to meet its own privacy, security, governance, and data management requirements.

See [Privacy and security](privacy-and-security.md) for more information about organizational responsibilities and accountability.

### Where to go next

- [SDX onboarding documentation](/docs/default/component/aps-infra-platform-docs/how-to/sdx-org-onboarding/)
