# Enterprise applications: access and qualification

Assessment date: October 25, 2026. These are routes to a lab, not certified integrations. No new vendor account, tenant, trial, paid service or Google sign-in was initiated.

| Platform | Feasible path | Current status |
|---|---|---|
| [Oracle](enterprise/oracle.md) | Versioned APEX Customers sample; Fusion/EBS in a separate test environment | Public APEX source fork; compatible workspace needed |
| [SAP](enterprise/sap.md) | Existing Fiori/CAP source; approved S/4HANA/ECC landscape | Source available; actual ERP sandbox needed |
| [Workday](enterprise/workday.md) | Personal development tenant beta or existing test tenant | Current public access route found; allocation/demo rights unverified |
| [ServiceNow](enterprise/servicenow.md) | Approved licensed/partner demo instance | PDI exists for learning, but business use is excluded in its guide |
| [Pega](enterprise/pega.md) | Practice environment or approved nonproduction tenant | Practice route and SDK found; instance/version/demo rights unverified |
| [Infor](enterprise/infor.md) | Product-specific nonproduction tenant | Product and access must be selected |

## Pilot sequence — recommendation

1. Deploy the existing SAP Fiori/CAP sample and import Oracle Customers into a compatible, approved APEX workspace.
2. Qualify Workday's newer personal development route and Pega practice access. An available personal trial does not establish permission for a shared commercial demo.
3. Use approved nonproduction/partner environments for ServiceNow, SAP ERP and Infor. Reuse an existing authorized tenant where possible.
4. Keep existing Salesforce scratch-org/sandbox work in the same access/verification process.

A public repo contains test assets, synthetic fixture definitions, setup notes and redacted evidence. It does not redistribute proprietary enterprise platforms or expose private tenant credentials. Use recordings with explicit provenance when a shared public environment is unavailable and the vendor permits publication.

## Ready for crawling only after

The actual browser URL, product/version, user role, authentication path and reachable surface are established. Begin with bounded read-only discovery. Review generated writes against a disposable test fixture; prevent outbound messages, purchases or irreversible business actions. Capture actual assertions and results. Native terminal/desktop surfaces need separate runner qualification.

## Engineering handoff

For each platform record: environment owner, permitted use, expiry/cost, runtime/version, browser surface, dedicated roles, synthetic seed/reset, evidence publication scope and the first agreed scenario. Do not assign team commitments or promise a date until an owner accepts the work.

## Related future candidates

Dynamics 365, NetSuite, SAP SuccessFactors and Oracle PeopleSoft/JD Edwards can be assessed next; no availability or support is claimed here. IBM i/mainframe remains a separate terminal/environment track.
