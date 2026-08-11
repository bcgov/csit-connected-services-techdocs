# Introduction

Finding information about government's technical products and services usually means going to multiple systems or relying on word of mouth to figure out who owns what. Integration Toolkit (ITK) brings that information together in one place, so you don't have to.

ITK is the discovery layer for Connected Services BC's products and services. It pulls information from those systems into a consolidated view. This lets you find and understand what's available in one place. When you need the full record, you can go to the original source.

ITK isn't a separate application or portal, you won't find a button, portal, or menu item called "Integration Toolkit" in DevHub. Right now, ITK shows up as documentation, like this and the ones it links to, helping you understand what's available and how to get involved.

The vision for ITK is a searchable catalogue, where a single API or dataset record brings together information from across these systems into one consolidated view. That catalogue is planned for a later milestone.

## What makes up ITK

ITK will bring together information from several products and services, including:

- API Services Portal - APIs available across government
- Authoritative Data Register (ADR) - shared terms, definitions, and standards for data
- Eligibility Factor Verification (EFV) - checking eligibility against authoritative sources
- Secure Data Exchange (SDX) - secure data sharing between systems
- BC Data Catalogue (BCDC) - datasets available across government

Each of these products and services is owned and maintained by its own government team. ITK doesn't replace or govern these products, services, or the teams behind them. Instead, ITK draws information from each of these products and services and brings the data together into a consolidated records, so you don't have to piece it together yourself.

**A quick example**

Pre-ITK, finding this kind of information meant asking around within your team, then other teams, then word of mouth - hoping the right person was still in that role. It often meant checking multiple service catalogues and directories, and still not being sure you'd found the right answer.

With ITK, you will be able to start with what you're trying to do. Say you're building a service that needs to verify an applicant's income as a part of program eligibility. You don't need to know which team owns that check or where it technically lives. You can search or browse by what you're trying to do and discover the right catalogue record - whether that's an API, a dataset, or a data exchange path - along with the documentation to get started.

## Where this fits

Right now, ITK exists as documentation, such as this and the ones it links to. ITK content will live in DevHub and more features and functionality will be added with each milestone as work continues. This documentation explains the ITK concept itself. For details on a specific product or service, like ADR, EFV, SDX, or BCDC, see that team's own documentation, linked in the ITK contributors \[link to ITK contributors\] section.

# ITK contributors

ITK will bring together a defined set of products and services, listed below. This section introduces what's part of ITK, what each one contributes, and where to go for the details. This list is expected to grow as more products and services are added over time. If you're interested in finding out more, please \[reach out\].

**API Services Portal**  
Brings APIs available across government. If you're looking to connect to or publish an API, this is where those records live. See the [API Services Portal technical documentation](https://developer.gov.bc.ca/docs/default/component/aps-infra-platform-docs/) for onboarding and technical details.

**Authoritative Data Register (ADR)**  
Brings shared terms, definitions, relationships, and standards for data. ADR maintains the Connected Services Glossary. It keeps shared terms consistent across government, including what it means for data to be authoritative. This way, a dataset described one way in one place matches how it's described everywhere else. See the ADR documentation \[link\] for details.

**Eligibility Factor Verification (EFV)**  
Brings the ability to check eligibility against authoritative sources. EFV lets you verify that someone meets program or service requirements, such as income or residency. See the EFV documentation \[link\] for details.

**Secure Data Exchange (SDX)**  
Brings secure data sharing between systems. SDX supports the exchange of data between providers and consumers where a direct, secure connection is needed. See the SDX documentation \[link\] for details.

**BC Data Catalogue (BCDC)**  
Brings datasets available across government. If you're looking for a dataset to work with, BCDC is where its metadata is registered and maintained. ITK surfaces what's in BCDC and shows you how to access it. See the BCDC documentation \[link\] for details.

## **How products and services are integrated into ITK**

Each product or service is owned and maintained by its own government team, which is responsible for its data and accuracy over time. API Program Services works with contributing teams to help their data show up in ITK in a consistent way - things like how it's discovered, how it's understood, and how someone can access it. The Developer Experience (DevX) team governs DevHub. DevHub is the platform that ITK will live in, and DevX supports the underlying platform and technical setup that makes this possible.

# Finding and using ITK

## Using ITK today Right now, ITK is mostly documentation. You can discover it by browsing or searching this TechDoc and the ones it links to, then read it to understand what a product or service does, who maintains it, and how to get involved

## The vision for ITK

Once the catalogue is available, every record in ITK will follow the same basic pattern: you'll discover it, understand what it does, try it, and request access. This is what each step is expected to look like. For the latest on what's actually been delivered, see Milestone updates \[link to Milestone page\].

ITK will surface more than one kind of thing: APIs, datasets, and documentation, with more planned over time, like templates for building an SDX API. You'll be able to start with a search for what you're trying to do, then filter to narrow down by owner, type, or other criteria. Results will show as cards you can scan at a glance before opening anything.

**Understand**

Once you've found something, its record will tell you what it does, who maintains it, and its security requirements and access conditions. The record could be an API or a dataset. From there, you'll also be able to reach related glossaries, data dictionaries, and support paths.

**Try**

Where available, you'll be able to test a record before committing to it, for example trying a sample API call or previewing a dataset's structure.

**Request**

When you're ready to move forward, the record will point you to the next step, whether that's requesting API access, requesting a data exchange connection, or downloading a dataset.

**A quick example**

Say you're building a service and need to verify an applicant's income as part of program eligibility, the same scenario from the Introduction. Once the catalogue is available, you'll be able to discover the EFV income verification record by searching for "income" or "income verification," then filtering by eligibility-related records. You'll understand what it checks and what it needs from you using its record. Then you'll try a sample request to see the response format, and finally request production access when you're ready to integrate.

Check Milestone updates for the latest on what's actually available today.

# Milestone updates

This page will be updated with milestone updates and release notes as we continue to make progress on ITK.

# Support

If you have a question about ITK, submit a support ticket\[ITK general enquiries\]. APS will answer directly or direct you to the right team.

Each contributor (API Services Portal, ADR, EFV, SDX, BCDC) has its own support mechanism, available on their documentation pages. See the ITK Contributors section for links.

If you're looking at a specific API or dataset record in ITK, that record also has its own support contact for targeted help.